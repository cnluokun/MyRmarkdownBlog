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
{{<tabbed-codeblock TabbedCodeBlock>}}

    <!-- tab js -->
        var test = 'test';
    <!-- endtab -->
    
    <!-- tab css -->
        .btn {
            color: red;
        }
    <!-- endtab -->
    
    <!-- tab html -->
        <?xml version="1.0"?>
        <response value="ok" xml:lang="en">
          <text>Ok</text>
          <comment html_allowed="true"/>
          <ns1:description><![CDATA[
          CDATA is <not> magical.
          ]]></ns1:description>
          <a></a> <a/>
        </response>
        
        
        <!DOCTYPE html>
        <title>Title</title>
        
        <style>body {width: 500px;}</style>
        
        <script type="application/javascript">
          function $init() {return true;}
        </script>
        
        <body>
          <p checked class="title" id='title'>Title</p>
          <!-- here goes the rest of the page -->
        </body> 
    <!-- endtab -->
    
{{</tabbed-codeblock>}}

### 3.Hugo Dynamic Tabs
外挂插件实现Tab栏效果
{{< tabs tabTotal="3" tabID="1" tabName1="Tab 1" tabName2="Tab 2" tabName3="Tab 3" >}}
{{< tab tabNum="1" >}}

**Tab 1 Content**
```cpp
cout<<"hello world!"<<endl;
```
{{< /tab >}}
{{< tab tabNum="2" >}}

**Tab 2 Content**

{{< /tab >}}
{{< tab tabNum="3" >}}

**Tab 3 Content**

{{< /tab >}}
{{< /tabs >}}

### 3.Pull Quote:Quote内容环绕
Here's a more realistic example of how you might use a pull quote. When writing longform posts, I find it helpful to include pull quotes to help readers easily identify the topics covered in each section. Some prefer to break things up with lots of headings, and while this seems to be a trend it doesn't work so well for long form prose. It is important to note that pull quotes are merely visual in presentation and should not appear twice in the text. That is why it a CSS only technique for styling pull quotes is preferable. Octopress includes a handy pull quote plugin to make this easy for you.
{% pullquote left %}
Surround your paragraph with the pull quote tags. Then when you come to
the text you want to pull, {" surround it like this "} and that's all there is to it.
{% endpullquote %}