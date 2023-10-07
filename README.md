注册一个 SparsePackage，至少需要 build19041 win2004 的系统。

自己通过makeappx建立一个msix包，再对其签名。

再建立一个win32程序，调用AddPackageOptions(winrt-19041引入)，将实现的IExplorerCommand的dll与msix打包在一起。（即使是使用命令行Add-AppxPackage -ExternalLocation参数也是该版本同时引入的）

这样打包好的win32应用还必须自行处理卸载，可以通过命令行也可以通过code。
