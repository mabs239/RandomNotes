# Reclaim Disk Space
Tips and Notes

## Save 4GB of Hibernate state data
Turn off the hibernate mode

save space: hiberfil.sys stored in 4GB file

powercfg -h off

Ref: https://www.howtogeek.com/howto/15140/what-is-hiberfil.sys-and-how-do-i-delete-it/

## WinSXS
Disk Clean Up > Windows update Cleanup 
Ref: https://www.laptopmag.com/articles/clean-winsxs-folder-to-save-space

## LaTeX Tips
To number equation within subsection. Requieres amsmath package
\usepackage{amsmath}
\numberwithin{equation}{subsection}

Set section counter to 10
\setcounter{section}{10}

To write beautiful E
\usepackage{boondox-cal}
\mathcal{E}

To allign continued equations under equal sign
\begin{align}\label{key}
y_m=& \sum_{n=-\infty}^\infty a_n x_{m-n}+w_m \nonumber \\
=& x_0a_m+\sum_{n\neq m}a_n x_{m-n}+w_m
\end{align}

To conditional equation allignment
\begin{equation}\label{eq:recursive}
    P_{VPAPM} = \left\{\begin{array}{cc}
    \sqrt{\frac{2M^2}{B_I \log_2(2M)}} & 0\leq B_I <0  \\
	\sqrt{\frac{2M^2}{(1-B_I) \log_2(2M)}} & 0.5 \leq B_I <1
\end{array}   \right..
\end{equation}

To define a4 size paper
\documentclass[a4paper]{article}

To write the sinc fuction like \sin and \cos
\DeclareMathOperator{\sinc}{sinc}

To add header and footer to a page
\usepackage{fancyhdr}
\pagestyle{fancy}
\lhead{Engr. Muhammad Abu Bakar Siddique}
%\rhead{\thepage}
\rhead{RCET, UET Lahore}

To add a figure
\usepackage{graphicx}
\begin{figure}[h] 
	\includegraphics[width=\textwidth]{../figures/fig10_.png}	
	\caption{}
	\label{fig10_}
\end{figure}

To cahnge figure number insection as opposed to continuous
\usepackage{chngcntr}
\counterwithin{figure}{section}
\setcounter{figure}{0}


To refer a figure by \ref, \caption must come before \label. Otherwise figure number would be wrong.
\usepackage{graphicx}
\begin{figure}[!htbp]
	\includegraphics[width=\textwidth]{../figures/fig10_.png}	
	\caption{}
	\label{fig10_}
\end{figure}

To write syntax highlighted Matlab codes
\usepackage{listings}
\lstset{captionpos=b,
        frame=tb,
        basicstyle=\scriptsize\ttfamily,
        show 

stringspaces=false,
        keepspaces=true}
\lstdefinestyle{matlab} {
        language=Matlab,
        keywordstyle=\color{blue},
        commentstyle=\color[rgb]{0.13,0.55,0.13}\em,
        stringstyle=\color[rgb]{0.7,0,0} }
\usepackage[numbered,framed]{matlab-prettifier}
\begin{lstlisting}[style=Matlab-editor,basicstyle=\mlttfamily]
\end{lstlisting}

## Excel Tips
Change product of two base 60 (1 through 59) to ABJD words in excel. Both place value 1 and place value 60 words returned with a space inbetween.
LOOKUP(INT(INT((C$2*$A4)/60)/10)*10,{0,1,2,3,4,5,6,7,8,9,10,20,30,40,50},{"","ا","ب","ج","د","ہ","و","ز","ح","ط","ی","ک","ل","م","ن"})& LOOKUP(MOD(INT((C$2*$A4)/60),10),{0,1,2,3,4,5,6,7,8,9,10,20,30,40,50},{"","ا","ب","ج","د","ہ","و","ز","ح","ط","ی","ک","ل","م","ن"}) &CHAR(10)&"    "& LOOKUP(INT(MOD(C$2*$A4,60)/10)*10,{0,1,2,3,4,5,6,7,8,9,10,20,30,40,50},{"","ا","ب","ج","د","ہ","و","ز","ح","ط","ی","ک","ل","م","ن"})& LOOKUP(MOD(MOD(C$2*$A4,60),10),{0,1,2,3,4,5,6,7,8,9,10,20,30,40,50},{"","ا","ب","ج","د","ہ","و","ز","ح","ط","ی","ک","ل","م","ن"})

