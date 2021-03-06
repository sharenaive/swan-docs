---
title: 编译工具历史更新日志
header: develop
nav: devtools
sidebar: uplog_compile
---

## 2.16版本更新日志

|版本号|更新内容|
|----|----|
|v2.16.17|**Bugfixes**<p>**·**web编译 修复filter和引用的swan文件不在一个目录下找不到资源的问题；<p>**·**修复css文件中@keyframes中的from to选择器动画不生效的问题。|
|v2.16.15|**Change**<p>**·**css文件中的html、body选择器将会被编译为swan-html、swan-body，从而在渲染时无效；<p>**·**project.swan.json 文件的改动将不会触发编译。|
|v2.16.14|**Bugfixes**<p>修复因app.json语法错误，而导致点击编译按钮无反应的bug。|
|v2.16.13|**Bugfixes**<p>修复 json 改动 watch 失效 bug 。|
|v2.16.12|**Bugfixes**<p>**·**web编译 app.css中样式前加.web-swan-app加权重；<p>**·**web编译 自定义组件css中给标签样式前加自定义标签，限制css有效域。|
|v2.16.11|**Bugfixes**<p>修复2.16.09引入web化编译参数错误bug。|
|v2.16.09|**New**<p>预览发布性能优化。|
|v2.16.08|**Bugfixes**<p>修复自定义组件css中@keyframes中rpx的转换无效bug。|
|v2.16.07|**Bugfixes**<p>**·**自定义组件css加载策略调整;<p>**·**自定义组件支持使用图标字体。|
|v2.16.05|**Bugfixes**<p>修正合并代码造成的run.js里工具方法名错误。|
|v2.16.04|**Bugfixes**<p>swan编译 自定义组件css中!import的兼容修复。|
|v2.16.03|**Bugfixes**<p>swan编译 自定义组件css中@charset, 以及样式声明中!import吞掉的bug修改。|
|v2.16.02|**Bugfixes**<p>web编译 修复window计算页面scope不同的问题。|
|v2.16.01|**Change**<p>分包中自定义组件page化的处理。|
|v2.16.00|**Change**<p>自定义组件优化重构。|

## 2.15版本更新日志

|版本号|更新内容|
|----|----|
|v2.15.07|**Change**<p>**·**web编译 manifest.json和白屏检测需要的html写进内存，不走fs；<p>**·**web编译 若有ext.json文件，copy进产出，支持tp；<p>**·**web编译 json文件内容提取后不置空module。|
|v2.15.06|**Change**<p>web编译 限制page的css中html、body的样式不在全局生效。|
|v2.15.04|**Change**<p>恢复merge分支丢掉的影响编译性能的代码。|
|v2.15.02|**Change**<p>web框架代码拆分一期，兼容新老web化白屏检测。|
|v2.15.01|**Change**<p>从磁盘缓存拿编译结果的增加打点字段isCache。|
|v2.15.00|**Change**<p>编译版本号第二位加1。|

## 2.13版本更新日志

