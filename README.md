# ZYPlayer
基于 AVFoundation AVPlayer 的视频播放器 swift 3.0

## 关于 ZYPlayer
* ZYPlayer是一款基于AVPlayer的视频播放器
* 支持横竖屏旋转功能
* 支持手势控制快进，亮度调节，音量调节
* 支持重播功能
* 集成视频播放器常用的UI界面

## 支持版本与编译测试
* 由于本项目并未使用过新的AIP 理论上支持iOS8+。其他版本请自行测试。 经过测试的版本iOS9,iOS10。(真机)
* 编写工具XCode8.1

## 如何使用
* 集成
  * 1.下载demo文件，将demo中的ZYPlayer文件夹整体拖拽到你的项目中。不需要添加其他的依赖
  * 2.仿造demo中 ViewController里面唯一的便利构造函数进行初始化。其中需要的参数注释已经说明
  * 3.由于播放器需要支持屏幕旋转，如果不希望在使用次播放器碰到问题，请认真查看demo里面的注释
  * 4.播放器内使用了定时器，为了不造成内存问题，在退出界面的时候请参照demo 手动销毁播放器
  
## 如何扩展
* 1.ZYPlayer 本身是一个UIViewController, 内部集成了AVPlayer。设计之初，就考虑到了不同的用户需求。所以在UI界面上，采用了storyboard集成，如果需要调整功能，或者是做一些扩展，UI层面上建议在storyboardd上进行修改。
* 2.老张力求最精简的代码，以及最优化的性能，500行代码左右完成上述所有功能，注释也尽可能详细。所以如果你需要添加一些特殊的需求，建议先对源代码进行阅读，了解清楚思路，这样会事半功倍。
* 3.如果你跟我一样，也是个菜鸟，想了解整体的实现方法，那么请点后面的链接，文章会介绍如何实现屏幕的旋转，已经播放器实现的基本原理

## 适合对象
* 如果你是个拿来主义者，这就不要错过了。因为连代理方法我都没有设计，带上你的url 和 父控件view 视频立马就能放起来，还有什么比这个更愉快的？5个以内属性设置简单意思一下，也算有了API，所以拿去吧！

## 未来
* 播放器目前并未设置代理或者回调闭包，封装相对较死，如果start多了，我会尽可能完善播放器的API

## 联系我
* 如果有疑问或者发现了bug 请issue我。如果觉得还不错，请star, 多谢！
