# 中国科学院大学研究生学位论文中期报告LaTex模板

> 注意，这是本人根据当年的中期报告word模版和 [ucasproposal](https://github.com/mohuangrui/ucasproposal) 修改的LaTeX模板，不保证完全正确，如有错误请提issue。

## 更新
+ 2024.09.05 封面将第二导师信息合并到第一导师信息中
+ 2023.10.13 封面添加第二导师相关信息
+ 2023.10.13 分章节撰写时每章另起一页
+ 2023.10.13 页码用阿拉伯数字编写，右页右对齐，左页左对齐
+ 2023.10.13 奇数页页眉为章节标题，偶数页页眉为论文题目
+ 2023.10.14 增加了中英文摘要 `Tex/Frontmatter.tex`
+ 2023.10.14 封面、摘要、目录后面都有一个空页，用于双面打印

## 未完成的工作
+ 封面字体和WORD模板字体有一点不同。
+ 目录格式和WORD模板的目录有一点不同。

> 欢迎PR。

## 使用

### 方法1
1. 下载本项目：右上角 Code -> Download ZIP。
2. 上传到overleaf：打开[overleaf](https://www.overleaf.com/)上传zip文件。
3. 修改overleaf的编译器为XeLaTex：左上角Menu->Settings->Compiler。

### 方法2
1. 打开[链接](https://www.overleaf.com/read/thwmmpbckgfh#33f55f)。
2. 返回overleaf的[项目主页](https://www.overleaf.com/project)，点击copy按钮，复制项目到自己的overleaf账号。

### 目录
+ `Thesis.tex` 编译用的主文件。

+ `Tex/Frontinfo.tex` 中填写封面信息。

+ `Tex/Frontmatter.tex` 中填写中英文摘要信息。

+ `Tex/Mainmatter.tex` 中填写正文信息。

+ `Biblio/ref.bib` 中填写参考文献信息。

### 删除中英文摘要

+ 删除`Tex/Frontmatter.tex`中
```latex

% ----------------摘要-------------------------
\renewcommand{\abstractname}{\bfseries\zihao{4}摘 \quad 要}

\fancypagestyle{abstractpage}{
    \fancyhf{} % 清空页眉页脚
    \fancyhead[C]{\footnotesize 摘要}
}

\begin{abstract}
    \thispagestyle{abstractpage}
    \zihao{-4}  % 设置摘要正文为宋体小4号字
    这里是摘要的正文内容。摘要需要简要说明研究的目的、方法、结果和结论。
\end{abstract}
\noindent \textbf{关键词：} 关键词1, 关键词2, 关键词3
% --------------------------------------------


% ----------------英文摘要-------------------------
\renewcommand{\abstractname}{\bfseries\zihao{4} Abstract}

\fancypagestyle{abstractpage}{
    \fancyhf{} % 清空页眉页脚
    \fancyhead[C]{\footnotesize Abstract}
}

\begin{abstract}
    \thispagestyle{abstractpage}
    \zihao{-4}  % 设置摘要正文为宋体小4号字
    Here is the text of the abstract. The abstract needs to briefly describe the purpose, methods, results, and conclusions of the study.
\end{abstract}
\noindent \textbf{Keywords:} University of Chinese Academy of Sciences (UCAS), Thesis,
% --------------------------------------------


```
## 致谢
感谢 [ucasproposal](https://github.com/mohuangrui/ucasproposal) 提供的模板，本模板在其基础上进行了修改，使其尽量符合最新的中国科学院大学的中期报告要求。
