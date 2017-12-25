# paper
\documentclass[9pt,twocolumn,twoside]{optica}
\setboolean{shortarticle}{true}
\setboolean{minireview}{false}

\title{Temporal signal concealing and revealing with the variety of sum-frequency generation}

\author[1]{Yi'an Liu}
\author[1,*]{Yuping Chen}
\author[1]{Haowei Jiang}
\author[1]{Guangzhen Li}
\author[1]{Licheng Ge}
\author[1,*]{Xianfeng Chen}

\affil[1]{State Key Laboratory of Advanced Optical Communication Systems and Networks,
Department of Physics and Astronomy, Shanghai Jiao Tong University,
800 Dongchuan Road, Shanghai 200240, China
}

\affil[*]{Corresponding author: ypchen@sjtu.edu.cn; xfchen@sjtu.edu.cn}

% To be edited by editor
% \dates{Compiled \today}

\ociscodes{(140.3490) Lasers, distributed feedback; (060.2420) Fibers, polarization-maintaining; (060.3735) Fiber Bragg gratings.}

% To be edited by editor
% \doi{\url{http://dx.doi.org/10.1364/optica.XX.XXXXXX}}

\begin{abstract}
Recent research has been focused on temporal cloaking that mainly works by creating a gap in spatial-time domain. In this work, we theoretically and experimentally present a way to conceal and reveal optical signal in time domain based on the variety of sum-frequency generation. The temporal signal carried by optical pulse turned into continuous wave with constant intensity in the concealing process. When the continuous wave was received by users, optical pulse was restored in the revealing process. The conversion between pulse and continuous wave was related to sum-frequency generation. The temporal signal was transmitted privately in consideration of the variety of sum-frequency generation.
\end{abstract}

\setboolean{displaycopyright}{true}

\begin{document}

\maketitle

\section{INTRODUCTION}
The idea of temporal cloaking\cite{mccall2010spacetime} is analogous to spatial cloaking\cite{gabrielli2009silicon,valentine2009optical,li2008hiding} and becomes popular in recent years. The original temporal cloaking works in a time gap and aims to conceal events. With a time gap created by time lens and dispersive medium, temporal cloaking has been firstly demonstrated in optical fibers\cite{fridman2012demonstration}. Then temporal cloaking for a telecommunication optical pulse is demonstrated with periodic time gap obtained by fractional Talbot effect\cite{lukens2013temporal}. The aim of these temporal cloaking is to achieve walk-off between probe beam and events in time-spatial domain, and these temporal cloaking can only conceal events in finite time gap. From another point of view, by controlling the four-wave mixing process of probe beam and events in fiber, an infinite temporal cloaking is obtained\cite{bony2014temporal} but it fails easily when the condition of interaction between probe beam and events is corrected. In this paper, temporal cloaking is achieved by control the sum-frequency generation(SFG) between probe beam and events(or signal). Furthermore, a protocol of signal concealing and revealing which is similar to BB84 protocol\cite{bennett2014quantum} in quantum key distribution is designed ensuring the reliability of temporal cloaking.
\section{PRINCIPLE AND METHODS}
The schematic of temporal signal concealing and revealing is depicted in Figure.1. A sender intended to transmit some information to user which was contained in an optical pulse train. However, a spy could filch the information easily if the sender transmitted information to receiver directly. Therefore, the sender transformed the pulse train into continuous wave(CW) using SFG with quasi-phase matching(QPM) in periodically poled lithium niobate(PPLN)\cite{zhang2008flexible,gong2010all,lu2008all,chen2006type} and this step is called temporal signal concealing. According to the intensity of the optical pulse train, the sender selected signal beam and pump beam with horizontal or vertical state of polarization(SOP) in each time interval. After the SFG process, the idler beam was detected by photoelectric detection and the electric intensity contained the same information as the optical pulse train did. As a result, the information contained in optical pulse train was concealed into continuous signal beam. Then the sender transmitted the signal beam to the user directly without any disguise. When the signal beam was obtained by the user, pump beam with randomly horizontal or vertical SOP was selected and SFG process in PPLN with the same poled period as the sender's was carried out. The user's idler beam was also detected by photoelectric detection. The following step is called pump checking. In this step, the user reported the SOP of his pump beam to the sender and the sender then informed the user in which time intervals their SOP of pump beam was coincident, in other word, in which time intervals user's SOP of pump beam was 'correct'. The last step is called temporal signal revealing. The user reserved those 'correct' pump beam and the corresponding electric intensity of idler beam of his SFG process. After this step, the information that the sender was prepared to transmit was revealed from continuous signal beam. Finishing three steps above, information contained in an optical pulse train was transmitted from sender to user privately.
\begin{figure}[htbp]
\centering
\includegraphics[width=\linewidth]{schematic}
\caption{Schematic of temporal signal concealing and revealing. The information is the electric intensity of sender’s idler beam. Sender selected signal beam for sum-frequency generation and he got the electric intensity of idler beam which detected by optical-electric detector. Then signal beam was sent to user in fiber which is called signal transportation. And the SOP of pump beam was delivered from sender to user in classic channel.
}
\label{fig:schematic}
\end{figure}
In consideration of different types of SFG, four modes for temporal signal concealing and revealing are shown in Figure.2. For example in Figure.2(a), the horizontal or vertical SOP is expressed as 'o' or 'e' which means ordinary or extraordinary light defined according to the orientation of crystal axis of PPLN. And the type of SFG 'o + e -- 1' means the electric intensity of idler beam is '1' if pump beam is 'e' and signal beam is 'o'. And pump, signal as well as idler beam are labeled in green, red and yellow respectively. The sender and user shared the signal beam while had different pump beam. The last two rows show the results of pump checking and the information transmitted eventually. Let us suppose that a spy wanted to filch the information. Clues that the spy could obtain was signal beam, user's pump beam and the results of pump checking. However, if the type of SFG was unknown to the spy, these clues could not contribute to information decode for the spy. Moreover, when information was transmitted using all the four modes with certain order that only the sender and user were aware of, as is shown in Figure.1, it would be more complicated for the spy to filch the information. It is the variety of SFG that ensures the privacy of the temporal signal concealing and revealing process.
\begin{figure}[htbp]
\centering
\fbox{\includegraphics[width=\linewidth]{table1a}}
\fbox{\includegraphics[width=\linewidth]{table1b}}
\fbox{\includegraphics[width=\linewidth]{table1c}}
\fbox{\includegraphics[width=\linewidth]{table1d}}
\caption{Four modes of signal concealing and revealing between sender and receiver. Mode I is based on type II SFG and has idler output when pump is ordinary light and signal is extraordinary light. Mode II is also based on type II SFG but has contrary SOP of pump and signal. Mode III and Mode IV are based on type I SFG with different SOP of pump and signal.}
\label{fig:mode}
\end{figure}
\section{SIMULATION AND EXPERIMENT}
In this investigation, we simulate each type of SFG related to the four modes for temporal signal concealing and revealing, as is shown in Figure.4(a)-(d). From the results of simulation we find that 'e + e -- e' SFG(type 0 SFG) and 'o + o -- e' SFG(type I SFG) are convenient for experiment in communication band, mainly because of the poled period of PPLN in our laboratory. For type 0 SFG, we select PPLN with 19.6$\mu$m poled period and environment temperature 50$^\circ$C. The wavelength of pump beam and signal beam are 1554.1nm and 1556.2nm, with power of 10mW at input. The spectrum is shown in Figure.5(a). The middle peak with the highest level is the idler beam of SFG and the other two peaks beside are second-harmonic generation(SHG) of pump beam and signal beam. Figure.5(b) shows the type I SFG. The wavelength of pump beam and signal beam is 1553.8nm and 1563nm respectively with 10mW at input. The dashed line is the simulation of broadband SFG\cite{li2017broadband} calculated with Sellmeier equation\cite{gayer2008temperature}. AS for type II SFG, there is no experiment in our investigation.
\begin{figure}[htbp]
\centering
\includegraphics[width=\linewidth]{simandexp}
\caption{Simulation results of different types of SFG and the spectrum of 'e + e --e' SFG and 'o + o -- e' SFG. (a) is 'e + e -- e' SFG and the poled period of PPLN is 19.6$\mu$m as well as the temperature is 50$^\circ$C. The bright line is related to proper wavelength of pump and signal beam for SFG. (b) is 'o + o -- e' SFG on condition that the poled period of PPLN is 20.3$\mu$m and the temperature is 25.1$^\circ$C. The proper wavelength of pump and signal beam can be chosen in a broad region which refers to broad band SFG. (c) The pump beam is at 1554.1nm with power of 9.94mW and the signal beam is at 1556.2nm and 10.32mW. The idler beam is at 777.5nm observed from the spectrum. (d) The pump beam and signal beam is at 1553.8nm and 1563nm respectively with power of 50mW. The dashed line shows the simulated broadband type I SFG.}
\label{fig:simandexp}
\end{figure}
As is introduced in former part, each one of the four modes of signal concealing and revealing is able to deliver information privately. Here we choose the forth mode to deliver a pulse train. Figure.6 shows the setup of our experiment. The setup mainly consists of two parts, sender and user. The pump beam is given by two tunable lasers at 1553.8nm and the SOP of pump beam is adjusted by polarization switch which is triggered by square wave from function generator. The signal beam is at 1563nm from tunable laser. All pump and signal beams are enhanced by erbium doped fiber amplifier(EDFA) before inserting PPLN to ensure the power of idler beam. We firstly observe the spectrum of SFG, then we detect the electric intensity of idler beam using photoelectric detection. The results of intensity detection of pump beam and idler beam are shown in Figure.7. The pump beam is continuous wave with SOP varying over time. We put a polarization beam spliter(PBS) between the fiber collimator and detector before the placement of lens, PPLN and filter. Ordinary light is able to pass through the PBS while extraordinary light is reflected. Therefore, from the fluctuation of intensity we know the SOP of sender's and user's pump beams. The idler beam has time-dependent intensity so it can be detected with photoelectric detection directly. Figure.8 shows the process of signal concealing and revealing with the forth mode. It is obvious that the pulse train is successfully delivered from sender to user.
\begin{figure}[htbp]
\centering
\includegraphics[width=\linewidth]{setup}
\caption{The setup of the experiment. Sender and receiver shared the signal beam. And the state of polarization(SOP) of pump beam was adjusted by polarization switch. The state of polarization is controlled by a polarization switch which is triggered with function generator. Both sender’s and user’s idler beams are detected and recorded with optical-electric detector and oscilloscope. The filter in the setups is used to exclude pump beam and signal beam.}
\label{fig:setup}
\end{figure}
\begin{figure}[htbp]
\centering
\includegraphics[width=\linewidth]{pumpchecking}
\caption{The results of intensity detection of both pump beam and idler beam. The signal concealing and revealing mode chosen in experiment is the third mode as is introduced in Figure.2. The pump checking progress ensured that User chose the correct time parts and got the inverted code.}
\label{fig:result}
\end{figure}
\begin{figure}[htbp]
\centering
\fbox{\includegraphics[width=\linewidth]{table2}}
\caption{The process of signal concealing and revealing with the forth mode.}
\label{fig:result}
\end{figure}
\section{CONCLUSION}
In this work, we present a scheme for temporal signal concealing and revealing and then successfully delivered temporal pulse train privately. The deficiency is not all of four modes which we design in principle are achieved in experiment, especially type II SFG. And the code rate of signal is not high enough in view of the key point of this work is introducing the principle of temporal signal concealing and revealing. We plan to improve our work in such aspects above and we hope this scheme of temporal signal concealing and revealing will be applied in the field of communication and information security.
\section{Funding Information}
National Natural Science Foundation of China (NSFC) (11574208, 61235009)\; National Key R\&D Program of China (2017YFA0303700).
\section{Acknowledgments}
The authors thank Tong Xiang for technical support.
\section{References}
\bibliographystyle{elsarticle-num}
\bibliography{ref}
\end{document} 
