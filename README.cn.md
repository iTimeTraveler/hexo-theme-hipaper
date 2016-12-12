# Hipaper

**A fashional newspaper, blog theme for Hexo**. [**☞ 点击预览**](https://itimetraveler.github.io/hexo-theme-hipaper/)


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


### 代码高亮

Hipaper 使用 [Tomorrow Theme](https://github.com/chriskempson/tomorrow-theme) 作为代码主题. 共有一下六种选项: `default`, `normal`, `night`, `night blue`, `night bright`, `night eighties`

![code `default` theme Preview](https://raw.githubusercontent.com/iTimeTraveler/hexo-theme-hipaper/master/source/preview/code-theme-default.png)

默认如上图，其他五种主题如下.

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

主体中的 `sidebar` 字段可以设置为 `left`或`right`，用来控制侧边栏显示在页面左侧还是右侧。
Hipaper 拥有以下7种侧边栏组件:

- search （搜索框）
- social （社交网站链接）
- recent_posts （最新文章）
- category （分类）
- tag （标签）
- tagcloud （标签云）
- archive （归档栏）

以上默认主题中均已启用. 您可以在 `widget` 字段中设置显示哪些以及顺序。


### Search

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

Hipaper 使用 [Fancybox] 来展示文章图片预览.

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
