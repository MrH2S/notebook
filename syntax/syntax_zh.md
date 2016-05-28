
# leanote Markdown 语法手册



## 1. 斜体和粗体



使用 * 和 ** 表示斜体和粗体。



----------



示例：



这是 *斜体*，这是 **粗体**。



## 2. 分级标题



使用 === 表示一级标题，使用 --- 表示二级标题。



示例：



```

这是一个一级标题

============================



这是一个二级标题

--------------------------------------------------



### 这是一个三级标题

```



你也可以选择在行首加井号表示不同级别的标题 (H1-H6)，例如：# H1, ## H2, ### H3，#### H4。



## 3. 外链接



使用 \[描述](链接地址) 为文字增加外链接。



示例：



这是去往 [本人博客](http://ghosertblog.github.com) 的链接。



## 4. 无序列表



使用 *，+，- 表示无序列表。



示例：



- 无序列表项 一

- 无序列表项 二

- 无序列表项 三



## 5. 有序列表



使用数字和点表示有序列表。



示例：



1. 有序列表项 一

2. 有序列表项 二

3. 有序列表项 三



## 6. 文字引用



使用 > 表示文字引用。



示例：



> 野火烧不尽，春风吹又生。



## 7. 行内代码块



使用 \`代码` 表示行内代码块。



示例：



让我们聊聊 `html`。



## 8. 代码块



使用 四个缩进空格 表示代码块。



示例：



这是一个代码块，此行左侧有四个不可见的空格。



## 9. 插入图像



使用 \!\[描述](图片链接地址) 插入图像。



示例：



![leanote](http://leanote.com/images/logo.png)



# Markdown 高阶语法手册



## 1. LaTeX 公式



$ 表示行内公式：



质能守恒方程可以用一个很简洁的方程式 $E=mc^2$ 来表达。



$$ 表示整行公式：



∑i=1nai=0∑i=1nai=0



f(x1,xx,…,xn)=x21+x22+⋯+x2nf(x1,xx,…,xn)=x12+x22+⋯+xn2



∑k=0j−1γˆkjzk∑k=0j−1γ^kjzk



访问 [MathJax](http://meta.math.stackexchange.com/questions/5020/mathjax-basic-tutorial-and-quick-reference) 参考更多使用方法。



# 2. 加强的代码块



支持四十一种编程语言的语法高亮的显示，行号显示。



非代码示例：



```

$ sudo apt-get install vim-gnome

```



Python 示例：



```python

@requires_authorization

def somefunc(param1='', param2=0):

'''A docstring'''

if param1 > param2: # interesting

print 'Greater'

return (param2 - param1 + 1) or None



class SomeClass:

pass



>>> message = '''interpreter

... prompt'''

```



JavaScript 示例：



``` javascript

/**

* nth element in the fibonacci series.

* @param n >= 0

* @return the nth element, >= 0.

*/

function fib(n) {

var a = 1, b = 1;

var tmp;

while (--n >= 0) {

tmp = a;

a += b;

b = tmp;

}

return a;

}



document.write(fib(10));

```



## 3. 表格支持



示例：



| 项目     | 价格 | 数量  |

| --------  | ----- | ----:  |

| 计算机 | $1600 | 5    |

| 手机    | $12     | 12   |

| 管线    | $1       | 234 |

:表示左右对齐

##缩进

&#160;&#160;&#160;&#160;看到了吧
