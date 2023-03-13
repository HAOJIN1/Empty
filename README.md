# Empty

[测试相对路径的文件跳转](./测试/test.md) 

对 GitHub 的 md 进行测试：

[测试# 不带空格目录跳转](#跳转锚点-不加空格版) 

[测试# 有空格目录跳转](#跳转锚点-有空格版) 



> 根据测试、GitHub 可以通过相对路径跳转，并且 GitHub 可以根据上面两个测试跳转。

通过测试，在 GitHub 中的 `ipynb` 文件的 `md` 跳转是报错的，可知 GitHub 并不支持 `ipynb` 文件的 `md` 语法跳转。

## 跳转链接

2023年3月13日14:37:37

经过测试发现，在 vscode 中操作 ipynb 文件目录跳转时

```
[First](#First)
	## First
	## first
```

英文目录可正常跳转，而中文目录无法正常跳转，

但是可使用

```
<a href="#目录一">目录一</a>
	# 目录一
<a href="#1.-目录一">目录一</a>
	# 1. 目录一
```

跳转，该跳转兼容 vscode 的 ipynb 和 Jupyter notebook 的 ipynb，相对于为全文中文标题添加 html 锚点是一个更好的选择。

在 vscode 跳转使用 html 的 a 标签作为目录时，只能使用小写字母，并且不能使用半角标点的句号，空格需要短横线代替，特殊标点则无法使用。



> 在大部分常见 markdown 中，例如 `Obsidain、GitHub、 Jupyter` 中，`[](#)` 的跳转圆括号里面空格必须为 “-”，或者使用 `html` 标签跳转，而 Typora 可以兼容空格。



在 `github markdown` 和 `ipynb` 中：（跳转链接及可跳转到的锚点）

```
[jump-1](#mark-1)
	# mark-1
	<a id="mark-1"></a>
	
<a href="#mark 1">mark 1</a>
	<a id="mark 1"></a>
	
<a href="#mark-1">mark 1</a>
	<a id="mark-1"></a>
```

> 根据测试可知，在常规 md 类型文档使用 md 格式时，带空格的标题需要在跳转链接的空格转为 "-" 才能识别。



在 `typora` 中：

```
[jump-1](#mark-1)
	# mark 1
	# mark-1
	<a id="mark-1"></a>
	
[jump 1](#mark 1)
	# mark 1
    # mark-1
    <a id="mark 1"></a>
    
<a href="#mark 1">mark 1</a>
	<a id="mark 1"></a>
	
<a href="#mark-1">mark 1</a>
	<a id="mark-1"></a>
```

> 而 `Typora` 对空格识别添加了支持，不需要转空格为 "-"。



以下是为了在基于 GitHub 的页面进行测试的内容



### 跳转锚点-不加空格版

>锚点内容：
>
>### 跳转锚点-不加空格版



填充文字

填充文字

填充文字

填充文字

填充文字

填充文字

填充文字

填充文字

填充文字

填充文字



### 跳转锚点 有空格版

> 锚点内容：
>
> ### 跳转锚点 有空格版





填充文字

填充文字

填充文字

填充文字

填充文字

填充文字

填充文字

填充文字

填充文字

填充文字
