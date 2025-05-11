\documentclass[12pt]{article}
\usepackage{listings}
\usepackage[margin=1in]{geometry}
\usepackage{xcolor}
\usepackage{graphicx} % For including images

% Code formatting
\lstset{
    language=Java,
    basicstyle=\ttfamily\small,
    keywordstyle=\color{blue},
    stringstyle=\color{red},
    commentstyle=\color{gray},
    numbers=none,
    showstringspaces=false,
    frame=single,
    breaklines=true
}

\begin{document}

% Centered Title Page
\begin{titlepage}
    \centering
    \vspace*{5cm}
    {\Huge\bfseries Simple Example of Method Overloading in Java \par}
    \vspace{2cm}
    {\large \today\par}
\end{titlepage}

% Table of Contents
\tableofcontents
\newpage

\section{What is Method Overloading?}
Method overloading in Java means creating multiple methods with the same name but different parameters. This helps reuse method names and improves readability.

\section{Java Code Example}
\begin{lstlisting}
public class Test {
    void show() {
        System.out.println("No arguments");
    }

    void show(int a) {
        System.out.println("One integer: " + a);
    }

    public static void main(String[] args) {
        Test obj = new Test();
        obj.show();
        obj.show(5);
    }
}
\end{lstlisting}

\section{Output}
\begin{center}
    \includegraphics[width=0.6\textwidth]{sigh.jpg} % Ensure the image file exists
\end{center}

\section{Explanation}
\begin{itemize}
    \item \textbf{show()} prints a message without needing any input.
    \item \textbf{show(int a)} prints the integer that is passed to it.
    \item Depending on how we call \texttt{show()}, the correct version runs.
\end{itemize}

\end{document}
  
