# Troubleshooting

> Auto-generated from evolutions.json. Do not edit directly.

<a id="ev_ee253580"></a>
### [ev_ee253580] 编辑文件前必须先用 read_file 读取目标文件的最新内容，且每次切换目标文件时都要重新 read，即使之前读过其他文件；禁止直接用 bash 写文件，应优先使用 code 工具执行...
### 文件编辑失败（edit_file 要求先读取文件）
- 在编辑任何文件（包括但不限于 `IVT.md`、`references/*.md`、`call_log/*.md` 等）之前，必须先用 `read_file` 工具读取该文件的完整内容，否则 `edit_file` 会返回错误：`File must be read before editing.`
- 即使你之前已经读过其他文件，在切换编辑目标时，必须重新 `read_file` 读取新目标文件；如果在读取后执行了其他操作（如编辑另一个文件、调用其他工具），open 状态可能丢失，应再次 `read_file` 确认后再编辑。
- 如果 `edit_file` 持续失败，改用 `code` 工具执行 Python 脚本进行写入：先 `read_file` 获取内容，在内存中完成替换/插入，再通过 `code` 执行 Python 写入（使用 `open(path, "w", encoding="utf-8")`）。
- 绝对禁止使用 bash 的 `echo`、`Set-Content`、`Out-File` 等命令写文件，否则会导致编码丢失（Windows 默认 GBK）或 UTF-8 BOM 丢失问题。

*Source: execution_failure | 2026-07-12T03:56:02.901690+00:00*

---

<a id="ev_78ea4ea8"></a>
### [ev_78ea4ea8] 批量更新多个诗作分析文件时，先一次性 read_file 所有目标文件再逐文件修改后写回，避免重复读取和工具状态丢失
### 批量更新多个文件时的读取策略
- 当需要更新多个诗作分析文件（如添加新分析列）时，不要逐个文件边读边修改，应先用 read_file 一次性读取所有目标文件的完整内容，存入内存字典（按文件路径分组），再逐文件执行修改和写入。
- 避免在读取一个文件后立即编辑写入，否则可能因工具状态丢失导致后续文件需要重新读取，降低效率。正确的做法：先读取全部文件，再统一写入。
- 写入时倾向于使用 code 工具执行 Python 脚本（open/write），而非 edit_file，因为 edit_file 需要文件处于 open 状态，批量场景下频繁切换容易触发“File must be read before editing”错误。

*Source: script_artifact | 2026-07-12T11:10:51.713974+00:00*

---

<a id="ev_8611c001"></a>
### [ev_8611c001] 编辑文件时，优先使用 read_file + code 执行 Python 脚本；禁止用 bash/PowerShell 写文件；批量操作前一次性读取所有文件到内存再统一写入
### 文件编辑故障处理（通用）
- 编辑任何文件前必须先调用 `read_file` 读取最新内容；切换编辑目标文件时必须重新 `read_file`（即使之前读过其他文件），否则 `edit_file` 返回 `File must be read before editing`。
- 如果 `edit_file` 因字符串匹配失败或 open 状态丢失而报错，立即降级为：使用 `code` 工具执行 Python 脚本（`open(path, "w", encoding="utf-8")`）完成写入。此方法不受文件 open 状态限制，且保证 UTF-8 编码。
- 绝对禁止使用 bash 的 `echo`、`Set-Content`、`Out-File` 等命令写文件（Windows 下默认非 UTF-8 编码），也禁止使用 PowerShell 进行文件内容搜索或统计（路径中的冒号会导致变量引用语法错误）。
- 批量更新多个文件时：先用 `read_file` 一次性读取所有目标文件内容存入内存字典（key=文件路径），再逐个修改并统一写入；避免每处理一个文件就执行一次 `edit_file`。写入一律使用 `code` 执行 Python 脚本。
- 每次写入后立即用 `read_file` 验证内容是否已变更；未变更则视为失败并降级处理。

*Source: script_artifact | 2026-07-12T12:11:00.754428+00:00*

---

<a id="ev_2d51b6a4"></a>
### [ev_2d51b6a4] 在 Windows 环境下进行文件内容搜索或统计时，应避免使用 PowerShell 命令（路径冒号导致语法错误），优先使用 bash 的 grep 或 Python 脚本
### Windows 环境下文件搜索/统计工具选择
- 执行 `grep` 等文本搜索命令时优先使用 bash 工具（Unix 风格路径），避免使用 PowerShell 内置命令（如 `Select-String`、`grep` 的 PowerShell 模拟）。
- Windows PowerShell 中文件路径包含冒号（如 `C:\...`）时，冒号会被误解析为变量引用前缀，导致 `InvalidVariableReferenceWithDrive` 错误。
- 如果需要跨平台兼容或统计大量文件，推荐编写简短的 Python 脚本（`re` / `os.walk`）并通过 `code` 工具执行，既避免编码问题也避免路径解析错误。

*Source: script_artifact | 2026-07-12T12:11:00.754428+00:00*

---

<a id="ev_e3005918"></a>
### [ev_e3005918] 在读取参考文件（如 references/IVT_core.md）时，必须指定包含文件名的完整文件路径，不能只提供目录路径，否则 read_file 会返回 File not found 错误
### 读取参考文件时需指定完整文件路径
- 在 `read_file` 参考文件（如 `references/IVT_core.md`、`assets/analysis_template.md` 等）时，必须提供包含文件名的完整路径，不能只提供目录路径。例如，正确的路径是 `references/IVT_core.md` 或 `assets/analysis_template.md`，而不是 `references/` 或 `assets/`。
- 如果只提供目录路径，`read_file` 会返回 `File not found: ...\references` 错误（错误码 199003），因为系统无法读取一个目录作为文件。
- 在 Windows 环境下，建议使用相对路径（如 `references/IVT_core.md`），并确保当前工作目录正确；如果需要绝对路径，可使用 `os.path.join(workspace_path, 'references/IVT_core.md')` 构造。
- 执行 `read_file` 前，最好先确认文件是否存在，可用 `list_files` 列出目录内容验证。

*Source: execution_failure | 2026-07-12T14:11:11.607003+00:00*

---
