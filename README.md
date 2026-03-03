JustRunMy 自动续期
这是一个基于 GitHub Actions 的自动化脚本，用于定时登录并续期 JustRunMy 应用。为了保护你的账号和代理安全，所有敏感信息均已通过 GitHub Secrets 进行配置。

⚙️ 变量配置（必须填写）
在运行此脚本前，你必须在 GitHub 仓库中添加以下 3 个环境变量。

配置路径：
进入你的 GitHub 仓库 ➡️ 点击顶部的 Settings ➡️ 左侧菜单找到 Secrets and variables ➡️ 点击 Actions ➡️ 点击绿色的 New repository secret 按钮。

Name (变量名),Secret (变量值填写示例),说明
JUSTRUNMY_EMAIL,abc@def.com,你的 JustRunMy 登录邮箱
JUSTRUNMY_PASSWORD,abc123,你的 JustRunMy 登录密码
GOST_PROXY_TARGET,socks5://x:x@123.456.789.012:1234,你的 Gost 代理完整地址
