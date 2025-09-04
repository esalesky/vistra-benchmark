# Vistra benchmark

This repository contains the images and annotations for the Vistra benchmark, [published at WMT 2024](https://aclanthology.org/2024.wmt-1.115). 

Each image has a corresponding json file with the:
- Transcript in English, semantically grouped.
- Translations of the text into four target languages: German (de), Spanish (es), Russian (ru), and Mandarin Chinese (zh).
  - Translation segments are aligned to the transcript groups.
- A field `requires_image_context` which contains a binary value for each target language where human translators marked whether the broader visual context was necessary to disambiguate between possible target translations of the English text.
  - Note that this value varies across target languages.
- Image dimensions

An example from the dataset is demonstrated below:

![alt text](https://vistra-benchmark.github.io/static/images/vistra-data-sample.png "An example image from the Vistra dataset, with a box illustrating all the annotation fields and translations.")

An example where visual context disambiguates possible translations of `"EXIT"` into German is shown below:

<img src="https://vistra-benchmark.github.io/static/images/exit-example-large.png" alt="alt text" title="An example showing two images containing the text 'EXIT', which have different translations in German given their visual context." style="width: 50%;">



## License

<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" /></a><br />The Vistra benchmark is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">Creative Commons Attribution-ShareAlike 4.0 License</a> (CC BY-SA).



## Citation

Please cite this data as:

``` bibtex
@inproceedings{salesky-etal-2024-benchmarking,
    title = "Benchmarking Visually-Situated Translation of Text in Natural Images",
    author = "Salesky, Elizabeth  and
      Koehn, Philipp  and
      Post, Matt",
    editor = "Haddow, Barry  and
      Kocmi, Tom  and
      Koehn, Philipp  and
      Monz, Christof",
    booktitle = "Proceedings of the Ninth Conference on Machine Translation",
    month = nov,
    year = "2024",
    address = "Miami, Florida, USA",
    publisher = "Association for Computational Linguistics",
    url = "https://aclanthology.org/2024.wmt-1.115/",
    doi = "10.18653/v1/2024.wmt-1.115",
    pages = "1167--1182",
}
```