|版本号|更新内容|
|----|----|
|v2.13.44|**Bugfix**<p>windows平台自定义组件没有require的bug修改。|
|v2.13.42|**Bugfix**<p>磁盘缓存时，当修改page页面的json文件时，没有在swan文件的依赖分析图中加上json的依赖，导致编译产出异常。|
|v2.13.40|**Change**<p>增加编译的磁盘缓存。|
|v2.13.38|**Bugfix**<p>修复web 编译fitler中不支持标签的问题。|
|v2.13.36|**Change**<p>**·** 自定义组件对应的css文件是否存在不会进行强校验；<p>**·**全部异步错误信息捕获。|
|v2.13.35|**Change**<p>**·**编译增加文件大小打点字段；<p>**·**web 编译自定义组件配置错误在非watch模式下主动退出；<p>**·**删除产出 app.js 和 filter 中增加 Function 字段。|
|v2.13.34|**Change**<p>自定义组件路径错误、css@import的资源不存在时，在非watch模式下退出。|
|v2.13.33|**Bugfix**<p>修复 replace.js 中写文件事件监听错误导致copy文件缺损。|
|v2.13.32|**Bugfix**<p>修复产出 manifest.json 文件在 windows 下路径错误。|
|v2.13.30|**Bugfix**<p>web 编译分包 css 增加 scope。|
|v2.13.29|**Change**<p>web 编译增加文件路径替换 。|
|v2.13.28|**Bugfixes**<p>**·**web 编译修复自定义 template 内引用 template 路径查找错误 。|
|v2.13.27|**Bugfixes**<p>**·**web 编译兼容修复用户 page 中配置文件为空编译退出，对齐 swan 编译；<p>**·**web 编译兼容用户自定义组件路径配置错误编译退出问题，对齐 swan 编译。|
|v2.13.26|**Bugfixes**<p>swan 编译更新静态资源文件名hash值生成规则。|
|v2.13.24|**Change**<p>非watch模式下json错误抛错。|
|v2.13.23|**New**<p>增加音频文件的处理。|
|v2.13.22|**Bugfixes**<p>修复错误日志在watch模式下误报。|
|v2.13.21|**Bugfixes**<p>template标签中filter定义的js不经过babel转换的bug修改。|
|v2.13.20|**Bugfixes**<p>媒体资源在windows平台无编译的bug修改。|
|v2.13.19|**New**<p>**·**增加对视频的处理；<p>**·**web 编译处理非 page、component json 文件。|
|v2.13.17|**Change**<p>编译日志优化。|
|v2.13.16|**BugFix**<p>**·**修复编译进程主动退出未打印错误；<p>**·**去除 web 编译 css 中背景图片限制；<p>**·**产出 app.js 和 filter 中增加 Function 字段|
|v2.13.15|**BugFix**<p>去除 unhandledRejection 事件。|
|v2.13.14|**BugFix**<p>去除 Function。|
|v2.13.13|**New**<p>web 编译增加自定义组件 page 化。<p>**BugFix**<p>web 编译修复 watch 模式下用户代码异常会导致进程退出问题。|
|v2.13.12|**New**<p>编译监听报错后主动退出。|
|v2.13.11|**BugFix**<p>**·**在window中，css文件url里路径格式化的bug修复；<p>**·**编译错误上报优化windows下路径转换问题。|
|v2.13.10|**BugFix**<p>对绝对路径判断的bug修复。|
|v2.13.9|**BugFix**<p>规避对src属性中变量的校验。|
|v2.13.8|**Change**<p>资源文件找不到时报error。|
|v2.13.7|**BugFix**<p>**·**web 编译修复 filter 多次引用解析错误；<p>**·**web 编译修复 template 中引入图片路径转换错误；<p>**·**css中找不到图片时，warning级别改为error级别。|
|v2.13.6|**BugFix**<p>**·**css文件中@import资源中使用url引入的资源路径解析错误的bug修复；<p>**·**watch触发两次end的bug修复。|
|v2.13.5|**BugFix**<p>**·**template文件没有加到依赖分析里，不触发watch的bug修复；<p>**·**项目目录下无swan文件退出编译进程的bug修复。|
|v2.13.4|**BugFix**<p>web 编译修复rpx小数替换错误修复。|
|v2.13.3|**BugFix**<p>在模板中filter有前缀时会将前缀置为空的bug修改。|
|v2.13.2|**Change**<p>更新打点字段。<p>**BugFix**<p>低版本core时，自定义组件循环引用编译直接打断。|
|v2.13.1|**Change**<p>编译优化。<p>**BugFix**<p>在属性中用filter时，会导致模板闭合错误的bug修改。|
|v2.13.0|**Change**<p>**·**编译优化;<p>**·**当有普通分包时，appJs拆分相关资源不产出。<p>**BugFix**<p>**·**自定义组件中标签src属性为相对路径，资源路径处理错误的bug修复；<p>**·**rpx转换bug修复。|


## 2.12版本更新日志

