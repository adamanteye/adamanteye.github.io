```
\documentclass[UTF8,a4paper]{article}% 文档格式
\usepackage{graphicx}
\usepackage{amsmath}
\usepackage{ctex}% 输出汉字
\usepackage{times}% 英文使用Times New Roman
\usepackage[left=1.50cm,right=1.50cm,top=1.80cm,bottom=1.50cm]{geometry}% 页边距设置
\usepackage{indentfirst}% 中文首行缩进
\renewcommand{\baselinestretch}{1.5}% 定义行间距（1.5）
\usepackage{fancyhdr} %设置全文页眉、页脚的格式
\pagestyle{fancy}

\usepackage{listings}
\usepackage{ctex}

\lstset{
    basicstyle          =   \sffamily,          % 基本代码风格
    keywordstyle        =   \bfseries,          % 关键字风格
    commentstyle        =   \rmfamily\itshape,  % 注释的风格，斜体
    stringstyle         =   \ttfamily,  % 字符串风格
    flexiblecolumns,                % 别问为什么，加上这个
    numbers             =   left,   % 行号的位置在左边
    showspaces          =   false,  % 是否显示空格，显示了有点乱，所以不现实了
    numberstyle         =   \zihao{-5}\ttfamily,    % 行号的样式，小五号，tt等宽字体
    showstringspaces    =   false,
    captionpos          =   t,      % 这段代码的名字所呈现的位置，t指的是top上面
    frame               =   lrtb,   % 显示边框
}

\lstdefinestyle{Matlab}{
    language        =   Matlab,
    basicstyle      =   \zihao{-5}\ttfamily,
    numberstyle     =   \zihao{-5}\ttfamily,
    keywordstyle    =   \color{blue},
    keywordstyle    =   [2] \color{teal},
    stringstyle     =   \color{magenta},
    commentstyle    =   \color{red}\ttfamily,
    breaklines      =   true,   % 自动换行，建议不要写太长的行
    columns         =   fixed,  % 如果不加这一句，字间距就不固定，很丑，必须加
    basewidth       =   0.5em,
}

\title{\fontsize{14pt}{27pt}\selectfont% 四号黑体
	{\heiti% 黑体 
		弦振动~实验报告}}
\author{\fontsize{12pt}{18pt}\selectfont% 小四楷体
	{\kaishu% 楷书
	姓名~~~班级~~~学号}}
\date{\today}
\begin{document}
\maketitle
\lhead{}% 页眉左边设为空
\chead{}% 页眉中间设为空
\rhead{}% 页眉右边设为空
\lfoot{}% 页脚左边设为空
\cfoot{\thepage}% 页脚中间显示页码
\rfoot{}% 页脚右边设为空
\section*{摘要}
\section{实验仪器}
\begin{itemize}
	\item 
\end{itemize}
\begin{figure}[htb]
	\centering
	\includegraphics[scale=0.7]{string-0.png}
	\caption{实验仪器示意图}
\end{figure}
\section{实验内容}

\subsection{实验原理}

\subsection{实验步骤}

\subsubsection*{安装仪器}


\subsection{数据处理}

\section{讨论}

\begin{figure}[hbp] % 多图排版
	\centering
	\begin{minipage}[t]{0.5\linewidth}
		\centering
		\includegraphics[scale=0.4]{1.png}
		\caption{}
		\label{}
	\end{minipage}%
	\begin{minipage}[t]{0.5\linewidth}
		\centering
		\includegraphics[scale=0.4]{2.png}
		\caption{}
		\label{}
	\end{minipage}
	\begin{minipage}[t]{0.5\linewidth}
		\centering
		\includegraphics[scale=0.4]{3.png}
		\caption{}
		\label{}
	\end{minipage}%
	\begin{minipage}[t]{0.5\linewidth}
		\centering
		\includegraphics[scale=0.4]{2.png}
		\caption{}
		\label{}
	\end{minipage}
\end{figure}
\newpage
\appendix
\section{数据}

\section{计算过程}

\subsection{matlab直线拟合代码}
\begin{lstlisting}

\end{lstlisting}
\end{document}
```