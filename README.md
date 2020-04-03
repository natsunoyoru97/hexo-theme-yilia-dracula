# yilia-theme-dracula

A dracula-like theme originated from the hexo theme yilia, inspired by [Dracula](https://draculatheme.com/).

See [my blog](https://natsunoyoru97.github.io/) to look how it works.

# Get Started

Get a dracula theme in your yilia blog is easy. 

1. Just copy the ``dracula.scss`` file and paste it to the ``source-src/css`` folder in your yilia folder.

2. Open the ``main.scss`` file, and add one line in the last of the file:

```scss
@import "./dracula";
```

3. Compile with webpack and regenerate your blog content.

# TODO

- **enable configuration from yaml(the .yml file)**
- do more tests
- draculafy the smart menu
- fix the bug: the border around the avatar is still white in mobiles
- fix the bug: searching in yilia is not working
- customized social icons (if you would like to)! 
- maybe some animations
- fix other minor bugs
