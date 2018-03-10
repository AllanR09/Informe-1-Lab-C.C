# Informe-1-Lab-C.C
Primer informe de laboratorio de Circuitos.
%% Este ejemplo está basado en la plantilla
%% bare_jrnl.tex (V1.4a)
%% de Michael Shell (http://www.michaelshell.org/)

\documentclass[journal]{IEEEtran}

% Paquetes a utilizar
\usepackage[utf8]{inputenc} 
\usepackage[spanish]{babel}
\usepackage{graphicx}

% Indicación de como dividir algunas palabras, en caso que no sean correctamente divididas por Latex
\hyphenation{op-tical net-works semi-conduc-tor}

\begin{document}
% Renombrado de algunas partes del texto
\renewcommand{\tablename}{Tabla}
\renewcommand{\IEEEkeywordsname}{Palabras clave}
\renewcommand{\refname}{Bibliografía}

% Título del documento
\title{Informe del experimento 1.}

% Autores
% Se pone el símbolo ~ para separar nombre y apellido para que LaTeX no los separe
% en los saltos de línea

\author{Alejandro Martinez Cartin\\
		Carné: 2016254092\\
        Allan Cespedes Sandí\\
        Carné: 2016}

% Encabezados del documento
\markboth{ITCR. Martinez, Cespedes. Informe de Experimento 1.}%
{}
% Se puede poner un segundo encabezado dentro de las llaves de la línea anterior.
% Este segundo encabezado aparece si se utiliza la opción twoside en documentclass

% Para crear el título
\maketitle

% El resumen
\begin{abstract}
En este informe explicaremos lo realizado en el primer experimento de laboratorio de mediciones así como demostrar los resultados y conclusiones al respecto
\end{abstract}

% Las palabras clave
%\begin{IEEEkeywords}
%Informe, laboratorio, \LaTeX, ejemplo.
%\end{IEEEkeywords}

\section{Introducción}

En el informe se realiza la medición de 
\textbf{Este texto va en negrita}.
\textit{Este texto va en cursiva}.
Los saltos de línea (como el usado en esta parte del documento) no producen un cambio de párrafo.

Para cambiar de párrafo hay que dejar una línea en blanco entre dos líneas, justo como en este caso.

Para poner símbolos especiales hay que usar un ''backslash'' (\textbackslash) antes de estos:

\textbackslash \_ : texto\_1

\textbackslash \$ : texto\$1

\textbackslash \& : texto\&1

El ''backslash'' es un caracter de control en \LaTeX, por lo que hay que usarlo con cuidado.
Un doble ''backslash'' sirve para dejar una línea en blanco: \\

A continuación se inserta una figura.

\begin{figure}[!ht]
	\centering
    \fbox{\includegraphics[width=2.5in]{archivo.png}} %fbox se utiliza para dibujar el borde de la figura
    \caption{Este es el título de la figura.}
    \label{fig_paralelo} %Este es un texto para hacer referencia a la figura
\end{figure}

Se puede hacer referencia a una figura por medio de la instrucción \textbackslash ref.
\textbf{Ejemplo:} En la fig. \ref{fig_paralelo} se tiene un circuito en paralelo.

\subsection{Esta es una subsección}

Ahora se presenta una lista numerada:
\begin{enumerate}
	\item Opción 1.
	\item Opción 2.
\end{enumerate}

Una lista con viñetas en lugar de números:
\begin{itemize}
	\item Primera opción.
	\item Segunda opción.
\end{itemize}

\LaTeX se encarga de colocar las figuras y las tablas donde considere que se ubican mejor.
Debido a esto, tiende a colocarlos al inicio o al final de las páginas.
En el documento \emph{pdf} se podrían observar, eventualmente, todas las tablas juntas.
Esto es esperable y por lo tanto, conviene hacer referencia a tablas y figuras por medio de sus números.

En la tabla \ref{tab_ejemplo_1} se tienen líneas verticales dobles, y se usan dos columnas. En la tabla \ref{tab_ejemplo_2} se tienen tres columnas.

\begin{table}[!ht]
  \centering
  \caption{Este es el título de la tabla \ref{tab_ejemplo_1}.}
  \begin{tabular}{|c||c|}
    \hline
    Uno & Dos\\
    \hline
    Tres & Cuatro\\
    \hline
  \end{tabular}
  \label{tab_ejemplo_1}
\end{table}

\begin{table}[!ht]
  \centering
  \caption{Este es el título de la tabla.}
  \begin{tabular}{|c||c||c|}
    \hline
    Uno & Dos & Tres\\
    \hline
    Cuatro & Cinco & Seis\\
    \hline
  \end{tabular}
  \label{tab_ejemplo_2}
\end{table}

En la tabla \ref{tab_ejemplo_3} se tienen tres columnas, además de filas que requieren varios renglones. También se eliminó la línea doble en vertical:

\begin{table}[!ht]
  \centering
  \caption{Este es el título de la tabla.}
  \begin{tabular}{|c|c|c|}
    \hline
    Texto & Texto & Texto\\
    largo 1 & largo 2 & largo 3\\
    \hline
    Texto & Texto & Texto\\
    más & más &más\\
    largo 1 & largo 2 & largo 3\\
    \hline
  \end{tabular}
  \label{tab_ejemplo_3}
\end{table}

Las ecuaciones se pueden escribir de diferentes formas.
Por ejemplo, se pueden escribir ecuaciones dentro de un párrafo encerrándolas entre símbolos de dólar: $ N = \frac{2}{p} $.
También se pueden escribir por fuera del párrafo, y con un tamaño completo usando doble símbolo de dólar:

$$N = \frac{2}{p}$$

Se pueden enumerar las ecuaciones, pero en ese caso hay que escribirlas como se muestra en la ec. \ref{ec_a}:

\begin{equation}
	N = \frac{2}{p}
    \label{ec_a}
\end{equation}

Algunos ejemplos de ecuaciones:

$$(x^m)^n=x^{mn}$$

$$x_1=1,\quad x_2=1,\quad x_n=x_{n-1}+x_{n-2}\;\;(n>2)$$

$$\sqrt[5]{4}$$

\[ \overbrace{x+\underbrace{y+z}_{2} +w}^{4} \]

Para hacer referencia a un elemento de la bibliografía se usa \textbackslash cite: los ejemplos de las ecuaciones fueron tomados de \cite{apuntes}. Más sobre bibliografías en \LaTeX en \cite{sobreBibliografia}.

\section{Conclusiones}
Conclusiones del trabajo.

Texto texto texto texto texto texto texto texto texto texto texto texto texto.

Texto texto texto texto texto texto texto texto texto texto texto texto texto texto texto.

Texto texto texto texto texto texto texto texto texto texto texto texto texto texto texto texto texto texto texto texto texto.

% Un apéndice contiene material generado por el autor del documento,
% sin embargo es complementario al resto del trabajo, y por lo tanto se
% coloca al final en caso que el lector quiera revisarlo

% NO colocar las ecuaciones que deberían ir en el cuerpo del texto aquí

\appendices
\section{Demostración de...}
Texto del apéndice.


\section{}
Texto del apéndice.

% Se puede usar BibTeX para generar la bibliografía
\begin{thebibliography}{X}
% El caracter dentro de la llave {X} es para indicarle a LateX la cantidad de cifras que
% van a tener las citas, en este caso un caracter implica citas desde 1 hasta 9.
% Con dos caracteres (por ejemplo {XX}) se podrían definir citas desde 1 hasta 99.
% No importa qué caracter se coloca entre las llaves, solo la cantidad de estos.

\bibitem{kopka} %Texto para hacer referencia a este elemento 
H.~Kopka and P.~W. Daly, \emph{A Guide to \LaTeX}, 3rd~ed.\hskip 1em plus
  0.5em minus 0.4em\relax Harlow, England: Addison-Wesley, 1999.

\bibitem{apuntes}
“Apuntes de Latex Capítulo 3: Fórmulas matemáticas – Conceptos básicos.” [Online]. Disponible en: http://metodos.fam.cie.uva.es/~latex/curso-2015/apuntes3.pdf. [Accedido: 01-Mes-2017].

\bibitem{sobreBibliografia}
"LaTeX: Generación de bibliografías con thebibliography – 1" [Online]. Disponible en: 
http://elclubdelautodidacta.es/wp/2012/09/latex-generacion-de-bibliografias-con-thebibliography-1/. [Accedido: 01-Mes-2017].

\end{thebibliography}

\end{document}
