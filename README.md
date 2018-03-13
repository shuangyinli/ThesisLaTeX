# ThesisLaTeX
<p>
Thesis-LaTeX template for Sun Yan-sen University
<br>
<br>
USAGE:
<br>
首先，按如下序列运行后可得到main.pdf文件:<br>
xelatex main.tex<br>
bibtex main.aux<br>
xelatex main.tex<br>
xelatex main.tex<br>

其次，请在sysuthesis.bib里面添加论文引用。<br>

最后，运行如下命令可得到两个文件分别供彩色打印机和黑白打印机打印, 其中的 "3 5 8"
	是包含了彩图的页面, 这种页面连同其背面需要成双输出给彩色打印机, 因此需
	要这样分拆:<br>
./split.sh main.pdf 0  3 5 8<br>

（当然，大家也可以选择全部彩印）<br>


========================更新说明2018.3.12=======================================<br>

1，更新了sysuthesis.cls<br>
2，调试了mac下，在macos+TeX+texstudio的环境下修改和编译通过的。ubuntu下相同的环境应该也可以编译通过，不过未测试。<br>
3，支持了博士学位论文，硕士学位论文和本科毕业论文。只需要在sysuthesis.cls的109行，110行，111行选择相应的选项，去掉注释即可。默认是硕士学位论文。切记，一定要根据自己的情况修改此处，这决定了页眉和页脚。<br>
4，增加了images的文件夹，用于集中放置论文中的图像。<br>
5，删除了每个文件夹下的test模式，因为这个模式太啰嗦了，使得结构不清晰。新的版本结构如下：<br>

sysuthesis/main.tex<br>
----------/README<br>
----------/script.sh<br>
----------/sysuthesis.bst<br>
----------/sysuthesis.cls<br>
----------/references.bib<br>
<br>
----------/iamges/**.eps<br>
<br>
----------/frontmatter/frontmatter.tex<br>
<br>
----------/abstract/abstract.tex<br>
<br>
----------/mainbody/chapters/foreword.tex<br>
----------/mainbody/chapters/chapter1.tex<br>
----------/mainbody/chapters/chapter2.tex<br><br>
----------/mainbody/chapters/conclusion.tex<br>
<br>
----------/appendix/appendix.tex<br>
<br>
----------/backmatter/backmatter.tex<br>
<br><br>
