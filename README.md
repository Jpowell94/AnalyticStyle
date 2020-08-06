
## What is Analytic Style?

This repository contains all the necessary files for a stylometric analysis of my hand-picked philosophy corpus, along with the results. The corpus contains a subset of the analytic philosophical canon —a textual tradition beginning with the work of Gottlob Frege (1848-1925), Bertrand Russell (1872-1970), G.E. Moore (1873-1958), and Ludwig Wittgenstein (1889-1951), and ending with the works of English language philosophers in the late 1950's early 1960's, The work of W.V.O. Quine, and the work of Noam Chomsky— together with a subset of the continental philosophical canon, (see *Continental Philosophy: A Very Short Introduction*. Critchley, Simon. 2001), understood to be the sum of at least the following philosophical traditions: 

  1. German Idealism, British Idealism, and Romanticism.
  2. The critics of metaphysics and "masters of suspicion" including Feuerbach, Marx, Nietzsche, Freud, Bergson, and so on.
  3. Germanophone phenomenology and existential philosophy, (Husserl, Max Scheler, Karl Jaspers, and Heidegger).
  4. French phenomenology, Hegelianism, and anti-Hegelianism (some of whom are also called "Existentialists") including Kojeve, Sartre, Merleau-Ponty, Levinas, Bataille, and Simon de
     Beauvoir, among others.
  5. Hermeneutics (Dilthey, Gadamer, Ricoeur)
  6. Western Marxism, the Frankfurt school, including Lukacs, Benjamin, Horkheimer, Adorno, Marcuse, Habermas, etc.
  7. French Structuralism and structuralism, including Levi-Strauss, Lacan, and Althusser
  8. Post-Structuralism, exemplified in the works of Foucault, Derrida, and Deleuze
  9. "Post-modernism" here meant to refer to the work of Lyotard, and Baudrillard at least.
  10. Feminism, typified by thinkers like Irigaray, and Kristeva.


