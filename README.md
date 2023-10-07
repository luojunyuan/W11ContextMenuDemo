注册一个 SparsePackage，至少需要 build19041 win2004 的系统。
自己通过makeappx建立一个msix包，再对其签名。
再建立一个win32程序，调用AddPackageOptions(winrt-19041引入)，将实现的IExplorerCommand的dll与msix打包在一起。
