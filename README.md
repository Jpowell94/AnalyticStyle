
## What is Analytic Style?

This repository contains files for my stylometric analysis of a corpus I created, containing a subset of the analytic philosophy canon, a textual tradition beginning with the work of Gotlob Frege (1848-1925), Betrand Russell (1872-1970), G.E. Moore (1873-1958), and Ludwig Wittgenstein (1889-1951), and ending with the works of English language philosophers in the late 1950's early 1960's, togther with a subset of the continental philosophical canon, (see "*Continental Philosophy: A Very Short Introduction*". Critchley, Simon. 2001), understood as the sum of: 

  1. German Idealism, British Idealism, and Romanticism. 
  2. The critics of metaphysics and "masters of suspicion" including Feuerbach, Marx, Nietzsche,                 Freud, Bergson, and so on. 
  3. Germanophone phenomenology and existential philosophy, (Husserl, Max Scheler, Karl Jaspers, and             Heidegger). 
  4. French phenomenology, Hegelianism, and anti-Hegelianism (some of whome are also called                      "Existentialists") including Kojève, Sartre, Merleau-Pont, Levinas, Bataille, and Simon de Beauvoir,        among others. 
  5. Hermeneutics (Dilthey, Gadamer, Ricoeur) 
  6. Western Marxism, the Frankfurt school, including Lukacs, Benjamin, Horkheimer, Adorno,                      Marcuse, Habermas, etc. 
  7. French Structuralism and structuralism, including Lévi-Strauss, Lacan, and Althusser 
  8. Post-Structuralism, exemplified in the works of Foucault, Derrida, and Deleuze 
  9. "Post-modernism" here meant to refer to the work of Lyotard, and Baudrillard at least. 
  10. Feminism, typofied by thinkers like Irigaray, and Kristeva.

