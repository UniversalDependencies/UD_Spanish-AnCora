# Summary

Spanish data from the [AnCora](http://clic.ub.edu/corpus/) corpus.


# Introduction

The original annotation was done in a constituency framework as a part of the
[AnCora](http://clic.ub.edu/corpus/) project at the University of Barcelona.
It was converted to dependencies and used in the
[CoNLL 2009 shared task](https://ufal.mff.cuni.cz/conll2009-st/index.html).
The CoNLL 2009 version was later converted to
[HamleDT](https://ufal.mff.cuni.cz/hamledt) and to Universal Dependencies.

The GNU license is inherited from the original dataset, downloaded from
the AnCora website. Any license-related questions have to be directed to
the original data providers at the University of Barcelona (that is, not
to the UD contact address listed at the end of this README file).


# Acknowledgements

The following paper must be cited when using this corpus:

 * Taulé, M., M.A. Martí, M. Recasens (2008) 'Ancora: Multilevel Annotated Corpora for Catalan and Spanish',
   Proceedings of 6th International Conference on Language Resources and Evaluation. Marrakesh (Morocco).

In addition, the following paper must be cited if coreference information (attributes entity, coreftype,
corefsubtype, homophoricDD or entityref) is used:

 * Recasens, Marta, M. Antònia Martí (2010) ‘AnCora-CO: Coreferentially annotated corpora for Spanish and
   Catalan’. Language Resources and Evaluation, Springer Science.

Additionally, the following paper must be cited when argumental attributes in "sn" or "grup.nom"
(attributes func, arg, tem or lexicalid) are used:

 * Peris, Aina, Mariona Taulé, Horacio Rodríguez (2010) ‘Semantic Annotation of Deverbal Nominalizations in the
   Spanish AnCora corpus’. Treebanks and Linguistic Theories (TLT-2010), Estonia.


# Changelog

* 2021-05-15 v2.8
  * Fixed: AdpType=Preppron wrongly appeared at the first word of multi-word
    prepositions such as "delante del".
  * Removed XPOS (which was uninformative).
  * Split fused preposition-articles al, del.
* 2019-05-01 v2.4
  * Hundreds of manual fixes and thousands of semiautomatic fixes of errors.
* 2017-03-01 v2.0
  * Converted to UD v2 guidelines.
* 2016-05-01 v1.3
  * Initial release.


=== Machine-readable metadata =================================================
Data available since: UD v1.3
License: GNU GPL 3.0
Includes text: yes
Genre: news
Lemmas: converted from manual
UPOS: converted from manual
XPOS: not available
Features: converted from manual
Relations: converted from manual
Contributors: Martínez Alonso, Héctor; Zeman, Daniel
Contributing: here
Contact: zeman@ufal.mff.cuni.cz
===============================================================================
