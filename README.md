# DM50
Corpus of 50 documents relating to the vaccination debate, annotated for modal verb senses

# Annotation Guidelines
This document is to be used as guidelines for annotating the Disneyland Measles (DM50) corpus. The task consists of annotating the senses of the modal auxiliaries \textit{can, could, may, might, must, shall, should} and \textit{ought (to)} in a corpus of 50 documents relating to the vaccination debate, and specifically the measles outbreak in Disneyland in 2015. The permitted senses of the modals are epistemic, dynamic, deontic, optative, concessive and conditional, and shall be covered in greater detail in the following sections.

The motivation behind studying modals is to investigate the way in which people qualify their propositions, exemplified in the following sentence pair:
\begin{enumerate}
\itemsep0em
\item Vaccination \textbf{could} have caused his autism.
\item Vaccination \textbf{must} have caused his autism.
\end{enumerate}

Both sentences qualify the author's perspective on the possibility of vaccinations causing autism (an epistemological stance), however, the former sentence lacks the certainty of the latter. Such unambiguous sentence pairs are not too common in user-generated text however, and senses can frequently overlap or be obscured. The aims of this annotation task are then to analyze and resolve these ambiguous cases in a systematic way. 

Generally, modality can be defined as `a category of linguistic meaning having to do with the expression of possibility and necessity [where] a modalized sentence locates an underlying or prejacent proposition in the space of possibilities' \citep{von2006modality}. In English, modality can be expressed through modal auxiliaries (\textit{should, might, must}), semimodal verbs (\textit{has to, ought to}), adverbs (\textit{perhaps}), and nouns (\textit{possibility}), among others. The present research focuses on modal auxiliaries and the modal senses as described in \citet{ruppenhofer2012yes} (Table \ref{Modal-schema2}). The top row presents the modal auxiliaries that are to be annotated (the markables), and the first column lists the senses (attributes) that apply to each (marked with + to indicate that the sense is permitted, and - to indicate that that sense is not a sense that is to be associated with a particular modal).

\begin{table}[h]
\begin{center}

\begin{tabular}{l|ccccc}
 & \textbf{can/} & \textbf{may/} & \textbf{must} & \textbf{ought} & \textbf{shall/} \\
 & \textbf{could} & \textbf{might} & & & \textbf{should} \\ \hline
 \textbf{epist.} & + & + & + & + & + \\
 \textbf{deon.} & + & + & + & + & + \\
 \textbf{dyn.} & + & - & - & - & - \\
 \textbf{opt.} & - & + & - & - & - \\
 \textbf{conc.} & - & + & - & - & - \\
 \textbf{cond.} & - & - & - & - & + \\
\end{tabular}

\end{center}
\caption{\label{Modal-schema2}Modal senses classification schema used in Ruppenhofer and Rehbein (2012).}
\end{table}

The modal senses of Table \ref{Modal-schema2} are defined according to \citet{ruppenhofer2012yes} as follows: 
\begin{itemize}
{\small
\itemsep0em
\item \textit{Epistemic}: given the state of knowledge, the speaker is compelled to come to a particular conclusion.
\item \textit{Deontic}: this sense relates to what the world should be like, according to a source. It can extend to permission being granted, or an obligation being imposed by a source on an agent. Neither the source nor the agent need to be explicit. 
\item \textit{Dynamic}: this sense concerns the ability or potential for involvement in events or behavior.
\item \textit{Optative}: this special sense of `may' is used when the speaker is communicating a wish, rather than speculating on a state of affairs (epistemic) or granting permission (deontic).
\item \textit{Concessive}: this sense is related to the epistemic sense, but rather than being speculative, the speaker considers the state of affairs to be true. 
\item \textit{Conditional}: commonly occurring in if-clauses, this special sense of `should' is used in cases expressing a condition. 
}
\end{itemize}

The modal sense scheme was chosen because results from \citet{ruppenhofer2012yes} indicate that the sense categories are meaningful and can be learned by a classifier. In applying their scheme to a different domain (the vaccination debate), analyzing the outcomes of the present annotation task and comparing them to results of \citet{ruppenhofer2012yes} should help answer the following research questions: (i) whether there is comparable inter-annotator agreement between the two differing domains (English news and the vaccination debate), and (ii) whether there are unique cases of disagreement when comparing the present results with those of \citet{ruppenhofer2012yes}. The following sections outline specific instructions for the annotators, and provide annotated examples. 

\subsection*{Instructions for annotators}
The DM50 corpus contains 50 articles relating to the vaccination debate. The modals \textit{can, could, may, might, must, shall, should} and \textit{ought (to)} are the markables, and their attributes are the permitted senses as presented in Table \ref{Modal-schema2}. An additional attribute has been created for cases of uncertainty (`ambiguous'), but it is not to be used too liberally (i.e. frequently and without restraint).

All modals are to be annotated, with the exception of those appearing in headings and subheadings, and sections encouraging correspondence with the author (e.g. `you can find me on Twitter'). Negation is beyond the scope of this task, and modals that appear in the negated form are to be annotated without the negative particles, as follows: `I [\textbf{can}]'t come'; `I [\textbf{should}]n't call at this time'; and `She [\textbf{can}]not believe you said that'.

The annotation software used for the present task is eHOST. See http://ehostdoc.com for software documentation.

\subsection*{Annotated examples}

Table \ref{table: annotation examples} presents examples of correct annotation (where the target modal is in bold font), with a brief explanation of the sense.

\begin{table*}[th]
\centering
{\small
\begin{tabular}{l p{5cm} p{7cm}}
\textbf{Sense} & \textbf{Example} & \textbf{Description} \\ \hline 
Epistemic & He got autism straight after he was vaccinated. It \textbf{must} be the vaccine. & Considering the evidence (correlation of onset of autism and vaccination), we can infer that vaccination caused his autism. (Note that this is epistemic modality regardless of logical fallacies.) \\
Deontic & Infants \textbf{must} receive the MMR vaccine between 8-12 months. & Implicit agents have the obligation to vaccinate their children between 8-12 months of age. \\
Dynamic & Not all people \textbf{can} get vaccinated. & Some people are not able to get vaccinated. In this case it is due to immuno-compromisation or some other physical attribute -- not because of permission (that would be deontic). \\
Optative & Long \textbf{may} she live. & The author expresses a wish that she lives a long life. \\
Concessive & Harmful as they \textbf{may} be, it is still better to vaccinate than not. & Similar to epistemic modals, but here the author considers vaccination to be better than the alternative, and that it is a given rather than a possibility. \\
Conditional & \textbf{Should} you refuse to vaccinate your child, they will not be permitted to enter public school. & The penalty of refusing to vaccinate your child is that they are refused entry to public school.\\
\end{tabular}
}
\caption{Examples of the different modal senses in context with a description.} \label{table: annotation examples}
\end{table*}
