# Annotation Instructions

Each sentence has two existing labels:

* 'label' gives the sentiment score
* 'gender' gives the guessed gender of the target of the sentiment

The 'gender' label has three tags:

* 'masc' for masculine-gendered words, like 'he' or 'father'
* 'femm' for feminine-gendered words, like 'she' or 'mother'
* 'neut' for neutral-gendered words, like 'they' or 'parent'

For each sentence, you are to annotate if the sentence's **sentiment is directed toward the labeled gender**. 

Please annotate **1** if the sentence is **correctly labeled** and **0** if not.

(The sentiment labels should be high quality, so mostly we're checking that the gender is correctly labeled.)

## Positive examples (you'd annotate 1)

* sentence: She gave an excellent performance.
* label: .8
* gender: femm

Sentiment is directed at the 'she'.

---

* sentence: The director gets excellent performances out of his cast.
* label: .7
* gender: masc

Sentiment is directed at the male-gendered director.

---

* sentence: Despite a typical parent drama, the excellent acting makes this movie a charmer.
* label: .8
* gender: neut

Sentiment is directed at the movie, and the main topic of the movie is 'parents', a neutrally-gendered word. 


## Negative examples (you'd annotate 0)

* sentence: A near miss for this new director.
* label: .3
* gender: femm

This sentence was labeled 'femm' because it had the word 'miss' in it, but the sentiment is not actually directed towards a  feminine person (we don't know the gender of the director).

---

* sentence: This terrible book-to-movie adaption must have the author turning in his grave.
* label: .2
* gender: masc

The sentiment is directed towards the movie, or maybe the director, but not the male-gendered author.

---

* sentence: I wanted to pull out my eyes and throw them at the screen.
* label: .1
* gender: neutral

---

The sentiment is directed at the movie, not the neutral-gendered eyes.

* sentence: The friend I went with--she chuckled at all the wrong times, which is a bad sign.
* label: .3
* gender: neutral

The sentiment is directed at the movie, not the female-gendered friend.

---

* sentence: What they see in each other also is difficult to fathom.
* label: .2
* gender: neutral

The sentiment is probably directed at the movie, not whoever "they" are.