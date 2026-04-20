# Dogdou 使用指南

[返回仓库首页](../README.md) | [英文使用指南](./guide.en.md) | [中文变更日志](./changelog.zh-CN.md)

## 安装

1. 从仓库 `Releases` 页签下载安装包。
2. 以管理员权限运行安装程序。
3. 安装文件会被复制到 `%ProgramData%\Dogdou`。
4. 安装程序会注册卸载项、驱动与 `DogdouService` 服务。

说明：

- 安装包不存放在仓库代码树中
- 正式 `.exe` 和校验文件应从发布页下载

![安装界面](./media/install.png)

## 首次启动

1. 从桌面快捷方式或安装目录启动 `DogdouToolkit.exe`。
2. 左侧当前主要入口包括：
   - `会话`
   - `凭据`
   - `关于`
3. 首次使用建议先创建一个凭据。

## 创建凭据

1. 打开 `凭据` 页面。
2. 点击 `+ 新建`。
3. 创建一个后续用于会话启动的凭据条目。

![凭据设置 1](./media/credentials-setup-1.png)
![凭据设置 2](./media/credentials-setup-2.png)
![凭据设置 3](./media/credentials-setup-3.png)

## 启动会话

1. 返回 `会话` 页面。
2. 在 `选择凭据` 中选择凭据。
3. 填写宽度、高度和刷新率。
4. 如需 Shell，可启用 `启动时打开 Shell`。
5. 点击 `启动会话`。

真实界面截图：

![会话启动 1](./media/start-session-setup-1.png)
![会话启动 2](./media/start-session-setup-2.png)
![会话启动 3](./media/start-session-setup-3.png)
![会话启动 4](./media/start-session-setup-4.png)
![本地连接示例](./media/local-linker-game-example.png)

## 创建进程并连接

1. 在会话列表中确认会话已创建。
2. 在 `命令行` 中填写程序，例如 `cmd.exe`。
3. 在 `工作目录` 中填写目录，例如 `%USERPROFILE%`。
4. 点击 `创建进程`。
5. 点击 `连接会话` 进入该环境。
6. 如需处理音频，可在开启新会话前使用 `音频复用`，在需要恢复时使用 `恢复音频`。
