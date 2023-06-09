---
tags:
    - Markdown
    # - Tutorial
---

# markdown教程


## 1. 标题
markdown同HTML一样，支持六个等级标题。有两种标记方式:

### 1.1 #标记
```markdown
# 一级标题
## 二级标题
### 三级标题
#### 四级标题
##### 五级标题
###### 六级标题
```

### 1.2 =和-标记
```markdown
我是一级标题
===

我是二级标题
---
```

```
需要注意使用=和-表示一级和二级标题时,标题内容需要与之前的内容之间插入至少一个空行。
```

## 2. 段落格式

### 2.1 换行

换行直接在段落尾部回车即可，如果想在段落之间插入空行使段落分布更清晰，可以插入一个以上的空行。

### 2.2 强调

Markdown支持以下三种强调方式:

1. 斜体
   标记格式如下:
    ```
    *斜体*

    _斜体_
    ```
    效果如下:

    *斜体*

    _斜体_

2. 粗体
    标记格式如下:
    ```
    **斜体**

    __斜体__
    ```
    效果如下:

    **斜体**

    __斜体__

3. 粗斜体
    标记格式如下:
    ```
    ***斜体***

    ___斜体___
    ```
    效果如下:

    ***斜体***

    ___斜体___
    
### 2.3 分割线

你可以在一行中用三个以上的星号、减号、底线来建立一个分隔线，行内不能有其他东西。你也可以在星号或是减号中间插入空格。下面每种写法都可以建立分隔线:

```
***

* * *

*****

- - -

-----

___
```

效果如下:

***

* * *

*****

- - -

-----

___

### 2.4 删除线

如果段落上的文字要添加删除线，只需要在文字的两端加上两个波浪线 ~~ 即可，实例如下:

```
~~这是一段要删除的文字~~
```

效果如下:

<del>这是一段要删除的文字</del>

PS: mkdocs对于Markdown的删除线功能可能不支持,个人使用时没法实现,可以使用HTML的```<del>```标签代替使用。

### 2.5 下划线

下划线可以通过 HTML 的 ```<u>```标签来实现:

```
<u>带下划线文本</u>
```

效果如下:

<u>带下划线文本</u>

### 2.6 脚注

脚注是对文本的补充说明。

Markdown 脚注的格式如下:

```
[^要注明的文本]
```
使用时示例如下:

```
创建脚注格式类似这样 [^name1]。

[^name1]: 我是脚注
```

创建脚注格式类似这样 [^name1]。

[^name1]: 我是脚注

PS: mkdocs对于脚注功能支持,需要使用拓展功能。

## 3. 列表

Markdown 支持有序列表和无序列表。

### 3.1 无序列表

无序列表使用星号`*`、加号`+`或是减号`-`作为列表标记，这些标记后面要添加一个空格，然后再填写内容:

```
* 第一项
* 第二项
* 第三项

+ 第一项
+ 第二项
+ 第三项

- 第一项
- 第二项
- 第三项
```

效果如下:

* 第一项
* 第二项
* 第三项

+ 第一项
+ 第二项
+ 第三项

- 第一项
- 第二项
- 第三项

### 3.2 有序列表

有序列表使用数字并加上`.`号来表示，如:

```

```

### 3.3 列表嵌套

## 4. 区块

## 5. 代码

## 6. 链接

## 7.图片

## 8. 表格

## 9. 其他

