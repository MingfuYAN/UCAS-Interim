# 中国科学院大学研究生学位论文开题报告LaTex模板

## 使用
1. 下载本项目：右上角 Code -> Download ZIP。
2. 上传到overleaf：打开[overleaf](https://www.overleaf.com/)上传zip文件。
3. 修改overleaf的编译器为XeLaTex：左上角Menu->Settings->Compiler。

## 未完成的工作
+ 封面字体和WORD模板字体有一点不同。
+ 目录格式和WORD模板的目录有一点不同。

> 欢迎PR。

## 格式
+ 封面添加第二导师相关信息
+ 分章节撰写时每章另起一页
+ 页码用阿拉伯数字编写，右页右对齐，左页左对齐
+ 奇数页页眉为章节标题，偶数页页眉为论文题目

## 使用

如不需要第二导师，需要
+ 删除`Tex/Frontinfo.tex`中
```latex
\advisortwo{董超}% 第二指导老师
\advisortitletwo{研究员}% 第二指导老师职务
```
+ 删除`Style/ucasproposal.cls`中第`223`行的第二导师相关代码。
```latex
\ucas@label@ch@advisor & \ulenhance{\ulextend[151pt]{\hspace*{-\ulhshift}\ucas@value@ch@advisortwo}}\ucas@label@ch@advisortitle\ulenhance{\ulextend[170pt]{\hspace*{-\ulhshift}\ucas@value@ch@advisortitletwo}}\\
```

## 致谢
感谢 [ucasproposal](https://github.com/mohuangrui/ucasproposal) 提供的模板，本模板在其基础上进行了修改，使其尽量符合最新的中国科学院大学的开题报告要求。
