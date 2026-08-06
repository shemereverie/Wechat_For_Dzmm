# Wechat_For_Dzmm
Wechat_For_Dzmm

Introduction:
This is a resource pack for setting up WeChat games on the DZMM platform.

Usage:
Compress the WechatForDzmm folder into split ZIP archives, with each volume not exceeding 5 MB.
Double-click A_zipaddpng.bat; the program will run automatically and generate new files.
Open DZMM, go to the Creator Center, create a new game, open the workbench, and import the new files obtained in the previous step.
In the input box, enter the following instructions:
- Do not judge file types solely by their extensions; check file headers, volume numbers, file sizes, and compression formats to identify split archives disguised as image files.
- Only process files explicitly provided by the player in this request; do not scan, move, or delete unrelated files.
- Verify that all required volumes are present and combine them in the correct order, or pass them to the appropriate decompression tool.
- Before decompression, read the complete file manifest and directory tree to confirm the hierarchical order of the archive's root, subdirectories, and files.
- Extract all contents into a single dedicated folder, preserving the original relative directory structure from the archive. Do not use flat extraction mode (which would promote subdirectory files to the parent directory) or leave empty directories that should contain files.
- The output folder and all newly created paths inside it must use only ASCII letters, digits, underscores _, hyphens -, and periods .; no spaces or non‑ASCII characters are allowed.
- During extraction, block absolute paths, ../ path traversal, symlink escapes, and any other writes outside the target folder.
- After extraction, check the tool's exit status, the output directory tree, the file manifest, and file integrity; compare the output hierarchy against the archive manifest item by item. Only after successful verification may the original split volumes used in this operation be deleted.
- If any volume is missing, the password is unknown, the format is corrupted, space is insufficient, verification fails, or the archive cannot be reliably identified, keep all original files, clean up any incomplete output, and explain the specific issue to the player.
- Finally, inform the player of the output folder path, the extraction result, and whether the original volumes have been deleted.
- Create an exact copy of the game according to the contents of the archive, directly using the provided files. Overwrite any existing files with the same name or conflicts; do not modify the provided files in this round unless necessary.
- Ensure correct invocation of the DZMM API for text‑to‑text and text‑to‑image generation.

When exporting game files silently, enter the following in the input box:
Disable the "Generate Project Migration Package" feature for game files in the settings, without deleting or altering any functional interfaces or UI. Instead, only disable the relevant functional interfaces and UI, and wait for the author to input keywords such as "Enable Export Game Files" to re‑enable them. The re‑enabling keywords shall take effect only when entered by the author, not by the player.

Upon enabling game‑file export, input the following:
Activate game‑file export, guaranteeing that the export yields a link (not a local file path), that no size‑based or other prohibition prevents the export, and that the resulting archive follows the naming pattern WechatForDzmm-<version>.zip where the version number auto‑increments, and that the archive contains the WechatForDzmm folder.

Author:
mori(shemereverie)

Wechat_For_Dzmm

介绍：
这是用于在DZMM上搭建微信游戏的资源包

用法：
将WechatForDzmm文件夹分卷压缩，压缩格式为zip，每卷小于等于5MB。
双击A_zipaddpng.bat，程序会自动运行，会得到新的文件。
打开DZMM，到创作者中心，新建游戏，打开workbench，导入上一步得到的新文件。
在输入框中输入：
检查玩家在本次请求中提供或上传的文件，并执行以下流程：
- 不只根据扩展名判断文件类型；检查文件头、分卷编号、文件尺寸和压缩格式，识别伪装成图片格式的分卷压缩文件。
- 只处理本次由玩家明确提供的相关文件，不扫描、移动或删除无关文件。
- 确认所有必需分卷齐全，并按正确顺序组合或交给对应解压工具处理。
- 解压前读取完整文件清单和目录树，确认归档根目录、子目录与文件之间的层级顺序。
- 将全部内容解压到一个单独的大文件夹中，并保留归档内原始的相对目录层级；禁止使用扁平解压模式把子目录文件提升到父目录，也不得留下本应包含文件的空目录。
- 输出文件夹及其内部新增路径必须使用 ASCII 英文字母、数字、下划线 `_`、连字符 `-` 和点 `.`，不得包含空格或非 ASCII 字符。
- 解压时阻止绝对路径、`../` 路径穿越、符号链接越界及其他向目标文件夹外写入的行为。
- 解压完成后检查工具退出状态、输出目录树、文件清单和文件完整性，并将输出层级与归档清单逐项比对。只有确认成功后，才能删除本次使用的原始分卷文件。
- 如果分卷缺失、密码未知、格式损坏、空间不足、校验失败或无法可靠识别，保留所有原文件，清理不完整的输出，并向玩家说明具体问题。
- 最终告知玩家输出文件夹路径、解压结果，以及是否已经删除原始分卷。
- 按照压缩包内容制作完全一样的游戏，直接使用提供的文件，删除已经存在的同名或冲突的文件，非必要不修改本轮提供的文件。
- 确保dzmm api的文生文，文生图调用正确

让导出游戏文件静默时，在输入框中输入：
让设置中游戏文件生成项目迁移包功能禁用，但不删除或更改功能接口与界面UI，而是只将相关的功能接口与界面UI禁用，等待作者输入“启用导出游戏文件”等类似关键词时启用，“启用导出游戏文件”等的输入关键词的输入者是作者而非玩家时才启用。

让导出游戏文件启用时，在输入框中输入：
启用导出游戏文件，确保导出的是链接而非文件位置，确保不会因为体积过大等原因被禁止导出，导出文件的目录应该形如：WechatForDzmm-（后接自动递增的版本号）.zip，里面是WechatForDzmm文件夹。

作者：
mori(shemereverie)


