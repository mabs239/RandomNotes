# الصَّلاةُ وَالسَّلامُ عَلَيْكَ يَا رَسُولَ اللهِ

#  اَلْحَمْدُ لِلّٰهِ رَبِّ الْعٰلَمِیْنَۙ
- نَحْمَدُہُ وَ نُصَلّیِ عَلٰی رَسُولِہِ الْکَرِیْمْ 

# اشعار

کیا فکر کی جولانی کیا عرض ہنر مندی 

توصیف پیمبرﷺ ہے توفیق خداوندی 

# Fonts

**Urdu Font** https://www.google.com/get/noto/#kufi-arab

# Computer/Mobile Tips
*Mark Down Cheat Sheet*
- https://www.markdownguide.org/basic-syntax/
- https://help.github.com/en/github/getting-started-with-github/keyboard-shortcuts
### Save 4GB of Hibernate state data
Turn off the hibernate mode
save space: hiberfil.sys stored in 4GB file
`powercfg -h off`
Ref: https://www.howtogeek.com/howto/15140/what-is-hiberfil.sys-and-how-do-i-delete-it/

### WinSXS
Disk Clean Up > Windows update Cleanup 
Ref: https://www.laptopmag.com/articles/clean-winsxs-folder-to-save-space

# LaTeX Tips
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

# Excel Tips
Change product of two base 60 (1 through 59) to ABJD words in excel. Both place value 1 and place value 60 words returned with a space inbetween.
LOOKUP(INT(INT((C$2*$A4)/60)/10)*10,{0,1,2,3,4,5,6,7,8,9,10,20,30,40,50},{"","ا","ب","ج","د","ہ","و","ز","ح","ط","ی","ک","ل","م","ن"})& LOOKUP(MOD(INT((C$2*$A4)/60),10),{0,1,2,3,4,5,6,7,8,9,10,20,30,40,50},{"","ا","ب","ج","د","ہ","و","ز","ح","ط","ی","ک","ل","م","ن"}) &CHAR(10)&"    "& LOOKUP(INT(MOD(C$2*$A4,60)/10)*10,{0,1,2,3,4,5,6,7,8,9,10,20,30,40,50},{"","ا","ب","ج","د","ہ","و","ز","ح","ط","ی","ک","ل","م","ن"})& LOOKUP(MOD(MOD(C$2*$A4,60),10),{0,1,2,3,4,5,6,7,8,9,10,20,30,40,50},{"","ا","ب","ج","د","ہ","و","ز","ح","ط","ی","ک","ل","م","ن"})

# Online Resources
تاب المجسطي Ptolemy بطلميوس

https://fromthepage.com/bldigital/arabic-scientific-manuscripts/add-ms-7474-6308f07e-5248-4584-aa5b-372430968cb6/display/54909

الدر الثمين في شرح أرجوزة ابن الياسمين

https://fromthepage.com/bldigital/arabic-scientific-manuscripts/delhi-arabic-1901/display/53453

Qatar Digital Library

https://www.qdl.qa/en/search/site/ptolemy?page=2&f%255B0%255D=document_source%3Aarchive_source&retain-filters=1

http://kolkotob.blogspot.com/2015/01/1540.html?m=0

https://archive.org/search.php?query=makhtouta

https://issuu.com/murshidgee/docs/israr_e_najoom

https://ar.wikipedia.org/wiki/%D8%B9%D9%84%D9%85_%D8%A7%D9%84%D9%81%D9%84%D9%83_%D9%81%D9%8A_%D8%B9%D8%B5%D8%B1_%D8%A7%D9%84%D8%AD%D8%B6%D8%A7%D8%B1%D8%A9_%D8%A7%D9%84%D8%A5%D8%B3%D9%84%D8%A7%D9%85%D9%8A%D8%A9


# Electronics Circuits and Chips
6pcs 6 Kinds Sound Chip Voice Module Music IC Alarm/Recordable Sound/Dog Barking/Chinese Music/Christmas Song for DIY Toy Gift
Sound Module for Electronic Toy IC Chip Voice Recorder 120s 120secs Recording Playback Talking Music Audio Recordable Board Gift
6secs 6S Sound Voice Audio Recordable Recorder Module Chip Programmable ISD1806B-COB Board 0.5W Speaker For Greeting Card
5Pcs H-83A 12 kind of songs sound music ic voice chip module music circuit board | eBay
- PX85
- H-83A
- ISD1760
- ISD1820

# Physics
### Research: Why Moving Bicycle is stable?
https://physics.stackexchange.com/questions/506/why-doesnt-a-bike-bicycle-fall-if-going-with-a-high-speed

http://ruina.tam.cornell.edu/

https://physics.stackexchange.com/questions/24/does-leaning-banking-help-cause-turning-on-a-bicycle/524#524

https://ezramagazine.cornell.edu/SUMMER11/ResearchSpotlight.html

## Qibla Direction
الحاسب في علم النجوم و اصول الهيئة و حركات الاشخاص السماوية- 
 
- علامہ برجندی نے شرح تحریر مجسطی
- عبر العلى برجندی نقل في شرح النقاية
- حاشیہ شرح چغمینی للعلامہ البرجندی
- فی الحاشیۃ الشامیۃ فی حاشیۃ الفتال عن البرجندی 
- عبدالعلی بن محمد برجندی
- مولانا عبدالعلاء برجندی
 - , جیب اور عمل
 - تفاضل
-  الحاسب
 - شمالی انحراف کا ظل
 - Faizabad 27.5241582,80.7462959
 - Khana Kaaba 21.4224829,39.8240889
 - 9.8801802
 - 9.7133620

