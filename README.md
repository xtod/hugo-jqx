# Hugo jqx theme

### 一款简洁如纸的Hugo主题

[示例站点](https://0x8.net)

![Screenshot](https://raw.githubusercontent.com/xtod/hugo-jqx/refs/heads/main/images/screenshot.png)

## 特点

- 干净简约的设计
- 轻量且适合移动设备
- 零初始配置
- 简单的博客和分类
- 核心功能无需JavaScript
- 暗黑模式

## 试用示例

```sh
hugo new site example
cd example\themes
git clone https://github.com/xtod/hugo-jqx.git jqx
cd ..
hugo server --minify
```

## 配置文件

```toml
baseURL = 'https://example.org/'
title = 'jqx'
theme = 'jqx'
paginate = 5

languageCode = 'zh-cn'       
defaultContentLanguage = 'zh-cn'
locale = 'zh-cn'               

[params]
    mainSections = ["post"]
    description = "description of site"
    featuredImage = true                                     

[[menu.main]]
    name = "Home"
    url = "/"
    weight = 1

[[menu.main]]
    name = "Tags"
    url = "/tags/"
    weight = 2

[markup]
    [markup.goldmark]
        [markup.goldmark.renderer]
            unsafe = true

[taxonomies]
    tag = "tags"
    category = "categories"
    series = "series"          

[outputs]
    home = ["HTML", "RSS"]
    section = ["HTML", "RSS"]
    taxonomy = ["HTML", "RSS"]
    term = ["HTML", "RSS"]

[params.seo]
    enableRobots = true

[minify]
    disableXML = false  
    minifyOutput = true
```