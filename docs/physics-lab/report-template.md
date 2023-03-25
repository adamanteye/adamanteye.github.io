```
\documentclass[10.5pt,a4paper]{article}% 文档格式
\usepackage{ctex,hyperref}% 输出汉字
\usepackage{times}% 英文使用Times New Roman
\usepackage[left=2.50cm,right=2.50cm,top=2.80cm,bottom=2.50cm]{geometry}% 页边距设置
\usepackage{indentfirst}% 中文首行缩进
\renewcommand{\baselinestretch}{1.5}% 定义行间距（1.5）
\usepackage{fancyhdr} %设置全文页眉、页脚的格式
\pagestyle{fancy}
\hypersetup{colorlinks=true,linkcolor=black,citecolor=black}% 去除引用红框，改变颜色
\title{\fontsize{14pt}{27pt}\selectfont% 四号黑体
	{\heiti% 黑体 
		弦振动实验}}
\author{\fontsize{12pt}{18pt}\selectfont% 小四楷体
	{\kaishu% 楷书
	姓名~~~班级~~~学号}}
\date{\today}
\begin{document}
\maketitle
\lhead{2023年基础物理实验A(1)}
\chead{}% 页眉中间设为空
\rhead{}% 页眉右边设为空
\lfoot{}% 页脚左边设为空
\cfoot{\thepage}% 页脚中间显示页码
\rfoot{}% 页脚右边设为空
\section*{摘要}
\section{实验仪器}
\section{实验内容}
\subsection{实验原理}
\subsection{实验步骤}
\subsection{数据处理}
\section{讨论}
\appendix
\section{原始数据}
\end{document}
```