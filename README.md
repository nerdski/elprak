# elprak
%% LyX 2.1.4 created this file.  For more info, see http://www.lyx.org/.
%% Do not edit unless you really know what you are doing.
\documentclass[oneside,english]{scrbook}
\usepackage[T1]{fontenc}
\usepackage[latin9]{inputenc}
\setcounter{secnumdepth}{3}
\setcounter{tocdepth}{3}
\usepackage{float}
\usepackage{url}
\usepackage{graphicx}

\makeatletter

%%%%%%%%%%%%%%%%%%%%%%%%%%%%%% LyX specific LaTeX commands.
\floatstyle{ruled}
\newfloat{algorithm}{tbp}{loa}[chapter]
\providecommand{\algorithmname}{Algorithm}
\floatname{algorithm}{\protect\algorithmname}

\makeatother

\usepackage{babel}
\begin{document}

\title{Electronics lab course}

\maketitle

\part{Short overview of the available tools}


\chapter{Picoscope Oscilloscopes}


\section{Installation and set up}

Oscilloscopes are one of the main tools, if not the most important
for an electrical engineer. A good knowledge of oscilloscopes is mandatory
for any scientist working in a laboratory. Even if he is not directily
involed in the development of electronic devices.


\subsection{Installtion of picoscope on Linux computers}

If you want to use the picoscope on your Linux device, you can install
picoscope 6.0 Beta on your Ubuntu/debian operating system. Make sure
you have a working internet connection.

\begin{algorithm}
sudo bash -c 'echo \textquotedbl{}deb http://labs.picotech.com/debian/
picoscope main\textquotedbl{} >/etc/apt/sources.list.d/picoscope.list'

\caption{Add repository}
\end{algorithm}


\begin{algorithm}
wget -O - http://labs.picotech.com/debian/dists/picoscope/Release.gpg.key
| sudo apt-key add -

\caption{import public key}
\end{algorithm}


\begin{algorithm}
sudo apt-get update \& install picoscope

\caption{update package cache and install}


\end{algorithm}


depending on the type of pico scope you are working with, there's
the need to install different drivers. \url{https://www.picotech.com/downloads/linux}
lists the necessray driver for the module on your workplace

\begin{algorithm}
sudo {[}updater{]} install libps5000a

\caption{Install the required drivers}


\end{algorithm}


Once you have installed picoscope and the drivers you can connect
the hardware to your laptop/tablet. Make shure that you are using
a high speed USB port, as picoscope profits from increased bandwidth.
Also, make shure that you plug in the additional power source of the
picoscope, as some laptops/tablets don't deliver enough power over
USB.

\begin{figure}
\includegraphics[width=0.8\textwidth]{picoscope}

\caption{Workarea of the Picoscope}


\end{figure}

\end{document}