|版本号|更新内容|
|----|----|
|v2.12.18|**BugFix**<p>web 编译自定义组件模板未找到修复。|
|v2.12.17|**BugFix**<p>swab-web 依赖升级。|
|v2.12.16|**BugFix**<p>**·**web 编译兼容 json 文件为空；<p>**·**swan 编译自定义组件样式增加前缀 swan-组件名。|
|v2.12.15|**BugFix**<p>编译时长等相关信息上报。|
|v2.12.14|**New**<p>**·**自定义组件key值全部转为小写；<p>**·**自定义组件css增加swan前缀；<p>**·**web 编译跳转事件增加swan-spider-tap class。<p>**BugFix**<p>修复web编译自定义组件深目录导致获取tpl错误。|
|v2.12.13|**New**<p>**·**增加appJs拆分逻辑；<p>**·**对于project.swan.json不监听文件更改。|
|v2.12.12|**New**<p>增加第三方组件编译。|
|v2.12.11|**BugFix**<p>windows下路径转换问题。|
|v2.12.10|**BugFix**<p>分包主包依赖相同资源时，多次初始化的bug修复。|
|v2.12.9|**BugFix**<p>模板中$符的转换。|
|v2.12.7|**New**<p>自定义组件、模板中可使用filter。|
|v2.12.6|**New**<p>自定义组件Page化。|
|v2.12.5|**BugFix**<p>修复 web 编译中 filter 解析错误。|
|v2.12.4|**BugFix**<p>解决当图标格式为svg时，没有编译到产出中的问题修改。|
|v2.12.3|**New**<p>web 编译自定义组件策略变更，模板 class 交由框架处理前缀。|
|v2.12.2|**BugFix**<p>**·**增加用户css中url限制超过700条后报错；<p>**·**修复web编译css图片路径错误。|
|v2.12.1|**BugFix**<p>自定义组件中支持filter功能在低版本的兼容。|
|v2.12.0|**BugFix**<p>自定义组件中支持filter功能。|


## 2.11版本更新日志

|版本号|更新内容|
|----|----|
|v2.11.9|**BugFix**<p>**·**去除用户css expression 表达式；<p>**·**自定义组件循环引用的支持；<p>**·**自定义组件多层嵌套无效的问题修改。|
|v2.11.8|**BugFix**<p>更新 postcss-loader 版本至 3.0，解决与 cssnano 版本冲突导致 css 压缩在 windows 上运行报错问题。|
|v2.11.7|**BugFix**<p>修复 web 编译 windows 自定义组件解析失败问题。|
|v2.11.6|**BugFix**<p>**·**web 编译修复 windows 遗留路径问题；<p>**·** 修复 web 编译 swan 模板中 md5 和 css 中 md5生成不等问题。|
|v2.11.5|**BugFix**<p>自定义组件css字体图标不显示的问题修改。|
|v2.11.4|**BugFix**<p>自定义组件css图片资源路径为线上资源时路劲错误的问题修改。|
|v2.11.2|**BugFix**<p>自定义组件css图片资源路径为base64时的问题修改。|
|v2.11.1|**BugFix**<p>filter内联不生效的问题修复。|


## 2.10版本更新日志

|版本号|更新内容|
|----|----|
|v2.10.9|**BugFix**<p>**·**自定义组件css前缀的兼容处理；<p>**·**自定义组件资源路径的处理；<p>**·**自定义组件css支持iconfont。|
|v2.10.8|**BugFix**<p>web 编译修复 swan 模板中单双引号导致模板解析的问题。|
|v2.10.7|**BugFix**<p>**·**web 编译修复 windows 遗留路径问题；<p>**·** 修复 web 编译 swan 模板中 md5 和 css 中 md5生成不等问题。|
|v2.10.6|**BugFix**<p>web 编译修复 windows 路径问题。|
|v2.10.4|**BugFix**<p>去除工作目录下.babelrc文件对编译的影响。|
|v2.10.3|**BugFix**<p>自定义组件class属性值去除组件名前缀。|
|v2.10.2|**New**<p>增加web化的编译。|
|v2.10.1|**BugFix**<p>windows下路径无效的问题修复。|
|v2.10.0|**New**<p>**·**自定义组件中支持使用import、template；<p>**·**自定义组件css中可以使用@import语法。<p>**BugFix**<p>**·**自定义组件循环引用导致编译失败的问题；<p>**·**无用json文件也会被解析，从而导致编译失败；<p>**·**预览时，偶发的编译失败问题。|


## 2.0版本更新日志

|版本号|更新内容|
|----|----|
|v2.0.9|**BugFix**<p>解决图标字体无效的问题。|
|v2.0.8|**Change**<p>**·**css标签样式加swan-前缀的bug修改;<p>**·**事件绑定支持字符串加表达式的混合使用。<p>**BugFix**<p>解决十六进制颜色值简写无效的问题。|
|v2.0.6|**New**<p>**·** 新增依赖分析编译模式;<p>**·** 增量编译，编译模式分为普通编译模式及依赖分析编译模式。<p>**BugFix**<p>**·** 解决单引号包含双引号，页面空白的问题。|
|v2.0.4|**BugFix**<p>**·** 修复动画失效的问题；<p> **·** 修复因引入filter功能从而影响页面渲染的问题。|
|v2.0.0|**BugFix**<p> **·** 自定义组件引用js，报模块未定义的bug。<p> **·** 模板命名问题。|
