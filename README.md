#enjoy it!

--------------
#DONE

1、支持XCode4 & XCode5 & iOS7

2、集成新浪微博SDK

3、发帖、转发、评论

4、微博征文布局和@某人、#话题#识别

#TODO

1、原图查看

2、表情显示

--------------

#OpenSinaMBlog
--------------

基于轻量级iOS开发框架[nimbus](https://github.com/jverkoey/nimbus)，

网络层采用AFNetworking，在此基础上进行二次构建，可以简单、便捷地处理和显示列表数据，

通过新浪微博授权后的首页为例子，介绍框架的使用，通过开源分享，跟大家一起技术交流。

由于新浪微博的api接口阉割太多，所以这个开源客户端主要分享的技术点如下：

1、tableView列表的数据获取和显示

2、类似官方客户端列表中的富文本的布局和关键字的识别和交互

3、发布微博、拍照及地理位置获取

--------------
项目clone到本地后

1、更新submodule：

   git submodule init 
   
   git submodule update
   
   注：如需要添加其他的submodule

       git submodule add https://github.com/jverkoey/nimbus.git vendor/nimbus

2、使用[CocoaPods](http://cocoapods.org)的命令安装其他依赖库：
   
   pod install
   
   注：如需要添加其他依赖库，请修改Podfile

#ERROR解决方法

--------------
    1、若出现这个问题：'vendor/SDURLCache' already exists in the index

      git rm --cached vendor/SDURLCache

    2、若出现这个问题：fatal: not removing 'vendor/nimbus' recursively without -r
    
      git rm -r --cached vendor/SDURLCache

    3、若出现这个问题：diff: /../Podfile.lock: No such file or directory 
    diff: /Manifest.lock: No such file or directory 
    error: The sandbox is not in sync with the Podfile.lock. Run 'pod install' or update your CocoaPods installation.

      pod install