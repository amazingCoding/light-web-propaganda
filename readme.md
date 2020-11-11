# LightWeb - 为你的 app 加入 小程序 功能

## 一行代码接入
* 前端
  ```typeScript
  // 初始配置
  const conf = {
    isHideNav: false,
    statusStyle:ThemeTypes.light,
    title: 'demo',
    titleColor: '#ffffff',
    navBackgroundColor: '#000000',
    backgroundColor: '#f1f1f1',
    bounces: true
  }
  // 通过 new LightWebCore 实例来创建 lightWeb 容器
  const lightWeb = new LightWebCore(conf,success,fail)
  ```
* 安卓 Java
  ```java
  LightWebCoreActivity.createLightWebView(activity,loadZipURL,maxRouter,true);
  ```
* iOS Object-C
  ```Object-C
  LightWebCoreController *app = [[LightWebCoreController alloc] initWithURL:loadZipURL isDev:YES withMaxRouter:maxRouter];
  [self presentViewController:app animated:YES completion:nil];
  ```
## electron 制作的 PC 工具辅助
  * 完整的 devTool 工具
  * 便捷的 dark / light 切换
  * 和 客户端 一般的体验

## 不断拓展的新功能
  * 九个方法
    * init
    * pageConfig
    * vibrate
    * Clipboard
    * Local Router System
      * push
      * pop
      * replace
      * setPopExtra
      * restart
  * 五个事件
    * app show
    * app background
    * view show
    * view hidden
    * sceneMode
  * more to do
  