# HV
Tarea HV
%%%%%%%%%%%%%%%%%
% This is an sample CV template created using altacv.cls
% (v1.6.4, 13 Nov 2021) written by LianTze Lim (liantze@gmail.com). Now compiles with pdfLaTeX, XeLaTeX and LuaLaTeX.
%
%% It may be distributed and/or modified under the
%% conditions of the LaTeX Project Public License, either version 1.3
%% of this license or (at your option) any later version.
%% The latest version of this license is in
%%    http://www.latex-project.org/lppl.txt
%% and version 1.3 or later is part of all distributions of LaTeX
%% version 2003/12/01 or later.
%%%%%%%%%%%%%%%%

%% Use the "normalphoto" option if you want a normal photo instead of cropped to a circle
% \documentclass[10pt,a4paper,normalphoto]{altacv}

\documentclass[10pt,a4paper,ragged2e,withhyper]{altacv}
%% AltaCV uses the fontawesome5 and packages.
%% See http://texdoc.net/pkg/fontawesome5 for full list of symbols.

% Change the page layout if you need to
\geometry{left=1.25cm,right=1.25cm,top=1.5cm,bottom=1.5cm,columnsep=1.2cm}

% The paracol package lets you typeset columns of text in parallel
\usepackage{paracol}

% Change the font if you want to, depending on whether
% you're using pdflatex or xelatex/lualatex
\ifxetexorluatex
  % If using xelatex or lualatex:
  \setmainfont{Roboto Slab}
  \setsansfont{Lato}
  \renewcommand{\familydefault}{\sfdefault}
\else
  % If using pdflatex:
  \usepackage[rm]{roboto}
  \usepackage[defaultsans]{lato}
  % \usepackage{sourcesanspro}
  \renewcommand{\familydefault}{\sfdefault}
\fi

% Change the colours if you want to
\definecolor{SlateGrey}{HTML}{2E2E2E}
\definecolor{LightGrey}{HTML}{666666}
\definecolor{DarkPastelRed}{HTML}{450808}
\definecolor{PastelRed}{HTML}{8F0D0D}
\definecolor{GoldenEarth}{HTML}{E7D192}
\colorlet{name}{black}
\colorlet{tagline}{PastelRed}
\colorlet{heading}{DarkPastelRed}
\colorlet{headingrule}{GoldenEarth}
\colorlet{subheading}{PastelRed}
\colorlet{accent}{PastelRed}
\colorlet{emphasis}{SlateGrey}
\colorlet{body}{LightGrey}

% Change some fonts, if necessary
\renewcommand{\namefont}{\Huge\rmfamily\bfseries}
\renewcommand{\personalinfofont}{\footnotesize}
\renewcommand{\cvsectionfont}{\LARGE\rmfamily\bfseries}
\renewcommand{\cvsubsectionfont}{\large\bfseries}


% Change the bullets for itemize and rating marker
% for \cvskill if you want to
\renewcommand{\itemmarker}{{\small\textbullet}}
\renewcommand{\ratingmarker}{\faCircle}

%% Use (and optionally edit if necessary) this .tex if you
%% want to use an author-year reference style like APA(6)
%% for your publication list
\input{pubs-authoryear}

%% Use (and optionally edit if necessary) this .tex if you
%% want an originally numerical reference style like IEEE
%% for your publication list
% \input{pubs-num}

%% sample.bib contains your publications
\addbibresource{sample.bib}

\begin{document}
\name{Carlos Santiago Estacio Malte}
\tagline{Ingeniero Electrónico}
%% You can add multiple photos on the left or right
\photoR{2.8cm}{Globe_High}
% \photoL{2.5cm}{Yacht_High,Suitcase_High}

