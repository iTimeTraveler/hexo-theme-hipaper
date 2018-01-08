# Hipaper

[![Gitter](https://camo.githubusercontent.com/079d8764b5eebffbb7158fb375df0959029ab2c3/68747470733a2f2f6261646765732e6769747465722e696d2f6865786f2d7468656d652d696e6469676f2f4c6f6262792e737667)](https://gitter.im/hexo-theme-hiker/Lobby?utm_source=share-link&utm_medium=link&utm_campaign=share-link)             [![Build Status](https://travis-ci.org/iTimeTraveler/hexo-theme-hipaper.svg?branch=master)](https://travis-ci.org/iTimeTraveler/hexo-theme-hipaper)		[![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/iTimeTraveler/hexo-theme-hipaper/blob/master/LICENSE)


**A fashional newspaper, blog theme for Hexo**. 

- [**☞ Preview Demo**](https://itimetraveler.github.io/hexo-theme-hipaper/) | [**查看中文使用文档**](https://github.com/iTimeTraveler/hexo-theme-hipaper/blob/master/README.cn.md)


![](https://raw.githubusercontent.com/iTimeTraveler/iTimeTraveler.github.io/master/gallery/hipaper-demo-screen.png)

![](https://raw.githubusercontent.com/iTimeTraveler/hexo-theme-hipaper/master/source/preview/mobile-preview.png)

![](https://raw.githubusercontent.com/iTimeTraveler/hexo-theme-hipaper/master/source/preview/hipaper-preview.png)


<!--more-->

## Installation

  1. Get it from GitHub

 ```shell
 $ git clone https://github.com/iTimeTraveler/hexo-theme-hipaper.git themes/hipaper
 ```
  2. Enable

 Modify `theme` setting in `_config.yml` to `hipaper`.
 ```
 # Extensions
 ## Plugins: http://hexo.io/plugins/
 ## Themes: http://hexo.io/themes/
 theme: hipaper
 ```
  3. Update

 ```shell
 $ cd themes/hipaper
 $ git pull
 ```



## Features


### Logo: Image or Text

You can set a image as your logo instead of original text title. Like this:

![](https://raw.githubusercontent.com/iTimeTraveler/hexo-theme-hipaper/master/source/preview/logo-preview.jpg)

just enable `avatar` field in hipaper/_config.yml.

```yml
# Put your avatar.jpg into `hexo-site/themes/hipaper/source/` directory.
# url is target link (E.g. `url: https://hexo.io/logo.svg` or `url: css/images/mylogo.jpg`)
avatar: 
  enable: true
  width: 124
  height: 124
  bottom: 10
  url: https://hexo.io/logo.svg
```


### Code Highlight

Hipaper use [Tomorrow Theme](https://github.com/chriskempson/tomorrow-theme) for your code block. We have six options in total: `default`, `normal`, `night`, `night blue`, `night bright`, `night eighties`

![code `default` theme Preview](https://raw.githubusercontent.com/iTimeTraveler/hexo-theme-hipaper/master/source/preview/code-theme-default.png)

Above preview picture is default theme. the image below show other five Highlight themes.

![code themes](https://raw.githubusercontent.com/iTimeTraveler/hexo-theme-hipaper/master/source/preview/code-theme.jpg?raw=true)

Modify `highlight_theme` in hipaper/_config.yml.

```yml
# Code Highlight theme
# Available value:
#    default | normal | night | night eighties | night blue | night bright
# https://github.com/chriskempson/tomorrow-theme
highlight_theme: default
```



### Sidebar

You can put your sidebar in left side, right side or bottom of your site by editing `sidebar` setting.
Hipaper provides 7 built-in widgets:

- search
- social
- recent_posts
- category
- tag
- tagcloud
- archive

All of them are enabled by default. You can edit them in `widget` setting.


### Search

Hipaper use `Insight Search` to help you search anything inside your site without any third-party plugin.

![](https://raw.githubusercontent.com/iTimeTraveler/hexo-theme-hipaper/master/source/preview/search-preview.png)

```yml
# Search
search:
    insight: true # you need to install `hexo-generator-json-content` before using Insight Search
    swiftype: # enter swiftype install key here
    baidu: false # you need to disable other search engines to use Baidu search, options: true, false
```

> Attention: You need to install `hexo-generator-json-content` before using Insight Search.

```bash
$ npm install -S hexo-generator-json-content
```


### Fancybox

Hipaper uses [Fancybox] to showcase your photos. You can use Markdown syntax or fancybox tag plugin to add your photos.

```
![img caption](img url)

{% fancybox img_url [img_thumbnail] [img_caption] %}
```

### Comment support

Hipaper has native support for DuoShuo & Disqus comment systems. Modify the following snippets to Hipaper `hipaper/_config.yml`:

```yml
# comment ShortName, you can choose only ONE to display.
duoshuo_shortname: iTimeTraveler
disqus_shortname: 
```



## Browser support

![](https://raw.githubusercontent.com/iTimeTraveler/hexo-theme-hipaper/master/source/preview/browser-support.png?raw=true)



## Contributing

All kinds of contributions (enhancements, new features, documentation & code improvements, issues & bugs reporting) are welcome.

Looking forward to your pull request.

> Special thanks to ATHEMES, who designed the original theme [FASHIONISTA for Wordpress](http://athemes.com/theme/fashionista/).


## License

Hipaper is under the MIT license. See the [LICENSE](https://github.com/iTimeTraveler/hexo-theme-hipaper/blob/master/LICENSE) file for details.


[Hexo]: https://hexo.io/
[Fancybox]: http://fancyapps.com/fancybox/
[Font Awesome]: http://fontawesome.io/