In particular, I chose the works I deemed to be most appropriate and most representative of those authors for which we have real evidence to believe that they were or perceived themselves to be in conflict. I focused on 9 historical instances of debate or conflict to choose my authors:
  
  1. The debate between Frege and Husserl over the nature of logic and arithmetic.
  2. The debates between Moore and Russell and the British Idealists.
  3. The debate between Russell and Bergson.
  4. The disagreement beween Heidegger and Carnap over metaphysics.
  5. The disagreements between Horkheimer and the Critical School, and the Logical Positivists in the Vienna      Circle and Berlin Circle groups.
  6. Karl Popper's attacks on "Historicism" and "pseudo-science", which he saw as prototypical                   examples the works of Marx, Freud, and Theodor Adorno.
  7. The 1958 Royaumont Colloquium, concerning Ryle, Quine, and Mearleu-Ponty (among others).
  8. The dispute between John Searle and Derrida concerning the correct interpretation of J.L.                   Austin.
  9.[The televized debate](https://www.youtube.com/watch?v=7TUD4gfvtDY) between Foucault and Chomsky on         Human Nature.
  
  
My analysis consisted in using various stylometric functions and methods of analysis found in [**stylo**](https://journal.r-project.org/archive/2016/RJ-2016-007/index.html)(Eder, M., Rybicki, J. and Kestemont, M. 2016), such as the Zeta metric and related extensions to identify discriminating words between the two sets of texts, various principle component analysis done on a set of 26 texts and 17 authors, building a bootstrap consensus tree, and various text analysis functions such as Heirarchical Clustering analysis on the documents, and measuring keyness, using metrics such as term frequency-inverse document frequency, and so on. (see ["Text Mining with R"](https://www.tidytextmining.com/))


The project was inspired by Javier Virués-Ortega's paper "The Case Against B.F. Skinner 45 years Later: An Encounter with N. Chomsky" ( see [Virués-Ortega 2006](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC2223151/)), in which a footnote identified a large body of scientometric work that challenges Chomsky's history of [the decline of behaviorism](https://en.wikipedia.org/wiki/Verbal_Behavior#Chomsky's_review), and also the traditional cultural myth told about it within psychology, linguistics, and philosophy departments. I felt that something similar could be done concerning the cultural myths told in philosophy departments about the "Analytic-Continental Divide", though using **stylometric**, rather than scientometric data in its most general sense.

#Acknowledgements

I would like to recognize the Digital Scholars group at Florida State University, particularly those brilliant people of whom it was made up of in the Spring semester of 2019, for providing the catalyst for this project, and whose feedback was invaluable impetus towards the final character of my work and thoughts about this matter. I would also like to thank Tarez Graban in particular for advising me on this project along the way, without whose guidance I would have been lost.

#Context
## The Analytic Tradtion
The tradition began with an act of revolution on the part of Russel and Moore against the British Idealist philosophy of T.H. Green (1836-1882), F. H. Bradley (1846-1924), Bernard Bosanquet (1848-1923), and as Russell sees it, "Against both Kant and Hegel." What made the new philosopht of Russell and Moore was a commitment to a particular metaphilosophical belief, that "all sound philosophy should begin with an *analysis of propositions*," which meant something slightly different to both Russell and Moore. The method of philosophy eventually formulated so as to capture both men's projects, was one in which philosophy is seen as having as its central task the offering of explanations and clarifications about the nature of various parts of language, by way of various other linguistic devices, with the languages of formal logic playing a central and uniquely important role in the explanatory process. This is drastically different from what was taken to be the uniting central task of traditional philosophy up to that point, that being the formulation of a *logos* of the world, a rationally coherent account of reality at the level of utmost generality; of reality as a totality. Thus, coming to be concerned with explaining facts about language and not "capital R Reality", the turn to analytic philosophy is sometimes refered to as the *Lingustic Turn*.

In time this approach to philosophy became the unquestionable dominant metaphilosophical position of English speaking philosophy departments the world over, a position it enjoyed without devitation until the 1960's, when multiple camps within the movement began to disagree with one another over deep and central issues related to the nature of language, over scientific knowledge and practice, and the analytic methods themselves, and hence the nature of philosophy. Today, almost noone working in a English speaking philosophy department and publishing in English philosophy journals would consider themselves adherents to the positions of Russell, or Moore, or Wittgenstein, and with the defining feature of this present era sometimes being identified with its ecclectisism and philosophical pluralism, there is a sense in which we are in a "post-analytic" stage.

There are two issues with describing English philosophy as post-analytic though. The first is that it is not a label used by most philosophers, journals, and philosophical associations to describe themselves or what it is that they do. [There are more assocations of analytic philosophy today then there have ever been before](http://www.dif.unige.it/esap), and it is practiced more and more in non-english philosophical communities. Clearly then, we have not moved past being analytic in the sense that we still prefer to call ourselves analytic. The second issue is more interesting and formed part one part of the motivation for this project. It is clear also that if we mean for post-analytic to denote a particular "ism", in manner similar to something like post-Helianism would, then there is no "ism" associated with post-analytic philosophy. Philosophers calling themselves analytic hold a wide variety of competing beliefs about central philosophical issues, and whats more, they are not particularly good at guessing what the most popular positions taken by their peers are,as was shown by David Bourget and David Chalmers in their [Philpapers survey and metasurvey](https://philpapers.org/surveys/). Again it seems clear that there just is no one thing to be called post-analytic philosophy or analytic philosophy understood as a particular doctrine or set of beliefs today. 

So why do they call themselves analytic, and what do they mean? Of the kinds of answers typically given, two are the ones this project was concieved of as scrutinizing: what I will call the **the stylistic answer**, is the that analytic philosophy today is any philosophy written in a particular style, called the **analytic style**. 

##Analytic Style?
Under a naive conception of analytic style, it is supposed to be characterized by the unique level of emphasis it places on **argumentation, clarity, and rigour**, in comparison to "non-analytic" philosophy. But history tells us that none of these three features are distinctive of analytic philosophy. Argumentation has always been emphasized in philosophy; Wittgenstein, unquestionably one of the most influential authors in the analytic tradition, was called a mystic by Carnap, his works requiring a great deal of interpretation and to this day reasonable disagreements are had about what he really meant in works like the *Philosophical investigations*; Husserl argued that philosophy is a "rigorous science", where his phenomenological definition of rigour is as similar to any one analytic definition as any two of them are to each other.

Never the less, even among those philosophers who recognize all the points just made, their belief in a distinctive analytic style does not waiver, even though now they may find it difficult or even impossible to say exactly what such a style consists of! However, the above mentioned *positive* characterization of analytic style has a *negative* characterization with which it correlates; whatever analytic style is, it is often believed that it is certain that there is one thing it is *not*, and that is what gets called **Continental philosophy**.

##Continental Style?
If Analytic Philosophy broke with the traditional philosophy in taking its linguistic turn, we might say roughly that Continental Philosophy comprises all that philosophy that *did not* take such a turn, at least the same kind or at the same time that analytic philosophy did. Instead we might say it took a **phenomenalogical** turn. The work of Edmnund Husserl (1859-1938) is usually given as the definitive birthplace of phenomenology and the continental tradition. Phenomenology as Husserl understood it was a method for sustained attempts at offering descriptions of both our experiences and the "things themselves". As is evident from my definition of what counts as the Continental tradition, it has very nearly always found itself in an ecclectic era, such that the same issues we had with identifying a single post-analytic philosophy will likewise prevent us from considering any singular continental philosophy, even though just like the term "analytic philosophy" and "analytic philosopher", "continental philosophy" and "continental philospher" are widely-used and prefered professional self-descriptions by philosophers today, even if they do not, nor have they ever been, living on the continent of Europe (Critchley 2001, pg. 37-47). Continental Philosophy has had a tremendous influence on the present state of many humanities and social sciences departments in the United States, save for philosophy:

> ...[Continental Philosophy] has decisibely influenced many theoretical innovations in the humanities and social sciences: in literary theory, art history and theory, social and political theory, cultural studies, historiography, religious studies, and anthropology, not to mention debates in fine art, architecture, feminism, and psychoanalysis. (Critchley 2001, pg. 41)

So much influence, that the fact that philosophers working in the analytic tradition would label people like Derrida "Pseudo-philosophers" and writing an [open letter in protest](http://ontology.buffalo.edu/smith/varia/Derrida_Letter.htm) of him being awarded an honorary degree from Cambridge is rather interesting, and highly telling about the relationship between not just analytic and continental philosophy, but analytic philosphy and the humanities as a whole. (He was still awarded his degree by a vote fo 336 to 204, almost none of the votes in favor, according to [Sarah Richmond](https://doi.org/10.1111/j.1468-0378.1996.tb00064.x), were from members of the philosophy department!) It would thus be a desirata of a characterization of analytic style in terms of its difference from "continental style", that these differences help illuminate why continental work has found purchase with so many different people and fields. 

 
##Method
#Selecting Disciminative Features

To Analyze style, I focused on various measure I can perform on the **most frequent words**, equating document specific word frequency rankings with **author invariants**, linguistic items that are the same across documents in virtue of their being written by the same author, and that are not characteristic of documents not written by an author. In particular, I use the **Craig's Zeta** measure to identify a statistically significant difference in feature distribution between the analytic part of my corpus and the Continental part of my corpus, which I have labled the "Humanities" portion instead. According to Eder , Rybicki and, Kestemont in "Stylometry with R: A Package for Computational Text Analysis", 

>[The Craig Zeta metric] is popular for selecting discriminative stylometric features in a binary classification setting." (pg. 117)

in other words, by using the "oppose()" function in stylo, we can identify significant feature variantion between our subcorpora, and thus identify a set of most **discriminating** words, that is, words that are most characterstics of being analytic or not. This measure will fulfill the goal I outlined above of identifying a specific way in which Analytic style is not continental style, a short set of words that analytic writers prefer together with a set of words that they *avoid*, i.e. the words most characterstic of Continental writing. Thus my major results and contribution of this project will be this set of words most prefered by Analytic writers in contrast to Continental writers, and words most avoided in contrast to Continental writers.

#preprocessing
First we take all of the documents I have put together, and we treat all of the self-identified analytic authors as *one and the same* author, and similarly for the Continental authors. This allows me to treat all of the documents written by the various authors in my corpus as being written by one of two people, and then by running well established tests for checking differences between two authors, I can establish differences between two sets of authors.

Then we *tokenize* each document, seperating them into the words that they contain as parts.

All that is left is to calculate the Craig Zeta.

#Bootstrapping: A Test of MFW's effectiveness

I will quickyl demonstrate why you should trust these methods and consider most frequent words to adequately capture features of authorship by building a **bootstrapping consensus tee** from my documents. Bootstrapping consesus trees are consensus trees built using a distance metric, where a consesus tree is a way of estimating the level of "support" for claudes in a tree, clusters of nodes of the tree.

![Consensus trees](/Users/jesserussellpowell/analyticstyle/ConesensusTreeDiagram.jpg) 

Consensus trees work by taking multiple different tree diagrams/ cladograms, where the have all the same nodes, but have them grouped differently, and producing the tree that has groupings that *best approximate* the two alternative groupings for each grouping of nodes in each tree.



##Findings

