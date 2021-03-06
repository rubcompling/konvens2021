# Automatic Phrase Recognition in Historical German

This repository contains the manually annotated data sets and additional material for the paper:

Katrin Ortmann. 2021. Automatic Phrase Recognition in Historical German. In *Proceedings of the 17th Conference on Natural Language Processing (KONVENS 2021)*, Düsseldorf, Germany, pp. 127-136. [PDF](https://aclanthology.org/2021.konvens-1.11.pdf)

## Gold data

The manually annotated data sets can be found in the `data` folder. Included are:

- 547 sentences from five written modern registers from [Ortmann et al. (2019)](https://github.com/rubcompling/konvens2019),
- 342 sentences from the HIPKON corpus [(Coniglio et al., 2014)](https://doi.org/10.34644/laudatio-dev-yiTKCnMB7CArCQ9CxLhJ)
- and 608 sentences from the DTA [(German Text Archive; BBAW, 2019)](http://www.deutschestextarchiv.de/).

The data sets were taken from a previous study on chunking [(Ortmann, 2021a)](https://www.aclweb.org/anthology/2021.nodalida-main.19) and enriched with phrases.

The data is available in CoNLL2000 format (cf. [Sang & Buchholz, 2000](https://www.aclweb.org/anthology/W00-0726.pdf)) and contains word forms, [STTS POS tags](http://www.sfs.uni-tuebingen.de/resources/stts-1999.pdf), and BIO phrases, separated by spaces.

The following phrase types are included:

- `NP` (noun phrase)
- `PP` (prepositional phrase)
- `ADVP` (adverb phrase)
- `AP` (adjective phrase)

## Parser models

The trained grammars for the [Berkeley parser](https://github.com/slavpetrov/berkeleyparser) (v.1.7; Petrov et al., 2006) are included in the `models` folder.

## License

The parser models and the DTA corpus are licensed under [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/), and the HIPKON corpus is licensed under [CC BY 3.0](https://creativecommons.org/licenses/by-sa/3.0/). The modern data set is licensed under [CC BY-SA 3.0](https://creativecommons.org/licenses/by-sa/3.0/), except for the TED talk sample, which is provided under [CC BY–NC–ND 4.0](https://creativecommons.org/licenses/by-nc-nd/4.0/deed.de).

## References

BBAW. 2019. Deutsches Textarchiv. Grundlage für ein Referenzkorpus der neuhochdeutschen Sprache. Berlin-Brandenburgische Akademie der Wissenschaften; http://www.deutschestextarchiv.de/.

Marco Coniglio, Karin Donhauser, and Eva Schlachter. 2014. HIPKON: Historisches Predigtenkorpus zum Nachfeld (Version 1.0). Humboldt-Universität zu Berlin. SFB 632 Teilprojekt B4.

Ulrike Demske. 2005. Mercurius-Baumbank (Version 1.1). Universität Potsdam. [LAUDATIO access](https://doi.org/10.34644/laudatio-dev-VyQiCnMB7CArCQ9CjF3O)

Katrin Ortmann, Adam Roussel, and Stefanie Dipper. 2019. Evaluating Off-the-Shelf NLP Tools for German. In *Proceedings of the Conference on Natural Language Processing (KONVENS)*, pages 212–222.

Katrin Ortmann. 2021a. Chunking Historical German. In *Proceedings of the 23rd Nordic Conference on Computational Linguistics (NoDaLiDa)*, Reykjavik, Iceland (online), pages 190–199.

Katrin Ortmann. 2021b. Automatic Phrase Recognition in Historical German. In *Proceedings of the 17th Conference on Natural Language Processing (KONVENS 2021)*, Düsseldorf, Germany, pp. 127-136. [PDF](https://aclanthology.org/2021.konvens-1.11.pdf)

Slav Petrov, Leon Barrett, Romain Thibaux, and Dan Klein. 2006. Learning accurate, compact, and interpretable tree annotation. In *Proceedings of the 21st International Conference on Computational Linguistics and 44th Annual Meeting of the Association for Computational Linguistics*, pages 433–440.

Anne Schiller, Simone Teufel, Christine Stöckert, and Christine Thielen. 1999. *Guidelines für das Tagging deutscher Textcorpora mit STTS (Kleines und großes Tagset)*. [PDF](http://www.sfs.uni-tuebingen.de/resources/stts-1999.pdf).

