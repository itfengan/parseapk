# parseapk是一个解析apk信息的库.
给定一个Android apk或者iOS itunes地址获取应用的信息.

**使用前请配置aapt的环境变量**(我实在mac写的,直接跑🏃).在win下如果你有灵性请修改下ApkUtil的mAaptPath并使用它!
1. 仅获取APK应用信息
   * Android  
ApkInfo apkInfo=ApkUtil.getInstance().getApkInfo(path)
   * iOS  
ApkInfo apkInfo=ApkUtil.getInstance().getIOSInfo(url)
2. 获取APK信息并获取应用图标
   * Android  
ApkInfo apkInfo=ApkWithIconUtil.getApkInfoAndroid(apkpath,iconoutputpath)
   * iOS    
ApkInfo apkInfo=ApkWithIconUtil.getApkInfoIos(iOSUrl,iconoutputpath)

cool~
