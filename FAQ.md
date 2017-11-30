关于安装程序工作目录
安装程序在其工作目录中存储有关安装会话的数据。例如，此类数据包括系统中已安装的组件列表、安装日志消息以及注册表数据。
对于 Windows，安装程序工作目录的默认位置为 %USERPROFILE%\.nbi；对于其他平台，默认位置为 ~/.nbi。日志子目录中包含安装日志文件。
清理不完整的安装
如果未执行完整的安装或者安装不成功，则可能需要在系统中清理以前的安装。
对于 Microsoft Windows 和 Linux：
删除安装程序工作目录。
删除 IDE 和 GlassFish 应用服务器的安装目录。
在 Windows 平台上，从以下注册表键中删除所有 nbi* 注册表项：HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\Uninstall HKEY_CURRENT_USER\SOFTWARE\Microsoft\Windows\CurrentVersion\Uninstall
对于 OS X：
将程序文件夹或文件拖至“回收站”。
安装前禁用某些软件
开始执行安装前，最好禁用防火墙、防病毒和监视应用程序。它们中的某些应用程序可能会阻止安装过程中正确配置 IDE 组件。
例如，如果系统上正在运行 Logitech 进程监视应用程序 (LVPrcSrv.exe)，请在执行安装前将其关闭。
