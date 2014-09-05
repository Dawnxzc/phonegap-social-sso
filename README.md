# phonegap-social-sso

I think people who will use this plugin should be Chinese, so I'll use Chinese in following content. YOOOOOOOO!

这是phonegap plugin，用来做第三方平台登录的，目前有qq、微博、人人三个平台


## qq登录

首先要在[qq互联](http://connect.qq.com/)，创建移动应用，获取appId神马的

然后搭建环境，[ios环境搭建看这里](http://wiki.connect.qq.com/ios_sdk%E7%8E%AF%E5%A2%83%E6%90%AD%E5%BB%BA)，[android的在这里](http://wiki.connect.qq.com/%E5%88%9B%E5%BB%BA%E5%B9%B6%E9%85%8D%E7%BD%AE%E5%B7%A5%E7%A8%8B_android_sdk)

环境配好了，Next，就是写代码了，直接把`.java`和`.m` `.h`文件copy到工程里，然后把`www/plugins`下的`qqLogin.js`拷贝到对应的`www/plugins`目录下

还有一步，在工程的`cordova_plugins.js`和`config.xml`里增加对应plugin的说明
ios版

<feature name="QQLogin">
    <param name="ios-package" value="QQLogin" />
</feature>



android版

<feature name="QQLogin">
    <param name="android-package" value="com.example.cordova.qqLogin.QQLogin" />
</feature>


注意，android版`value`对应的是`QQLogin.java`这个文件所在的路径



## 微博登录

和qq基本一致，微博的文档po主放在doc目录下了





## 人人登录

人人文档在这里，[ios版](http://wiki.dev.renren.com/wiki/V2/sdk/objectivec_sdk)，[android](http://wiki.dev.renren.com/wiki/V2/sdk/android_sdk)

步骤和前面的一致



po主真是活雷锋有木有！！（～￣▽￣～）