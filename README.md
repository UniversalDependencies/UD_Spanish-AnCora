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


# Coreference and Entities

The MISC column contains annotation of named entities and coreference, converted
from the original XML files of AnCora-CO and merged with the UD-style morpho-
syntactic annotation. The format of these annotations is described in
[Nedoluzhko et al. (2021): Coreference meets Universal Dependencies – a pilot
experiment on harmonizing coreference datasets for 11 languages](https://ufal.mff.cuni.cz/techrep/tr66.pdf).


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

* 2024-11-15 v2.15
  * Removed feature AdvType.
  * Construction annotations in the [UCxn](https://github.com/LeonieWeissweiler/UCxn) framework added to MISC
  
     This release adds rule-based annotations of Interrogatives, Conditionals, Existentials, and NPN (noun-preposition-noun) constructions on the head of the respective phrase, plus construction elements. The UCxn v1 notation and categories are documented [here](https://github.com/LeonieWeissweiler/UCxn/blob/main/docs/UCxn-v1.pdf).

* 2024-05-15 v2.14
  * Dependency of "le" should be obl:arg or expl but not obj.
  * Dates ("el 7 de abril") should be connected via nmod, not compound.
  * Percentages ("40 por ciento") should be connected via nmod, not compound.
* 2023-11-15 v2.13
  * "No" and "que" before "hay que Inf" should depend on "hay".
  * NumForm=Word and NumForm=Digit used where appropriate.
  * Combination of letters and digits is not NUM but SYM.
  * Currencies do not have NumForm=Digit (but they keep their special XPOS).
  * Fixed remaining instances of double-subject clauses.
  * Fixed: Sentence-initial "y" is cc, not advmod.
  * "quién" is interrogative, not relative.
  * "quien" is relative, not interrogative.
  * Tokenization: number + "%" split into two tokens.
* 2023-05-15 v2.12
  * Propagated the arg and tem attributes from the original AnCora.
  * Por-nominals under participles changed from obj to obl:agent.
  * Prepositional objects changed to obl:arg.
  * Fixed: "donde", "cuando" can be SCONJ or ADV but not PRON. Interrogative "dónde", "cuándo" are only ADV.
  * Existential "hay" and necessitative "hay que": AUX changed to VERB.
  * Fixed: "hay que" + infinitive should be xcomp, not conj.
  * Named entities that are not annotated for coreference marked as such.
  * "cuyo" is a relative determiner.
  * "qué", "cuál" are interrogative, not relative.
  * "que", "cual" are relative, not interrogative.
* 2022-05-15 v2.10
  * Heuristically resolved coreference cluster type mismatches.
  * Coreference annotation converted to CorefUD 1.0 format.
* 2021-11-15 v2.9
  * Changed sentence ids to reflect the original AnCora documents.
  * Reordered sentences by sentence ids.
  * Added document boundaries.
  * Copied XPOS from the original AnCora.
  * Copied CorefUD-style coreference and entity annotation from the original AnCora.
  * Created enhanced representation (needed for coreference annotation).
  * The license changed to CC BY 4.0 (https://doi.org/10.5281/zenodo.4762030).
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
License: CC BY 4.0
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