In particular, I chose the works I deemed to be most appropriate and most representative of those pairs of authors/ author sets which we have real evidence to believe were or perceived themselves to be in conflict. I focused on 9 historical instances of debate or conflict to choose my authors:
  
  1. The debate between Frege and Husserl over the nature of logic and arithmetic.
  2. The debates between Moore and Russell and the British Idealists.
  3. The debate between Russell and Bergson.
  4. The disagreement between Heidegger and Carnap over metaphysics.
  5. The disagreements between Horkheimer and the Critical School, and the Logical Positivists in the Vienna Circle and Berlin Circle groups.
  6. Karl Popper's attacks on "Historicism" and "pseudo-science", which he saw as prototypical examples the works of Marx, Freud, and Theodor Adorno.
  7. The 1958 Royaumont Colloquium, concerning Ryle, Quine, and Merleau-Ponty (among others).
  8. The dispute between John Searle and Derrida concerning the correct interpretation of J.L. Austin.
  9. The [televized debate](https://www.youtube.com/watch?v=7TUD4gfvtDY) between Foucault and Chomsky on Human Nature.
  
  
My analysis consisted in using various stylometric functions and methods of analysis found in [**stylo**](https://journal.r-project.org/archive/2016/RJ-2016-007/index.html) (Eder, M., Rybicki, J. and Kestemont, M. 2016), such as the Zeta metric and related extensions to identify discriminating words between the two sets of texts, various principle component analysis done on a set of 26 texts and 17 authors, building a bootstrap consensus tree, and various text analysis functions such as Hierarchical Clustering analysis on the documents, and measuring keyness, using metrics such as term frequency-inverse document frequency, and so on. (see ["Text Mining with R"](https://www.tidytextmining.com/))


The project was inspired by Javier Virues-Ortega's paper "The Case Against B.F. Skinner 45 years Later: An Encounter with N. Chomsky" ( see [Virues-Ortega 2006](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC2223151/)), in which a footnote identified a large body of scientometric work that challenges Chomsky's history of [the decline of behaviorism](https://en.wikipedia.org/wiki/Verbal_Behavior#Chomsky's_review), and also the traditional cultural myth told about it within psychology, linguistics, and philosophy departments. I felt that something similar could be done concerning the cultural myths told in philosophy departments about the "Analytic-Continental Divide", though using stylometric, rather than scientometric data in its most general sense.

# Acknowledgements

I would like to recognize the Digital Scholars group at Florida State University, particularly those brilliant people of whom it was made up of in the Spring semester of 2019, for providing the catalyst for this project, and whose feedback was invaluable impetus towards the final character of my work and thoughts about this matter. I would also like to thank Tarez Graban in particular for advising me on this project along the way, without whose guidance I would have been lost.

# Context
## The Analytic Tradition
The tradition began with an act of revolution on the part of Russel and Moore against the British Idealist philosophy of T.H. Green (1836-1882), F. H. Bradley (1846-1924), Bernard Bosanquet (1848-1923), and as Russell sees it, "Against both Kant and Hegel." What made the new philosophy of Russell and Moore was a commitment to a particular metaphilosophical belief, that "all sound philosophy should begin with an **analysis of propositions**," which meant something slightly different to both Russell and Moore. The method of philosophy eventually formulated so as to capture both men's projects, was one in which philosophy is seen as having as its central task the offering of explanations and clarifications about the nature of various parts of language, by way of various other linguistic devices, with the languages of formal logic playing a central and uniquely important role in the explanatory process. This is drastically different from what was taken to be the uniting central task of traditional philosophy up to that point, that being the formulation of a **logos** of the world; a rationally coherent account of reality at the level of utmost generality; an account of reality as a totality. Thus, coming to be concerned with explaining facts about language and not "capital R Reality", the turn to analytic philosophy is sometimes referred to as the **Linguistic Turn**.

In time this approach to philosophy became the unquestionable dominant metaphilosophical position of English speaking philosophy departments the world over, a position it enjoyed without deviation until the 1960's, when multiple camps within the movement began to disagree with one another over deep and central issues related to the nature of language, over scientific knowledge and practice, and the analytic methods themselves, and hence the nature of philosophy. Today, almost no one working in a English speaking philosophy department and publishing in English philosophy journals would consider themselves adherents to the positions of Russell, or Moore, or Wittgenstein, and with the defining feature of this present era sometimes being identified with its eclecticism and philosophical pluralism, there is a sense in which we are in a "post-analytic" stage.


There are two issues with describing English philosophy as post-analytic though. The first is that it is not a label used by most philosophers, journals, and philosophical associations to describe themselves or what it is that they do. [There are more assocations of analytic philosophy today than there have ever been before](http://www.dif.unige.it/esap), and it is practiced more and more in non-English philosophical communities. Clearly then, we have not moved past being analytic in the sense that we still prefer to call ourselves analytic. The second issue is more interesting and formed part one part of the motivation for this project. It is clear also that if we mean for post-analytic to denote a particular "ism", that there is no "ism" associated with post-analytic philosophy. Philosophers calling themselves analytic hold a wide variety of competing beliefs about central philosophical issues, and what’s more, they are not particularly good at guessing what the most popular positions taken by their peers are, as was shown by David Bourget and David Chalmers in their [Philpapers survey and metasurvey](https://philpapers.org/surveys/). Again it seems clear that there just is no one thing to be called post-analytic philosophy or analytic philosophy understood as a particular doctrine or set of beliefs today. 

So why do they call themselves analytic, and what do they mean? Of the kinds of answers typically given, two are the ones this project was concieved of as scrutinizing: what I will call the **the stylistic answer**, is the that analytic philosophy today is any philosophy written in a particular style, called the **analytic style**. 

## Analytic Style?
Under a naive conception of analytic style, it is supposed to be characterized by the unique level of emphasis it places on **argumentation**, **clarity**, and **rigor**, in comparison to "non-analytic" philosophy. But history tells us that none of these three features are distinctive of analytic philosophy. Argumentation has always been emphasized in philosophy; Wittgenstein, unquestionably one of the most influential authors in the analytic tradition, was called a mystic by Carnap, his works requiring a great deal of interpretation and to this day reasonable disagreements are had about what he really meant in works like the Philosophical investigations; Husserl argued that philosophy is a "rigorous science", where his phenomenological definition of rigor is as similar to any one analytic definition as any two of them are to each other.

Never the less, even among those philosophers who recognize all the points just made, their belief in a distinctive analytic style does not waiver, even though now they may find it difficult or even impossible to say exactly what such a style consists of! However, the above mentioned positive characterization of analytic style has a negative characterization with which it correlates; whatever analytic style is, it is often believed that it is certain that there is one thing it is *not*, and that is what gets called **Continental philosophy**.


## Continental Style?
If Analytic Philosophy broke with the traditional philosophy in taking its linguistic turn, we might say roughly that Continental Philosophy comprises all that philosophy that *did not* take such a turn, at least the same kind or at the same time that analytic philosophy did. Instead we might say it took a **phenomenological** turn. The work of Edmund Husserl (1859-1938) is usually given as the definitive birthplace of phenomenology and the continental tradition. Phenomenology as Husserl understood it was a method for sustained attempts at offering descriptions of both our experiences and the "things themselves". As is evident from my definition of what counts as the Continental tradition, it has very nearly always found itself in an eclectic era, such that the same issues we had with identifying a single post-analytic philosophy will likewise prevent us from considering any singular continental philosophy, even though just like the term "analytic philosophy" and "analytic philosopher", "continental philosophy" and "continental philosopher" are widely-used and preferred professional self-descriptions by philosophers today, even if they do not, nor have they ever been, living on the continent of Europe (Critchley 2001, pg. 37-47). Continental Philosophy has had a tremendous influence on the present state of many humanities and social sciences departments in the United States, save for philosophy:

>...[Continental Philosophy] has decisively influenced many theoretical innovations in the humanities and social sciences: in literary theory, art history and theory, social and political theory, cultural studies, historiography, religious studies, and anthropology, not to mention debates in fine art, architecture, feminism, and psychoanalysis. (Critchley 2001, pg. 41)


So much influence, that the fact that philosophers working in the analytic tradition would label people like Derrida "Pseudo-philosophers" and writing an [open letter in protest](http://ontology.buffalo.edu/smith/varia/Derrida_Letter.htm) of him being awarded an honorary degree from Cambridge is rather interesting, and highly telling about the relationship between not just analytic and continental philosophy, but analytic philosophy and the humanities as a whole. (He was still awarded his degree by a vote of 336 to 204. According to [Sarah Richmond](https://doi.org/10.1111/j.1468-0378.1996.tb00064.x), almost none of the votes in favor were from members of the philosophy department!) It would thus be a desiderata of a characterization of analytic style in terms of its difference from "continental style", that these differences help illuminate why continental work has found purchase with so many different people and fields. 

 
# Method
## Selecting Disciminative Features

To analyze style, I focused on various measure I can perform on the **most frequent words** of each document. I here take it that document specific word frequency rankings, especially as concerns so called *function words*, such as prepositions, articles, and so on, are a reliable type of **author invariant**; the MFW's of a document are a type of linguistic item that appear in documents only by virtue of being written by a particular author, with sets of words occuring across multiple documents with similar frequencies constituting an important part of an author's style. In particular, I use **Craig's Zeta** measure to identify a statistically significant difference in feature distribution between the analytic part of my corpus and the Continental part of my corpus, which I have labeled the "Humanities" portion instead. According to Eder , Rybicki and, Kestemont in "Stylometry with R: A Package for Computational Text Analysis",

>[The Craig Zeta metric] is popular for selecting discriminative stylometric features in a binary classification setting. (pg. 117)

in other words, by using the "oppose()" function in stylo, we can identify significant feature variation between our subcorpora, and thus identify a set of most discriminating words, that is, words that are most characteristics of being analytic or not. This measure will fulfill the goal I outlined above of identifying a specific way in which Analytic style is not continental style, a short set of words that analytic writers prefer together with a set of words that they avoid, i.e. the words most characteristic of Continental writing. Thus my major results and contribution of this project will be this set of words most preferred by Analytic writers in contrast to Continental writers, and words most avoided in contrast to Continental writers.


## Preprocessing
First we take all of the documents I have put together and treat all of the self-identified analytic authors as *one and the same* author, and similarly for the continental authors. This allows me to treat all of the documents written by the various authors in my corpus as being written by one of two people, and then by running well established tests for checking differences between two authors I can establish differences between two sets of authors.

Next is to *tokenize* each document, seperating them into the tokens (words) that they contain as parts.

All that is left after tokenization is to calculate the Craig Zeta.

#Bootstrapping: A Test of MFW's effectiveness

I will quickyl demonstrate why you should trust these methods and consider most frequent words to adequately capture features of authorship by building a **bootstrapping consensus tee** from my documents. Bootstrapping consesus trees are consensus trees built using a distance metric, where a consesus tree is a way of estimating the level of "support" for claudes in a tree, clusters of nodes of the tree.

![Consensus Tree](https://bitbucket.org/JesseRP/analyticstyle/raw/2b31b9406bbc3f841d8e2b73d85c64a1fc71920d/ConsensusTreeDiagram.jpg) 

Consensus trees work by taking multiple different tree diagrams/cladograms having all the same nodes, yet with different groupings, and producing the tree whose nodes are grouped in the way that *best approximates* a grouping that all of the trees (or a given proportion of them) "agree" on. Bootstrapping is any metric that relies on random sampling with replacement; in the case of trees, subtrees from the population are sampled at random, and replaced with the consensus subtree according to the sampling. In this case, the bootstrap consensus tree is built from hierarchical clusterings of documents based on a range of MFW values that we can sample from with replacement (the bootstrapping).

using:

```
stylo(corpus.dir = "philosophy_style_corpus", 
      mfw.min = 1, 
      mfw.max = 277,
      analysis.type = "BCT", 
      sampling = "no.sampling", 
      sample.size = 10000, 
      custom.graph.title = "Style",
      write.png.file = TRUE, gui = FALSE)`
```

My corpus of documents produced this bootstraping tree:

![Bootstrap Tree](https://bitbucket.org/JesseRP/analyticstyle/raw/002c4be6ae17678a31a6295a1116f7e89437eb74/jesserussellpowell_Consensus_2-202_MFWs_Culled_0__Classic%20Delta_C_0.5__001.png)


One with any familiarity with these texts would see to the exemplary effectiveness of this method to attribute authorship and style: "WordandObject" and "TwoDogmasofEmpiricism" are both written by W.V.O. Quine, something that this model predicted by correctly clustering those documents. the same is true of "ThreeModelsfortheDescriptionofLanguage" and "SyntacticeStructures", both written by Noam Chomsky. Furthermore, "Capital" and "DialecticofEnlightment" are clustered, and this makes perfect sense; Horkheimer was a Marxist himself, if his work was not clustered with Marx, the model would have a glaring defect, and yet it got it right. Interestingly, it groups Heidegger with the Analytics.


## Findings
I hope that my demonstration with Bootstrap Consensus trees has helped demonstrate the potential use of these sorts of methods. I will now list my results of discriminant analysis.

using: 

```
raw.corpus <- load.corpus(files = "all", 
                          corpus.dir = "philosophy_style_corpus",
                          encoding = "UTF-8")

corpus.all <- txt.to.words.ext(raw.corpus, 
                                     language = "English.all",
                                     preserve.case = (TRUE))

corpus.analytic <- corpus.all[grep("Analytic", 
                                   names(corpus.all))]

corpus.humanities <- corpus.all[grep("Humanities",
                                     names(corpus.all))]

zeta.results <- oppose(primary.corpus = corpus.analytic,
                       secondary.corpus = corpus.humanities)

zeta.results$words.preferred[1:20]

zeta.results$words.avoided[1:20]

combined.features <- c(zeta.results$words.preferred[1:20],
                       zeta.results$words.avoided[1:20])
```

To identify most characteristic words using [Craig's Zeta Function](https://www.rdocumentation.org/packages/stylo/versions/0.6.9/topics/zeta.craig), I produced the following list of words characteristic of the analytic and Continental authors in my corpus:

![Characteristic Words](https://bitbucket.org/JesseRP/analyticstyle/raw/aaeebfb289da511fc4aa1cc21d34aaf6c71ea534/Image%205-3-19%20at%208.48%20PM.jpg)

We can see a few things immediately:

  1. Though all philosophy is concerned with arguments, and continental philosophy is surely concerned with logic, it seems that
     analytics really are uniquely obsessed with it.
  2. Analytic philosophers are concerned with linguistic entities in a special way that continental philosophers are not.
  3. Continental philosophers seem especially fond of discussing features of our everyday lives as we experience them, as is
     evidenced by dream and perception, but also consciousness, life, and being.
  4. Marxists notions seem to dominate; Marxist theory is disproportionally represented.

One way we might sum these differences up: The Continental writers, and subsequently much of the humanities outside of philosophy, are and have been centrally concerned with **Being**, with **human experience**, with **political conditions and change,** and so forth. They much prefer to use words having to do with **intentionality**, with human **subjectivity** and **action**, or as many might put it, with praxis rather than theory. Analytic philosophy is concerned with **theory** rather than praxis. It really is best conceived as preferring to use terms about **language** and **logic**; Analytic philosophers have been and still are concerned with **knowing**, **proof**, and **explanation**, and by way of all these, **evidence**, **justification**, and **computation**.

I do think the highest ranked words on both sides can definitely serve as approximations of what is distinctive of the two groups; one concerned with creating a useful reconciliation of the two would be wise to start with an account of theory and Being.


# Conclusion

None of this is meant to serve nor possibly could serve as an end to the question of what Analytic style might be, but it surely has gotten us a step closer. We can be confident in the fact there is an analytic style for us to get to the truth of, and that whatever it is today, it owes much of its character to a lineage of great thinkers whose stylistic and intellectual fingerprints are faithfully described by the traditional understanding of them and the cultural myths we tell about them. In many specific ways they may differ, but as a group our history of them has not yet deceived us about what they truly were. I doubt many would see this as a breakthrough in our understanding of what the relation between the analytic and continental traditions consists in, nor in our understanding of how, where, and why we should bring the two in to contact. I think more than anything, it has demonstrated the usefulness of these techniques for the philosophical and humanities enterprises. 

# Works Cited

* Eder, M., Rybicki, J. and Kestemont, M. (2016). Stylometry with R:
  a package for computational text analysis. R Journal 8(1): 107-121.
  <https://journal.r-project.org/archive/2016/J-2016-007/index.html>

