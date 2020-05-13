# MWE-CWI Dataset [![CC BY-NC-SA 4.0][cc-by-nc-sa-shield]][cc-by-nc-sa]

Publications using this dataset must include a reference to the following publication:

Ekaterina Kochmar, Sian Gooding, Matthew Shardlow (2020). [*Detecting Multiword Expression Type Helps Lexical Complexity Assessment*](https://arxiv.org/pdf/2005.05692.pdf). In Proceedings of LREC 2020.

## Dataset

The full annotated dataset consisting of 4732 phrases extracted from the Complex word identification Shared Task 2018 dataset(https://sites.google.com/view/cwisharedtask2018/datasets) is stored in the tab-separated file `final_MWE_dataset.tsv` with the following fields:

- Unique identifier of the expression in this dataset (`Index`): from *0* to *4731*
- Annotator's id (`Annotator`): *0* for the cases that were annotated by all three annotators, and *1-3* for individual annotations from each of the annotators 
- The original subset in the shared task data the instance comes from (`Subset`): *Train*, *Dev* or *Test*
- Genre of the text the instance comes from (`Genre`): *News*, *Wikipedia* or *WikiNews*
- The unique identifier of the text in the original shared task data (`ID`)
- Binary compexity score from the original shared task data (`Complex_binary`):	*0* for non-complex and *1* for complex expressions
- Complexity score assigned based on the proportion of 20 annotators that considered an expression complex; derived from the original dataset (`Complex_probabilistic`): values in the range of *[0.0, 1.0]*
- Character offset for the beginning of the expression in the instance; derived from the original dataset (`Start_index`)
- Character offset for the end of the expression in the instance; derived from the original dataset (`End_index`)
- Number of native annotators, among the total of 10, that considered an expression complex; derived from the original dataset (`Native_complex`): values in the range of *0* to *10*
- Number of non-native annotators, among the total of 10, that considered an expression complex; derived from the original dataset (`Non_native_complex`): values in the range of *0* to *10*
- The original expression from the shared task dataset that was annotated with an MWE type (`Expression`)
- The original context of use in the shared task dataset (`Context`)
- MWE type assgined to the expression (`Annotation`) – see the paper for details on the annotation scheme.

## Annotation Guidelines



This work is licensed under a [Creative Commons Attribution-NonCommerial-ShareAlike 4.0
International License][cc-by-nc-sa].

[![CC BY-NC-SA 4.0][cc-by-nc-sa-image]][cc-by-nc-sa]

[cc-by-nc-sa]: http://creativecommons.org/licenses/by-nc-sa/4.0/
[cc-by-nc-sa-image]: https://licensebuttons.net/l/by-nc-sa/4.0/88x31.png
[cc-by-nc-sa-shield]: https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg
