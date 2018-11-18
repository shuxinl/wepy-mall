https://github.com/dyq086/wepy-mall

https://tencent.github.io/wepy/document.html#/  vscode 安装插件

https://segmentfault.com/a/1190000013860866  小程序踩坑记 


wepy-mall\src\api\api.js 配置接入层地址

其他的说明看README.MD 文件说明

开发:
2018年11月7日：beautiful-wpy  crtl+ shift + 6 代码美化 
https://blog.csdn.net/zhao_gao/article/details/53485313    net::ERR_PROXY_CONNECTION_FAILED 解决异常

上线注意事项：
检查的oss 上传的域名重新配置一个OSS子账号

项目记录：
    2018年11月7日:
    https://blog.csdn.net/qq_38125123/article/details/73870667 方案： api提供获取签名(signature)和加密策略(policy)后发起上传
    组件 upload.wpy(upload_save.png,upload_save.png 后台提供一个获取授权策略的接口)
    上传策略： 应用授权 -> 获取授权策略、签名-> 直传到oss上面
    生成的业务情景： 授权key地址 + 日期文件夹 + 时间戳做为文件名 + 文件后缀
    文件区分:
    1、上传的文件动态数据展示 放在upload目录 情景：上传量大的需要进行冗余数据清除的
    2、上传文件静态数据放在static 目录下，类似配置logo等信息少量低频的文件进行存放，不进行冗余数据删除


