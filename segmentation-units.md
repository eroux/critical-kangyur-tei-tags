# Tibetan text segmentation units

This short page tries to describe the different units used to segment a Tibetan text, and particularly the Kangyur and Tengyur. Tibetan syntax is largely unexplored (cf. the [number of publications](https://en.wikibooks.org/wiki/Research_on_Tibetan_Languages:_A_Bibliography#Classical_Tibetan_Syntax)), so the vocabulary, the definitions, the units, everything may be inaccurate.

This table summarizes the different units:

TODO

A **volume** (པོ་ཏི or པོད) is a physical book, it is edition-dependant.

The **category** (སྡེ་ཚན) is a general and blur unit, designating a group of smaller units.

The **text** (ཆོས་ཚན in this context, but could also be པོད་ཚན, ལེ་ཚན or ཚན་པ) is the most consensual unit, all editions have the same text segmentation (but not the same order nor the same number of texts).

The **page** (ཤོག) and **line** (ཡིག་ཕྲེང) are quite obvious and edition-dependant.

The **verse** (ཚིག་བཅད་ཀྱི་རྐང་པ or ཚིག་རྐང) has the usual definition and is noted in the text, but not all text is in verse.

The **shloka** (ཚིག་བཅད) is a group of 4 verses (ཚིག་རྐང་བཞི) when the text is in verse, or a group of 30 syllables when the text is in prose. As different editions may have differences in the text, shlokas are edition-dependant.

The **bampo** (བམ་པོ) is a group of 300 shlokas,and thus edition-dependant.

The **chapter** (ལེའུ) is a division of a text, written in the text itself, all editions have the same chapter.

The **syllable** (ཚིག) is a group of characters, syllables are separated by tshegs (་).

The **word** (མིང་ཚིག) is a group of characters (including tshegs). It is not marked in the text and the division may not be consensual. Many ambiguities prevent automatic word segmentation, ex: བར can be `བ + particle ར` or the word བར. Words can be inflected with affix particles for instance བཀའི is word བཀའ + particle འི. There is thus no direct correspondance between group of syllables and word, but there is between words+affix particles and groups of syllables.

The **sentence** (ཚིག་སྒྲུབ) is a relatively new unit (the word itself is ~50 years old). Sentences are not noted in the text, and sentence segmentation is not consensual.

The **paragraph** (བརྗོད་པ) is a new unit (word is very new), not very well defined and non-consensual. It may or may not be a group of syllables ending by a སླར་བསྡུ particle.

## Table of content segmentation

Tibetan texts usually have a table of content (དཀར་ཆག) segmenting the text into different topics. Different table of contents may exist though, so this cannot be considered universal.


## Edition-independant references

It is necessary to have a common reference system allowing to reference all parts of texts in the Kangyur in an edition-independant way, similar to the reference system of the Bible. The problem is with texts in prose, as they have no consensual edition-independant units. A system is yet to be found.

## Concordance

Long term possibility: making something similar to [Strong's concordance](https://en.wikipedia.org/wiki/Strong%27s_Concordance) for the Kangyur and Tengyur. This would ease the constitution of glossaries, dictionnaries, etc. A first step is to cut the whole Kangyur into words and index them.
