# yilia-theme-dracula

![](https://img.shields.io/badge/hexo-3.7.1-blue)
![](https://img.shields.io/badge/yilia-4.0.0-blue)
![](https://img.shields.io/badge/IE-8+-red)

[中文文档](./README_CN.md)

A dracula-like color scheme originated from the hexo theme [yilia](https://github.com/litten/hexo-theme-yilia), inspired by [Dracula](https://draculatheme.com/).

See [my blog](https://natsunoyoru97.github.io/) to look how it works.

I want to build plugins(not only color scheme) rather than a theme. It's up to you to decide which files you want to import, and it's easy to uninstall any of these plugins if you don't need it anymore. It doesn't cause any side-effect.

# Get Started

Get a dracula theme in your yilia blog is easy. 

1. Just copy the ``dracula.scss`` file and paste it to the ``source-src/css`` folder in your yilia folder.

```shell
cp dracula.scss <your-path>/blog/theme/yilia/source-src/css
```

2. Open the ``main.scss`` file in the ``css`` folder, and add one line in the last of the file:

```scss
@import "./dracula";
```

Remind to copy ``tooltip.svg`` in the ``img`` as well, and paste it to the ``img`` folder in the ``source-src`` file of your yilia theme.

3. Compile with webpack in your ``yilia`` folder:

```shell
npx webpack
```


4. Regenerate your blog content in your ``blog`` folder with:

```shell
hexo clean && hexo g
```

# TODO

- **enable configuration from yaml(the .yml file)**
- **reconstruct the code if I have time cuz it's messy**
- install script in one-click
- do more tests
- draculafy the smart menu
- find a better way to display content
- customized social icons (if you would like to)! 
- the file tree
- maybe some animations
- fix other minor bugs
