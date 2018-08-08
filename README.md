# DM50
Corpus of 50 documents relating to the vaccination debate, annotated for modal verb senses

# Annotation Guidelines
This document is to be used as guidelines for annotating the Disneyland Measles (DM50) corpus. The task consists of annotating the senses of the modal auxiliaries *can, could, may, might, must, shall, should and ought (to)* in a corpus of 50 documents relating to the vaccination debate, and specifically the measles outbreak in Disneyland in 2015. The permitted senses of the modals are epistemic, dynamic, deontic, optative, concessive and conditional, and shall be covered in greater detail in the following sections.

The motivation behind studying modals is to investigate the way in which people qualify their propositions, exemplified in the following sentence pair:

- Vaccination **could** have caused his autism.
- Vaccination **must** have caused his autism.

Both sentences qualify the author's perspective on the possibility of vaccinations causing autism (an epistemological stance), however, the former sentence lacks the certainty of the latter. Such unambiguous sentence pairs are not too common in user-generated text however, and senses can frequently overlap or be obscured. The aims of this annotation task are then to analyze and resolve these ambiguous cases in a systematic way. 

Generally, modality can be defined as ''a category of linguistic meaning having to do with the expression of possibility and necessity [where] a modalized sentence locates an underlying or prejacent proposition in the space of possibilities'' (Von Fintel, 2006). In English, modality can be expressed through modal auxiliaries (*should, might, must*), semimodal verbs (*has to, ought to*), adverbs (*perhaps*), and nouns (*possibility*), among others. The present research focuses on modal auxiliaries and the modal senses as described in Ruppenhofer and Rehbein (2012), Table 1. The top row presents the modal auxiliaries that are to be annotated (the markables), and the first column lists the senses (attributes) that apply to each (marked with + to indicate that the sense is permitted, and - to indicate that that sense is not a sense that is to be associated with a particular modal).

| **can/could**| **may/might** | **must** | **ought** | **shall/shall** | 
|---|---|---|---|---|
| **epist** | + | + | + | + | + |
| **deon.** | + | + | + | + | + |
| **dyn.** | + | - | - | - | - |
| **opt.** | - | + | - | - | - |
| **conc.** | - | + | - | - | - |
| **cond.** | - | - | - | - | + |


Table 1: Modal senses classification schema used in Ruppenhofer and Rehbein (2012).


The modal senses of Table 1 are defined according to Ruppenhofer and Rehbein (2012) as follows: 

- *Epistemic*: given the state of knowledge, the speaker is compelled to come to a particular conclusion.
- *Deontic*: this sense relates to what the world should be like, according to a source. It can extend to permission being granted, or an obligation being imposed by a source on an agent. Neither the source nor the agent need to be explicit. 
- *Dynamic*: this sense concerns the ability or potential for involvement in events or behavior.
- *Optative*: this special sense of 'may' is used when the speaker is communicating a wish, rather than speculating on a state of affairs (epistemic) or granting permission (deontic).
- *Concessive*: this sense is related to the epistemic sense, but rather than being speculative, the speaker considers the state of affairs to be true. 
- *Conditional*: commonly occurring in if-clauses, this special sense of 'should' is used in cases expressing a condition. 



The modal sense scheme was chosen because results from Ruppenhofer and Rehbein (2012) indicate that the sense categories are meaningful and can be learned by a classifier. In applying their scheme to a different domain (the vaccination debate), analyzing the outcomes of the present annotation task and comparing them to results of Ruppenhofer and Rehbein (2012) should help answer the following research questions: (i) whether there is comparable inter-annotator agreement between the two differing domains (English news and the vaccination debate), and (ii) whether there are unique cases of disagreement when comparing the present results with those of Ruppenhofer and Rehbein (2012). The following sections outline specific instructions for the annotators, and provide annotated examples. 

**Instructions for annotators:**

The DM50 corpus contains 50 articles relating to the vaccination debate. The modals *can, could, may, might, must, shall, should* and *ought (to)* are the markables, and their attributes are the permitted senses as presented in Table 1. An additional attribute has been created for cases of uncertainty ('ambiguous'), but it is not to be used too liberally (i.e. frequently and without restraint).

All modals are to be annotated, with the exception of those appearing in headings and subheadings, and sections encouraging correspondence with the author (e.g. 'you can find me on Twitter'). Negation is beyond the scope of this task, and modals that appear in the negated form are to be annotated without the negative particles, as follows: 'I [**can**]'t come'; 'I [**should**]n't call at this time'; and 'She [**can**]not believe you said that'.

The annotation software used for the present task is eHOST. See http://ehostdoc.com for software documentation.

**Annotated examples:**

Table 2 presents examples of correct annotation (where the target modal is in bold font), with a brief explanation of the sense.


| **Sense** | **Example** | **Description** | 
|---|---|---|
| Epistemic | He got autism straight after he was vaccinated. It **must** be the vaccine. | Considering the evidence (correlation of onset of autism and vaccination), we can infer that vaccination caused his autism. (Note that this is epistemic modality regardless of logical fallacies.) |
| Deontic | Infants **must** receive the MMR vaccine between 8-12 months. | Implicit agents have the obligation to vaccinate their children between 8-12 months of age. |
| Dynamic | Not all people **can** get vaccinated. | Some people are not able to get vaccinated. In this case it is due to immuno-compromisation or some other physical attribute -- not because of permission (that would be deontic). |
| Optative | Long **may** she live. | The author expresses a wish that she lives a long life. |
| Concessive | Harmful as they **may** be, it is still better to vaccinate than not. | Similar to epistemic modals, but here the author considers vaccination to be better than the alternative, and that it is a given rather than a possibility. |
| Conditional | **Should** you refuse to vaccinate your child, they will not be permitted to enter public school. | The penalty of refusing to vaccinate your child is that they are refused entry to public school.|

Table 2: Examples of the different modal senses in context with a description.

