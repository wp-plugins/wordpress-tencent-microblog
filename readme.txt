=== wordpress-tencent-microblog ===
Contributors: HzlzH
Donate link: http://www.hzlzh.com/wordpress-tencent-microblog/
Tags: 腾讯微博,QQ,微博,腾讯,同步
Requires at least: 2.7
Tested up to: 3.0.1
Stable tag: 1.0.6

显示腾讯微博发言的插件，无需密码，安全可靠，采取缓存机制。利用民间API，支持1-10条发言输出。

== Description ==

显示腾讯微博发言的插件，无需密码，即可从 <a href="http://q.hzlzh.com/">民间API</a> 处获得消息，显示在wordpress侧边栏上，安全可靠。采用了缓存机制，可自定义刷新时间，不占用站点加载速度。可以在[外观]--[小工具]中调用，也可以在任意位置使用`<?php display_tencent('username=you-ID&number=5'); ?>` 调用。

== Installation ==

1. 上传 `wordpress-tencent-microblog`插件到 `/wp-content/plugins/` 目录
2. 在Wordpress后台控制面板"插件(Plugins)"菜单下激活"wordpress-tencent-microblog"
3. 在Wordpress后台控制面板"外观(Appearance)->小工具(Widgets)"下使用`腾讯微博`

== Frequently Asked Questions ==

= 我不想在侧边栏调用，而是在任意位置可以么？怎么做？ =

可以！需要激活插件后，在任意位置使用`<?php display_tencent('username=you-ID&number=5'); ?>`调用即可，只需要修改`you-ID` 为你的腾讯微博帐号，`5`是你想要展示的条数。

目前官方没有开放API，待开放时，我会第一时间更新。

= 有腾讯微博官方的API吗？ =

目前官方没有开放API，待开放时，我会第一时间更新。

= 如果我的HOST不支持copy()函数怎么办？ =

可以去除缓存功能，直接抓取API即可，参见 <a href="http://www.hzlzh.com/wordpress-tencent-microblog/">使用说明</a>

== Screenshots ==

1. 使用侧边栏[小工具]调用的效果
2. 后台截图

== Changelog ==

= V 1.0.5 =
*修改了几个重要的注释
*提供了WIN主机无法使用copy()函数的解决方案注释
*修改了一些细节

= V 1.0.3 =
*现在支持 1至10 条的发言调用
*修复了有实名认证的用户的显示错误BUG
*加入了 CSS 样式，预留自定义接口

= V 1.0.0  =
*在Wordpress中同步显示腾讯微博中的发言
*无需登录，采取民间API，安全可靠
*由于使用缓存，本插件目录需要有写入权限
*目前调取显示数量为1条，更多需要API的支持，尽在下一个版本

== Upgrade Notice ==

= V 1.0.6 =
为了减少API 被禁止的可能，使用新的API地址，http://q.hzlzh.com/wordpress/

= V 1.0.5 =
修改了几个重要的注释，提供了WIN主机无法使用copy()函数的解决方案注释

= 1.0.3 =
本版本已经完善了10条以内信息的完善，并且预留了CSS样式名

= 1.0.0 =
这个是第一个版本，由于API限制只能调用1发言
