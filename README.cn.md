# Hipaper

[![Gitter](https://camo.githubusercontent.com/079d8764b5eebffbb7158fb375df0959029ab2c3/68747470733a2f2f6261646765732e6769747465722e696d2f6865786f2d7468656d652d696e6469676f2f4c6f6262792e737667)](https://gitter.im/hexo-theme-hiker/Lobby?utm_source=share-link&utm_medium=link&utm_campaign=share-link)             [![Build Status](https://travis-ci.org/iTimeTraveler/hexo-theme-hipaper.svg?branch=master)](https://travis-ci.org/iTimeTraveler/hexo-theme-hipaper)		[![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/iTimeTraveler/hexo-theme-hipaper/blob/master/LICENSE)


**A fashional newspaper, blog theme for Hexo**. [**☞ 点击预览**](https://itimetraveler.github.io/hexo-theme-hipaper/)  |  [**Hipaper问题交流**](https://gitter.im/hexo-theme-hiker/Lobby?utm_source=share-link&utm_medium=link&utm_campaign=share-link)


![](https://raw.githubusercontent.com/iTimeTraveler/iTimeTraveler.github.io/master/gallery/hipaper-demo-screen.png)

![](https://raw.githubusercontent.com/iTimeTraveler/hexo-theme-hipaper/master/source/preview/mobile-preview.png)

![](https://raw.githubusercontent.com/iTimeTraveler/hexo-theme-hipaper/master/source/preview/hipaper-preview.png)


<!--more-->

## 安装步骤

 1. 从Github上获取源码

 ```shell
 $ git clone https://github.com/iTimeTraveler/hexo-theme-hipaper.git themes/hipaper
 ```
 2. 启用主题

 把Hexo主目录下 `_config.yml` 文件中的`theme`字段改为 `hipaper`，如下：
 ```
 # Extensions
 ## Plugins: http://hexo.io/plugins/
 ## Themes: http://hexo.io/themes/
 theme: hipaper
 ```
 3. 更新到最新

 ```shell
 $ cd themes/hipaper
 $ git pull
 ```



## 特性


### 支持图片Logo

就像下面这样：

![](https://raw.githubusercontent.com/iTimeTraveler/hexo-theme-hipaper/master/source/preview/logo-preview.jpg)

只用在hipaper/_config.yml中设置 `avatar`字段的`eanble`为true，然后设置图片的`url`就好了。

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



### 代码高亮

Hipaper 使用 [Tomorrow Theme](https://github.com/chriskempson/tomorrow-theme) 作为代码主题. 共有以下六种选项: `default`, `normal`, `night`, `night blue`, `night bright`, `night eighties`

![code `default` theme Preview](https://raw.githubusercontent.com/iTimeTraveler/hexo-theme-hipaper/master/source/preview/code-theme-default.png)

默认高亮配色如上图， 另外的五种配色如下.

![code themes](https://raw.githubusercontent.com/iTimeTraveler/hexo-theme-hipaper/master/source/preview/code-theme.jpg?raw=true)

您可以在本主题的 hipaper/_config.yml 文件中更改 `highlight_theme` 字段.

```yml
# Code Highlight theme
# Available value:
#    default | normal | night | night eighties | night blue | night bright
# https://github.com/chriskempson/tomorrow-theme
highlight_theme: default
```



### 侧边栏

主题_config.yml文件中的 `sidebar` 字段可以设置为 `left`或`right`，用来控制侧边栏显示在页面左侧还是右侧。
Hipaper 拥有以下7种侧边栏组件:

- search （搜索框）
- social （社交网站链接）
- recent_posts （最新文章）
- category （分类）
- tag （标签）
- tagcloud （标签云）
- archive （归档栏）

以上组件在主题中均已默认启用.您可以在 `widget` 字段中设置显示哪些以及顺序。


### 站内搜索

Hipaper 使用 `Insight Search` 来帮助大家使用站内搜索.

![](https://raw.githubusercontent.com/iTimeTraveler/hexo-theme-hipaper/master/source/preview/search-preview.png)

```yml
# Search
search:
    insight: true # you need to install `hexo-generator-json-content` before using Insight Search
    swiftype: # enter swiftype install key here
    baidu: false # you need to disable other search engines to use Baidu search, options: true, false
```

> ！！注意: 使用搜索工具之前您必须使用 `hexo-generator-json-content` 来安装，在Hexo根目录下执行命令如下：

```bash
$ npm install -S hexo-generator-json-content
```


### Fancybox

Hipaper 使用 [Fancybox] 来提供文章图片预览.

```
![img caption](img url)

{% fancybox img_url [img_thumbnail] [img_caption] %}
```

### 评论功能

Hipaper 已完全支持原生的多说、 Disqus评论功能. 您可以在 `hipaper/_config.yml` 文件中更改以下字段:

```yml
# comment ShortName, you can choose only ONE to display.
duoshuo_shortname: iTimeTraveler
disqus_shortname:
```



## 支持的浏览器

![](https://raw.githubusercontent.com/iTimeTraveler/hexo-theme-hipaper/master/source/preview/browser-support.png?raw=true)



## 贡献

> 本主题源于Wordpress作者 ATHEMES, 原生主题点击查看 [FASHIONISTA for Wordpress](http://athemes.com/theme/fashionista/).

大家有各种问题和改进建议的，直接提issue或者评论，或者pull request都行。我会尽量抽时间和大家交流。刚接触Hexo不久，疏忽不足之处，还望大家海涵！


## License

Hipaper is under the MIT license. See the [LICENSE](https://github.com/iTimeTraveler/hexo-theme-hipaper/blob/master/LICENSE) file for details.


[Hexo]: https://hexo.io/
[Fancybox]: http://fancyapps.com/fancybox/
[Font Awesome]: http://fontawesome.io/
