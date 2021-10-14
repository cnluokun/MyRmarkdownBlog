---
title: hugo-self-syntax
author: cnluokun
date: '2021-10-14'
slug: index.zh-cn
categories:
  - uncategoried
tags:
  - pull-quote
  - tabbed-codeblock
---

# 测试Hugo主题自带的一些syntax
## Tags plugins showcase
### 1. Alert Tag：测试Info/Succ/Warn/Danger标签
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
### 2. Tabbed code block: Tab测试
{{< tabbed-codeblock example  >}}
    <!-- tab js -->
        var test = 'test';
    <!-- endtab -->
    <!-- tab css -->
        .btn {
            color: red;
        }
    <!-- endtab -->
{{< /tabbed-codeblock >}}


突发奇想可不可以用`tabbed-codeblock`标签实现一般情况的Tab栏
{{< tabbed-codeblock >}}
    <!-- tab TAB1 -->
        此处文本代表TAB1的内容
        ```cpp
        cout<<"Hello World"<<endl;
        ```
    <!-- endtab -->
    <!-- tab TAB2 -->
        此处文本代表TAB2的内容
        ```bash
        sudo apt-get install npm
        ```
    <!-- endtab -->
{{< /tabbed-codeblock >}}

### 3.Pull Quote:Quote内容环绕
Here's a more realistic example of how you might use a pull quote. When writing longform posts, I find it helpful to include pull quotes to help readers easily identify the topics covered in each section. Some prefer to break things up with lots of headings, and while this seems to be a trend it doesn't work so well for long form prose. It is important to note that pull quotes are merely visual in presentation and should not appear twice in the text. That is why it a CSS only technique for styling pull quotes is preferable. Octopress includes a handy pull quote plugin to make this easy for you.
{% pullquote left %}
Surround your paragraph with the pull quote tags. Then when you come to
the text you want to pull, {" surround it like this "} and that's all there is to it.
{% endpullquote %}