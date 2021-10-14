---
title: 测试一些hugo主题的syntax
author: cnluokun
date: '2021-10-14'
slug: index.zh-cn
categories:
  - uncategoried
tags:
  - pull-quote
  - tabbed-codeblock
---
![thumbnailPicture](https://media.istockphoto.com/photos/social-network-hologram-drawings-over-computer-on-the-desktop-top-picture-id1288509320?s=612x612)
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
### 1.2 Tabbed code block: Tab测试
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

### 1.3.Tabbed-View:选项卡效果
#### 1.3.1 hugo-dynamic-tabs外挂插件实现Tab栏效果

{{< tabs tabTotal="3" tabID="2" tabName1="Tab 1" tabName2="Tab 2" tabName3="Tab 3" >}}
{{< tab tabNum="1" >}}

**Tab 1 Content**
```python
print("Hello World!")
```
{{< /tab >}}
{{< tab tabNum="2" >}}

**Tab 2 Content**


{{< /tab >}}
{{< tab tabNum="3" >}}

**Tab 3 Content**

{{< /tab >}}
{{< /tabs >}}

#### 1.3.2  docsy主题的tapped-pane效果
{{< tabpane >}}
  {{< tabbed header="English" >}}
    Welcome!
  {{< /tabbed >}}
  {{< tabbed header="German" >}}
    Herzlich willkommen!
  {{< /tabbed >}}
  {{< tabbed header="Swahili" >}}
    Karibu sana!
  {{< /tabbed >}}
{{< /tabpane >}}

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
```
{% pullquote %}
Here's a more realistic example of how you might use a pull quote. When writing longform posts, I find it helpful to include pull quotes to help readers easily identify the topics covered in each section. Some prefer to break things up with lots of headings, and while this seems to be a trend it doesn't work so well for long form prose. {"It is important to note that pull quotes are merely visual in presentation and should not appear twice in the text."} That is why it a CSS only technique for styling pull quotes is preferable. Octopress includes a handy pull quote plugin to make this easy for you.
{% endpullquote %}
```