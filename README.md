# Empty

[测试跳转](./测试/test.md)

## 跳转链接



> 在大部分常见 markdown 中，例如黑曜石、github、 ipynb 中，`[](#)` 的跳转圆括号里面空格必须为 “-”，或者使用 `html` 标签跳转。





在 github markdown 和 ipynb 中：（跳转链接及可跳转到的锚点）

```
[jump-1](#mark-1)
	# mark-1
	<a id="mark-1"></a>
	
<a href="#mark 1">mark 1</a>
	<a id="mark 1"></a>
	
<a href="#mark-1">mark 1</a>
	<a id="mark-1"></a>
```



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







