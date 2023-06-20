---
title: "About"
date: 2023-05-18T16:19:31+08:00
# 详细配置
# menu: 
#   main: 
#       pre: <i><></i>
#       name: 关于
#   footer:
#       name: About

# 简单添加
# menu:
#   - main
#   - footer

menu: [main, footer]
draft: false
---

## this is about page
它们帮助内容作者将对网页或section的更改，本地化到磁盘上的特定文件夹。 页面bundles主要有两种类型: leaf bundle和branch bundle。 除此之外，我们还有不太常用的headless bundles。

## 测试列表{#test-list}
- 阿迪力风景
- 阿道夫据了解
- 撒的老骥伏枥
### 三级标题
1. 有序列表
2. 阿斯顿发价
3. 阿斯顿了房间

> 这里是引用的部分


```html {linenos=table,hl_lines=[3,"5-6"],linenostart=199}
<meta charset="UTF-8">
<!-- moment -->
<meta http-equiv="X-UA-Compatible" content="IE=edge">
<meta name="viewport" content="width=device-width, initial-scale=1.0"><meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>{{ .Title }}</title>
```

```bash {linenos=false}
hugo new theme <theme-name>
```

```java {linenos=false}
public class main {
  int a;
  String str;
}
```


{{< highlight java >}}
public class main {
  int a;
  String str;
}
{{< /highlight >}}

{{< highlight go-html-template >}}
{{ range .Pages }}
  <h2><a href="{{ .RelPermalink }}">{{ .LinkTitle }}</a></h2>
{{ end }}
{{< /highlight >}}

```go-html-template
{{ range .Pages }}
  <h2><a href="{{ .RelPermalink }}">{{ .LinkTitle }}</a></h2>
{{ end }}
```

{{< highlight go "linenos=table,hl_lines=8 15-17,linenostart=199" >}}
// GetTitleFunc returns a func that can be used to transform a string to
// title case.
//
// The supported styles are
//
// - "Go" (strings.Title)
// - "AP" (see https://www.apstylebook.com/)
// - "Chicago" (see https://www.chicagomanualofstyle.org/home.html)
//
// If an unknown or empty style is provided, AP style is what you get.
func GetTitleFunc(style string) func(s string) string {
  switch strings.ToLower(style) {
  case "go":
    return strings.Title
  case "chicago":
    return transform.NewTitleConverter(transform.ChicagoStyle)
  default:
    return transform.NewTitleConverter(transform.APStyle)
  }
}
{{< / highlight >}}

{{</* myshortcode */>}}
