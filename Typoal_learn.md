[TOC]
# [Markdown+Typora] 学习记录

TaoXu 2023/5
## 简要介绍
**Markdown** 是一种轻量型标记语言，是一种语法。与 “.md” 为后缀的文本就是Markdown文件，相较于 **Word** ，它更像是**Latex** ，透露着一种极简主义，具有高效、简洁的特点，同时语法简单。

## 实际应用
所有的文本编辑都可以用Markdown完成
它可以让你不再纠结什么字体、什么样式、什么逻辑，而且逻辑清晰、层次分明。

## 工具
Markdown只是一种语法，用来编辑Markdown的编辑器一般采用**Typora**或Vscode

## Typora
Typora 应该是被广泛用于写 Markdown 的文本软件, 就和 Markdown 语法一样高效. 而且它还有很实用的扩展语法与自定义样式的功能. 其能将 `.md` 导出成多种文件, 如 `.pdf`, `.html`, `.docx` (没想到吧, 能导出到 Word)。

## Vscode
这是微软家的开源文本编辑器, 理论上来说所有代码, 语言, 都可以用 VS Code 来写, 同样是非常的简洁好用. 在下载插件 **Markdown All in One** 后对 Markdown 的基础支持也是非常的好. 若在 VS Code 下载 Markdown 各种附加扩展, 就能获得比 Typora 更加丰富的扩展语法与操作。

## Markdown 的基础语法
### 0. 写Markdown的第0步
Markdown的标点输入为半角，即英文键盘下的标点符号，中文下的标点不被Markdown认可。

### 1. 标题 [N个 “#” + 空格]


```
# 一级标题
## 二级标题
### 三级标题
#### 四级标题
```
标题会在目录与大纲处分级显示，可点击跳转。
建议在Typora软件中开启’严格模式‘，即不应为’#标题‘，应该为’# 标题‘，使得Markdown语法在其它编辑器上兼容。

### 2. 强调 [用 “**” 包围], 快捷键：’Ctrl + B‘
```
**Markdown学习笔记**
```
**基于Typora的Markdown学习笔记**

### 3. 斜体 [用 "*" 包围]，快捷键: 'Ctrl + I'
```
*Markdown学习笔记*
```
*基于Typora的Markdown学习笔记*

### 4. 强调并斜体 [用 '***' 包围
```
***Markdown学习笔记***
```
***基于Typora的Markdown学习笔记***

### 5. 删除线 [用’~~‘包围]
```
~~Markdown学习笔记~~
```
~~基于Typora的Markdown学习笔记~~

### 6. 高亮显示 [用 ’==‘ 包围] 
(扩展语法，仅在 Typora 或 添加了扩展的 VS Code **本地生效**, 在大多数平台上**并不认可**.)
```
==Markdown学习笔记==
```
==基于Typora的Markdown学习笔记==

### 7. 代码 [用 "`"包围]

```
`sudo apt update`
```

`sudo apt update`
~~"请输入管理员密码："~~

### 8. 代码块 [用"````+语言"包围]

````c++
#include <iostream>
#include <stdio.h>

int main(int argc, char * argv)
{
	std::cout<<"This is C++ !"<<endl;
	
	return 0;
}
````
### 9. 无序列表 [用 “-” + 空格]
```
- Markdown
- Typora
- Vscode
```
- Markdown
- Typora
- Vscode

### 10. 有序列表 [ 数字 + "." + 空格]
1. 语文
	1.1 古诗
2. 数学
3. 英语	
	敲回车会自动补全, 敲回车后按下 `Tab` 会缩进一级.

### 11. 任务列表 [ "- [空格]" + 空格 ]
```
- [ ] 吃饭
- [ ] 工作
- [ ] 玩耍
- [x] 睡觉 //x表示勾选
```
- [ ] 吃饭
- [ ] 工作
- [ ] 玩耍
- [x] 睡觉


### 12. 上标 [用"^"包围]
(扩展语法，仅在 Typora 或 添加了扩展的 VS Code **本地生效**, 在大多数平台上**并不认可**.)
```
2^4^=16
```
2^4^=16

### 13. 下标 [用"~"包围]
(扩展语法，仅在 Typora 或 添加了扩展的 VS Code **本地生效**, 在大多数平台上**并不认可**.)
```
H~2~O
```
H~2~O

### 14. 引用与注释 [用 “> ”和“[^]” 表示]
(扩展语法，仅在 Typora 或 添加了扩展的 VS Code **本地生效**, 在大多数平台上**并不认可**.)
```
> 今日我们相聚于此, 是为了学习 Markdown 的使用, 它的教程对于全体「观众」而言, 值得足足两个硬币的支持鼓励![^1]
[^1]: 沃兹·基·硕德 改编自「公鸡」普契涅拉.
```

