# 🚀 JustRunMy 自动续期（GitHub Actions）

一个基于 GitHub Actions 的自动化脚本，用于定时登录并自动续期 JustRunMy 应用。

为了保护账号和代理安全，所有敏感信息均通过 GitHub Secrets 进行配置。

──────────────────────────────

【⚙️ 必须配置的环境变量】

在运行脚本前，你必须在 GitHub 仓库中添加以下 3 个 Secrets 变量。

📍 配置路径：

进入你的 GitHub 仓库
➡ 点击顶部 Settings
➡ 点击左侧 Secrets and variables
➡ 点击 Actions
➡ 点击绿色按钮 New repository secret

──────────────────────────────

【📝 需要添加的 3 个变量】

1️⃣ 变量名：JUSTRUNMY_EMAIL
Secret 填写：你的 JustRunMy 登录邮箱
示例：abc@def.com
说明：JustRunMy 登录邮箱

2️⃣ 变量名：JUSTRUNMY_PASSWORD
Secret 填写：你的 JustRunMy 登录密码
示例：abc123
说明：JustRunMy 登录密码

3️⃣ 变量名：GOST_PROXY_TARGET
Secret 填写：你的 Gost 代理完整地址
示例：socks5://用户名:密码@123.456.789.012:1234
说明：必须包含协议（socks5/http 等）

──────────────────────────────

【📌 示例格式参考】

JUSTRUNMY_EMAIL=abc@def.com
JUSTRUNMY_PASSWORD=abc123
GOST_PROXY_TARGET=socks5://x:x@123.456.789.012:1234

──────────────────────────────

⚠️ 注意事项：

- 必须使用 Repository Secrets
- 不要写入代码文件
- 不要提交到仓库
- 三个变量必须全部填写
