# yilia-theme-dracula

![](https://img.shields.io/badge/hexo-3.7.1-blue)
![](https://img.shields.io/badge/yilia-4.0.0-blue)
![](https://img.shields.io/badge/IE-8+-red)

基于hexo主题[yilia](https://github.com/litten/hexo-theme-yilia)的配色方案，灵感源于[Dracula](https://draculatheme.com/)，因为很喜欢所以干脆自己动手做了一个。

[我的博客](https://natsunoyoru97.github.io/)现在就在用这个主题，在用之前可以先看看效果。有什么bug或者建议欢迎提出issue，当然也欢迎pull request。

另外这个仓库只是基于yilia的插件集合而不是另外一款主题。不同的功能会写在不同的文件里，供大家定制化自己的博客。虽然主要留作给玩家折腾用，但以后有时间也会写针对懒人的一键安装脚本（当然也支持一键删除），想一键集成也是可以的。

# 使用方法

目前在yilia博客上应用该主题有四步：

1. 复制``dracula.scss``到你yilia主题下的``source-src/css`` 文件夹中：

```shell
cp dracula.scss <your-path>/blog/theme/yilia/source-src/css
```

2. 在``css``文件夹中打开``main.scss``，在文件后面复制：

```scss
@import "./dracula";
```

还需要同时复制``img``文件夹下的``tooltip.svg``到yilia主题下``source-src``里的同名文件夹内，否则分享和目录的弹窗会有一部分仍然保持原来的颜色。

3. 在``yilia``文件夹下用webpack打包编译，重新生成你的博客：

```shell
npx webpack
```


4. 在``blog``文件夹下重新生成博客：

```shell
hexo clean && hexo g
```


# TODO

- **通过yaml自定义主题状态，当选择该主题时才加载主题文件**
- **重构代码**
- 针对懒人的一键安装脚本
- 进一步做测试
- 统一智能菜单与主题的风格
- 觉得yilia的目录显示很不方便，设法改进
- 添加自定义社交软件图标（虽然我的博客已经自定义了社交图标，但仓库的文件里**并不包含**这个功能，如果大家需要我再添加）
- 可能会做一些自定义动画，就符合dracula风格的那种
- 不同的功能会分成不同的文件写，dracula.scss只包括美化的内容，其它功能在别的文件里，大家可以只取自己想要的部分（日后会补充文件树）
- 修复其它小bug

# 须知

源主题[yilia](https://github.com/litten/hexo-theme-yilia)已经将近5年没更新代码了，而在这个期间hexo有些重大升级，所以更新hexo可能导致yilia
主题的一些样式和功能失效。我修好了其中一些bug，在我的个人博客上是能正常运作的。

修改过的yilia源文件都在``yilia``这个文件夹下面，可以随意取用并覆盖失效的原代码。