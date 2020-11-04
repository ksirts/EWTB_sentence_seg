## Estonian Web Treebank manually annotated with sentence and token boundaries

This repository contains the Estonian Web Treebank (EWTB), available in [Universal Dependencies](https://universaldependencies.org) Collection. The EWTB was originally created by Muischnek, Müürisep and Särg (2019).

The current version of the corpus has been manually annotated with both orthographic (O) and syntactic (S) sentence boundaries as well as token boundaries.
* **Orthographic sentence boundaries** are marked after the common sentence-final punctuation marks (.!?), but also when the sentence-final punctuation mark is missing but the next word starts with a capital letter and the intention of starting a new sentence is clear.
* **Syntactic sentence boundaries** are marked in places that do not necessarily correspond to orthographic sentence boundary, such that the sentence still makes up a syntactically complete unit.
* Finally, different from the original EWTB available in UD collection, the current version of the corpus also contains **aragraph boundaries** (P), which are always considered as sentence boundaries.

The data is in the [CONLL-U format](https://universaldependencies.org/format.html), currently containing only word tokens themselves. The exact label of the sentence boundary is given in the `# label` header of each sentence. The number after each boundary label (O, S and P) denotes how many annotators labelled this type of boundary in that specific place. All annotated boundaries are majority boundaries obtained based on the labels of 3 or 5 annotators.

### Referencing

If you use this dataset then please cite the following publication that describes the annotation process and the evaluation of several existing sentence segmentation and tokenization systems on this dataset:

Sirts, K., & Peekman, K. (2020). [Evaluating Sentence Segmentation and Word Tokenization Systems on Estonian Web Texts.](http://ebooks.iospress.nl/volumearticle/55541) In *Volume 328: Human Language Technologies – The Baltic Perspective*, Frontiers in Artificial Intelligence and Applications, pages 174-181.

```
@inproceedings{sirts2020evaluating,
  title={{Evaluating Sentence Segmentation and Word Tokenization Systems on Estonian Web Texts}},
  author={Sirts, Kairit and Peekman, Kairit},
  booktitle={Volume 328: Human Language Technologies – The Baltic Perspective},
  series={Frontiers in Artificial Intelligence and Applications},
  year={2020},
  pages={174--181},
  doi={10.3233/FAIA200620}
}
```