> 今日我们相聚于此, 是为了学习 Markdown 的使用, 它的教程对于全体「观众」而言, 值得足足两个硬币的支持鼓励![^1]

[^1]: 沃兹·基·硕德 改编自「公鸡」普契涅拉.

### 15. 链接 [常用"[]" + "()" 分别包含文本与链接，支持网页链接和文内跳转]
(扩展语法，仅在 Typora 或 添加了扩展的 VS Code **本地生效**, 在大多数平台上**并不认可**.)
```
[远程仓库](https://github.com/TaoXu-HNU)
[基础教程: 12. 下标](#12. 下标 [用 "~" 包围])
```
[远程仓库](https://github.com/TaoXu-HNU)
[基础教程: 12. 下标](#12. 下标 [用 "~" 包围])

### 16. 表格 [用"|" 绘制表格的边框]
```
|学号|姓名|年龄|
|:----|:--:|---:|  (引号的位置代表着 左对齐, 居中, 右对齐,'-'表示长度)
|1101|张三|22|
|1102|李四|25|
```
|学号|姓名|年龄|
|:----|:--:|---:| 
|1101|张三|22|
|1102|李四|25|

### 17. 图片 [直接拖进来或者复制粘贴]
Ps: 需要切换到非源代码模式下才可以拖动或复制粘贴图片

<img src="F:\0525-Typora\Typoal_learn.assets\c2ad3e918b9c4360ba4208b3385239ce.jpg" alt="c2ad3e918b9c4360ba4208b3385239ce" style="zoom: 33%;" />

<img src="F:\0525-Typora\Typoal_learn.assets\7d4f9f1ea11a4e4ab45f74802895fac0.jpg" alt="7d4f9f1ea11a4e4ab45f74802895fac0" style="zoom:50%;" />

### 18. 分割线 [用 "***" +回车 ]
```
分割线1
***
分割线2
***
```
分割线1
***
分割线2
***

## Markdown 进阶教程
### 1. 目录 [自动生成]
```
[TOC]  // Typora 软件特有的自动生成目录的方法，放在本文档的开头！
```

### 2. 内联公式 [用 "$" 包围]
**注意：部分编译器会出现不识别部分符号**
**用 `$` 包围为单条公式, 按下两个 `$` 并敲回车即生成公式块.**

```
$\LaTeX$ 是最好用的论文排版语言! 不信你看!
$a^n+b^n=c^n$ 
```
$\LaTeX$ 是最好用的论文排版语言! 不信你看!
$a^n+b^n=c^n$

#### 3. Markdown 的常用快捷键
|          按键          |          效果          |          按键          |          效果           |
| :--------------------: | :--------------------: | :--------------------: | :---------------------: |
|      `Ctrl` + `D`      |     **选中当前词**     |      `Ctrl` + `L`      |      选中当前句/行      |
|      `Ctrl` + `E`      |    **选中当前区块**    |      `Ctrl` + `F`      |      搜索当前选中       |
|      `Ctrl` + `B`      |    **加粗当前选中**    |      `Ctrl` + `H`      |      替换当前选中       |
|      `Ctrl` + `I`      |    **倾斜当前选中**    |      `Ctrl` + `U`      |      下划当前选中       |
|      `Ctrl` + `K`      | **将当前选中生成链接** |      `Ctrl` + `J`      | 滚动屏幕将选中滚至顶部  |
|      `Ctrl` + `W`      |      关闭当前窗口      |      `Ctrl` + `N`      |       打开新窗口        |
|      `Ctrl` + `O`      |        打开文件        |      `Ctrl` + `P`      |     搜索文件并打开      |
|    `Ctrl` + `回车`     |     表格下方插入行     |      `Ctrl` + `,`      |      打开偏好设置       |
|      `Ctrl` + `.`      |   切换全角/半角标点    |      `Ctrl` + `/`      | **切换正常/源代码视图** |
| `Ctrl` + `Shift` + `-` |      缩小视图缩放      | `Ctrl` + `Shift` + `+` |      放大视图缩放       |

## 总结
至此, **Markdown + Typora / VSCode** 的手册教程也告一段落. 

其实 Markdown 只是标记语言的最开始,. 标记语言正是为了摆脱 Word 那种虽然"所见即所得", 但又过于花哨浮华, 很差的兼容性与闭源的编码的缺陷. 当你能掌握这样的"**所写即所得**"时, 你肯定会感受到用 Markdown 这类语言来处理文本的妙处!