\personalinfo{%
  % Not all of these are required!
  \email{santiago.estacio@udea.edu.co}
  \phone{3105471586}
  \mailaddress{Cra 51c #67a-40 Barrio Sevilla}
  \location{Medellín, Colombia}
  \homepage{www.eecs.com}
  \twitter{@santx27}
  \linkedin{santx_27}
  \github{95398717}
  \orcid{0512-0542-0040-0450}
  %% You can add your own arbitrary detail with
  %% \printinfo{symbol}{detail}[optional hyperlink prefix]
  % \printinfo{\faPaw}{Hey ho!}[https://example.com/]
  %% Or you can declare your own field with
  %% \NewInfoFiled{fieldname}{symbol}[optional hyperlink prefix] and use it:
  % \NewInfoField{gitlab}{\faGitlab}[https://gitlab.com/]
  % \gitlab{your_id}
  %%
  %% For services and platforms like Mastodon where there isn't a
  %% straightforward relation between the user ID/nickname and the hyperlink,
  %% you can use \printinfo directly e.g.
  % \printinfo{\faMastodon}{@username@instace}[https://instance.url/@username]
  %% But if you absolutely want to create new dedicated info fields for
  %% such platforms, then use \NewInfoField* with a star:
  % \NewInfoField*{mastodon}{\faMastodon}
  %% then you can use \mastodon, with TWO arguments where the 2nd argument is
  %% the full hyperlink.
  % \mastodon{@username@instance}{https://instance.url/@username}
}

\makecvheader
%% Depending on your tastes, you may want to make fonts of itemize environments slightly smaller
% \AtBeginEnvironment{itemize}{\small}

%% Set the left/right column width ratio to 6:4.
\columnratio{0.6}

% Start a 2-column paracol. Both the left and right columns will automatically
% break across pages if things get too long.
\begin{paracol}{2}
\cvsection{Experiencia}

\cvevent{Asesor Técnico}{SUMMAR TEMPORALES S.A.S}{Febuary-2019 -- En curso}{Medellín}
\begin{itemize}
\item Realizar la instalación, asesorías, mantenimientos predictivos, preventivos y correctivos a los equipos de diagnóstico automotriz de los clientes internos y externos.
\end{itemize}

\divider

\cvevent{Control de Instrumentación}{POLCO S.A.S}{Marzo 2017 -- Enero 2019}{Medellín}
\begin{itemize}
\item Brindar todo el soporte Técnico comercial especializado para la venta de los productos y servicios de la organización con conocimientos y experiencia en metrología y calibración para cumplir con los presupuestos de ventas de Polco.

\end{itemize}

\cvsection{Proyectos}

\cvevent{Proyecto 1}{INSOL S.AS}{}{}
\begin{itemize}
\item Herramienta Software para la Simulación de un Caso Clínico de Neumonía Usando Realidad Virtual
\end{itemize}

\divider

\cvevent{Proyecto 2}{INOVING S.A.S}{2 años}{}
Sistema de demostración de inteligencia artificial para el control de robots móviles en un entorno lúdico

\medskip

\cvsection{Un día de mi vida}

% Adapted from @Jake's answer from http://tex.stackexchange.com/a/82729/226
% \wheelchart{outer radius}{inner radius}{
% comma-separated list of value/text width/color/detail}
\wheelchart{1.5cm}{0.5cm}{%
  6/8em/accent!30/{Dormir},
  3/8em/accent!40/Investigación,
  8/8em/accent!/Daytime job,
  2/10em/accent/Deportes y relajación,
  5/6em/accent!20/Pasar tiempo en familia
}

% use ONLY \newpage if you want to force a page break for
% ONLY the current column
\newpage

\cvsection{Habilidades}

\item Python 60%
\item C++ 35%
\item Git 15%
\item Índole comercial 100%


\switchcolumn

\cvsection{Mi Filosofía de Vida}

\begin{quote}
``El punto de salida hacia todo logro es el deseo''
\end{quote}

\cvsection{Orgullos Significativos}

\cvachievement{\faTrophy}{Emprendimiento Digital LatamDigital 2019.}{AppSC:  – Mejor nueva App.}


\divider

\cvachievement{\faHeartbeat}{Premio Nacional de Ciencia 2020}{Algoritmo de desfragmentación de espectros de redes ópticas elásticas}

\cvsection{Fuertes}

\cvtag{Optimista}
\cvtag{Perfeccionista}\\
\cvtag{Buen Trabajador}

\divider\smallskip

\cvtag{Python}
\cvtag{C++}\\
\cvtag{Estadística y análisis}

\cvsection{Lenguajes}

\cvskill{Inglés}{4}
\divider

\cvskill{Español}{5}
\divider

\cvskill{Francés}{4} %% Supports X.5 values.

%% Yeah I didn't spend too much time making all the
%% spacing consistent... sorry. Use \smallskip, \medskip,
%% \bigskip, \vspace etc to make adjustments.
\medskip

\cvsection{Educación}


\cvevent{Maestría en ingeniería electrónica y computadores}{Universidad de los Andes}{Sept 2017 -- June 2019}{}

\divider

\cvevent{Ingeniería Electrónica}{Universidad de Antioquia}{Sept 2010 -- June 2017}{}

% \divider

\cvsection{Referencias}

% \cvref{name}{email}{mailing address}
\cvref{Prof.\ Juliana Martinez}{Universidad de Antioquia}{juliana.martinez@udea.edu.co}
{Santa Rosa de Osos, Antioquia}

\divider

\cvref{Prof.\ Jorge Aguirre}{Universidad del Cauca}{jorge.aguirre@unicauca.edu.co}
{Popayán, Cauca}


\end{paracol}


\end{document}
