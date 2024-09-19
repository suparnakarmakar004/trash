# GROUP-21
\documentclass{article}
\begin{document}
\title{SOFTWARE TOOLS AND TECHNOLOGY Lab Notebook}
\author{MAULANA ABUL KALAM AZAD UNIVERSITY OF TECHNOLOGY}
\date{}
\maketitle

\section*{GROUP-21, TEAM MEMBERS:-}
\begin{itemize}
    \item Name : SUPARNA KARMAKAR(Lead)
        Roll No: 30054623008 ,
       Reg no: 233002410560, 
       Dept:  Bsc in IT(AI),
       \item GIT LINK- https://github.com/suparnakarmakar004/GROUP-21
    \item Name :SUJAL GUPTA, 
        Roll No: 30059223048,
        Reg no: 233002410052,
        Dept: Bsc in Forensic Science
        \item GIT LINK -https://github.com/DreadfullJail18
    \item Name :ADITYA NARAYAN HAMBIR , 
       Roll No:  30059223034,
       Reg no: 233002420038,
       Dept: Bsc in Foresic Science
       \item GIT LINK-https://github.com/Aditya-2005-Hambir 
    \item Name:SNEHA TALAPATRA,Roll no: 30084323019
Reg no:  233002410618,Dept:   Bsc in IT(DS)
\item GIT LINK-https://github.com/Snehatalapatra
\item Name:BISWAJIT NASKAR,Roll no:  30001223014 , Reg no: 233001010488 ,Dept:  BCA
\item GIT LINK-https://github.com/Biswajit213
\end{itemize}
\documentclass{article}
\usepackage{listings}
\usepackage{xcolor}

\lstset{
    language=C,
    basicstyle=\ttfamily\footnotesize,
    keywordstyle=\color{blue}\bfseries,
    commentstyle=\color{gray},
    stringstyle=\color{red},
    numbers=left,
    numberstyle=\tiny\color{gray},
    stepnumber=1,
    frame=single,
    breaklines=true
}

\begin{document}

\title{1. C Program: Basic Calculator}
\author{}
\date{}
\maketitle

\begin{lstlisting}
// Basic Calculator Program in C

#include <stdio.h>

int main() {
    char operator;
    double num1, num2, result;

    // Input operator
    printf("Enter an operator (+, -, *, /): ");
    scanf("%c", &operator);

    // Input two numbers
    printf("Enter two numbers: ");
    scanf("%lf %lf", &num1, &num2);

    // Perform the appropriate calculation
    switch (operator) {
        case '+':
            result = num1 + num2;
            printf("%.2lf + %.2lf = %.2lf\n", num1, num2, result);
            break;
        case '-':
            result = num1 - num2;
            printf("%.2lf - %.2lf = %.2lf\n", num1, num2, result);
            break;
        case '*':
            result = num1 * num2;
            printf("%.2lf * %.2lf = %.2lf\n", num1, num2, result);
            break;
        case '/':
            if (num2 != 0) {
                result = num1 / num2;
                printf("%.2lf / %.2lf = %.2lf\n", num1, num2, result);
            } else {
                printf("Error! Division by zero.\n");
            }
            break;
        default:
            printf("Invalid operator.\n");
            break;
    }

    return 0;
}
\end{lstlisting}

\end{document}
