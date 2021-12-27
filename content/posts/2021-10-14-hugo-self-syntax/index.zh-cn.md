---
title: "测试Hugo主题的syntax"
author: "cnluokun"
date: '2021-10-14'
output: pdf_document
coverImage: //d1u9biwaxjngwg.cloudfront.net/cover-image-showcase/city.jpg
coverMeta: in
metaAlignment: center
thumbnailImagePosition: left
autoThumbnailImage: yes
slug: index.zh-cn
---
This post is used to show how Tranquilpeak theme is configured for Hugo framework. Tranquilpeak theme is compatible with Hugo `v0.53`. See [docs](https://github.com/kakawait/hugo-tranquilpeak-theme/blob/master/docs/user.md#tags) for more information.
<!--more-->


## 1. Tags plugins showcase
### 1.1 Alert Tag：测试Info/Succ/Warn/Danger标签
{{<alert info>}}
此处文本测试Info标签使用效果。
此处文本测试Info标签使用效果。
{{</alert>}}

{{<alert success>}}
此处文本测试Succ标签使用效果。
此处文本测试Succ标签使用效果。
{{</alert>}}

{{<alert warning>}}
此处文本测试Warn标签使用效果。
此处文本测试Warn标签使用效果。
{{</alert>}}

{{<alert danger>}}
此处文本测试Danger标签使用效果。
此处文本测试Danger标签使用效果。
{{</alert>}}

### 1.4.折叠内容
{{%expand "EXPAND ME"%}}
Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod
tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam,
quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo
consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse
cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non
proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
{{% /expand%}}

### 1.5.Pull Quote:Quote内容环绕

Here's a more realistic example of how you might use a pull quote. When writing longform posts, I find it helpful to include pull quotes to help readers easily identify the topics covered in each section. Some prefer to break things up with lots of headings, and while this seems to be a trend it doesn't work so well for long form prose. 
{{< pullquote left >}}
It is important to note that pull quotes are merely visual in presentation and should not appear twice in the text.
{{< /pullquote >}} 
That is why it a CSS only technique for styling pull quotes is preferable. Octopress includes a handy pull quote plugin to make this easy for you.

