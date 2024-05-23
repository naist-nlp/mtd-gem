# Multilingual Travelogue Dataset with Geographic Entity Mention (MTD-GEM)

## Data Statistics

The dataset covers comparable Indonesian language and English articles.

| Number of   | Indonesian | English |
| :---        |       ---: |    ---: |   
| Sentences   |      1,391 |   1,914 |
| Words       |     47,415 |  47,902 |
| Named       |      3,937 |   2,756 |
| Nominal     |      2,062 |   2,243 |
| Named (U)   |      1,156 |   1,053 |
| Nominal (U) |        430 |     760 |

## Data Format

The dataset is available in **JSON** format with the following specifications.

- Each file is named according to the article ID (e.g., `0100001`) and it contains the sets of `text`, `line`, `range`, and `entities`.

```
[
    {
        "text": "October 29, 2020    Review Villa Dekat Canggu: Villa Ipanema", 
        "line": 0, 
        "range": [
            1, 
            60
        ], 
        "entities": [
            ...
        ]
    } 
    ... 
]
```

- An entity under `entities` has the `type`, `span`, and `name` as follows.

```
[
    {
        "type": "FAC_NOM", 
        "span": [
            27, 
            32
        ], 
        "name": "Villa"
    },
    ...
]
```

## Contact

Eunike Kardinata <eunike.kardinata.ef9 [at] is.naist.jp>

## Acknowledgement

This study was supported by JSPS KAKENHI Grant Number JP22H03648.

## Citation

Please cite the following paper.

```
@inproceedings{kardinata-etal-2024-constructing-indonesian,
    title = "Constructing {I}ndonesian-{E}nglish Travelogue Dataset",
    author = "Kardinata, Eunike Andriani  and
      Ouchi, Hiroki  and
      Watanabe, Taro",
    booktitle = "Proceedings of the 2024 Joint International Conference on Computational Linguistics, Language Resources and Evaluation (LREC-COLING 2024)",
    month = may,
    year = "2024",
    address = "Torino, Italy",
    publisher = "ELRA and ICCL",
    url = "https://aclanthology.org/2024.lrec-main.333",
    pages = "3759--3771",
}
```
