# DAASI-simplification-corpus

# DAASI: Arabic Text Simplification Corpus for Israeli Government Documents

**DAASI** (*Diglossia-Aware Arabic Simplification for Inclusion*) is a parallel corpus for **Arabic text simplification in the Israeli government domain**. 
DAASI is designed to support research on **inclusive Arabic NLP**, particularly text simplification for Arabic-speaking citizens who encounter formal, bureaucratic MSA in government communications while using Levantine Arabic in everyday life.
> **Important:** DAASI addresses **intralingual MSA-to-simplified-MSA text simplification**. It is not a translation corpus and does not convert MSA into Levantine Arabic. 
**DAASI: Arabic Text Simplification Corpus for Israeli Government Documents**

Maysa Abu Shareb, Huseen Abo Ismael, and Natalia Vanetik

Accepted at the **Fourth Arabic Natural Language Processing Conference (ArabicNLP 2026)**, co-located with EMNLP 2026, Budapest, Hungary.

### Citation

```bibtex
@inproceedings{abu-shareb2026daasi,
  title     = {{DAASI}: Arabic Text Simplification Corpus for Israeli Government Documents},
  author    = {Abu Shareb, Maysa and Abo Ismael, Huseen and Vanetik, Natalia},
  booktitle = {Proceedings of the Fourth Arabic Natural Language Processing Conference (ArabicNLP 2026)},
  year      = {2026},
  publisher = {Association for Computational Linguistics}
}
```

---

## Overview

Formal government documents can be difficult to understand even for proficient readers of Modern Standard Arabic. 
In Israel, this challenge is particularly relevant because many Arabic-speaking citizens use Levantine Arabic in everyday communication while encountering formal MSA in government, administrative, legal, and public-service documents.

DAASI was created to investigate and address this problem through domain-specific Arabic text simplification.

The corpus was constructed from **50 official Arabic-language documents** published by the Israeli National Insurance Institute. 

---

## Corpus Statistics

| Property                 |                                  Value |
| ------------------------ | -------------------------------------: |
| Source documents         |                                     50 |
| Initial source sentences |                                  2,702 |
| Final sentence pairs     |                              **2,350** |
| Source language          |                 Modern Standard Arabic |
| Target language          |      Simplified Modern Standard Arabic |
| Domain                   |   Israeli government / public services |
| Primary source           | National Insurance Institute of Israel |
| Simplification method    |        GPT-4o draft + human validation |

The initial collection contained **2,702 candidate sentence pairs**. After human validation, alignment, and filtering, **2,350 pairs** were retained.

Pairs were discarded when the proposed simplification changed the meaning, omitted important information, or otherwise failed the corpus requirements.

---

## Dataset Format

The recommended dataset format is one sentence pair per row:

| Column       | Description                             |
| ------------ | --------------------------------------- |
| `original`   | Original government-domain MSA sentence |
| `simplified` | Human-validated simplified MSA sentence |

Example:

```text
original:    <Arabic original sentence>
simplified:  <Arabic simplified sentence>
```

If additional metadata are included in the released version, their definitions are documented in the corresponding dataset file.



## Data Source

The source documents were collected from publicly available Arabic-language pages of the Israeli National Insurance Institute.

The original documents are government publications and remain subject to their respective terms and conditions.

DAASI should not be interpreted as an official translation, rewrite, or endorsement by the National Insurance Institute.

---

## Limitations

Several limitations should be considered when using DAASI:

* The corpus contains documents from a single government authority.
* Only 50 source documents are represented.
* The corpus contains 2,350 validated sentence pairs, which is relatively small compared with large general-domain simplification resources.
* The participant survey was based on a convenience sample and was skewed toward younger participants.
* The corpus targets simplified MSA rather than direct MSA-to-Levantine conversion.
* Generalization to other Arabic dialect communities has not been systematically evaluated.
* Inter-annotator agreement statistics were not retained during the original corpus-construction process.
* The detailed raw participant ratings for the final human evaluation were not retained; only aggregated statistics are reported in the paper.

---

## Intended Uses

DAASI is intended primarily for research on:

* Arabic text simplification;
* low-resource NLP;
* government-domain NLP;
* accessible language technologies;
* Arabic readability;
* Arabic diglossia;
* MSA simplification;
* domain adaptation;
* text-to-text generation;
* inclusive NLP; and
* human-centered NLP evaluation.

Potential applications include research prototypes for simplifying public-service information and studying linguistic accessibility.

---

## Citation

If you use DAASI, please cite:

```bibtex
@inproceedings{abu-shareb2026daasi,
  title     = {{DAASI}: Arabic Text Simplification Corpus for Israeli Government Documents},
  author    = {Abu Shareb, Maysa and Abo Ismael, Huseen and Vanetik, Natalia},
  booktitle = {Proceedings of the Fourth Arabic Natural Language Processing Conference (ArabicNLP 2026)},
  year      = {2026},
  publisher = {Association for Computational Linguistics}
}
```

Please also cite the original papers for any pretrained models or external datasets used in your experiments, including AraT5, mT5, AraBERT, SAMER, Stanza, and GPT-4o.

---



## Contact

For questions regarding DAASI or the associated research:

**Natalia Vanetik**
Department of Software Engineering
Shamoon College of Engineering
Beer Sheva, Israel
[natalyav@sce.ac.il](mailto:natalyav@sce.ac.il)

**Maysa Abu Shareb**
[maysaab@ac.sce.ac.il](mailto:maysaab@ac.sce.ac.il)

**Huseen Abo Ismael**
[huseen1141@outlook.com](mailto:huseen1141@outlook.com)

---

## Acknowledgement for Derived Work

If you extend DAASI, create additional annotations, or use the corpus in a published study, please cite the DAASI paper and clearly identify the version of the corpus used.
