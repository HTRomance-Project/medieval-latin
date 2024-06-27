HTRomance, Medieval Latin corpus of ground-truth for Handwritten Text Recognition
  and Layout Segmentation
=====================
![characters badge](badges/characters.svg) ![regions badge](badges/regions.svg) ![lines badge](badges/lines.svg) ![files badge](badges/files.svg)

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.8288817.svg)](https://doi.org/10.5281/zenodo.8288817)

<!-- Custom Zone -->


## Introduction

This ground-truth dataset has been carefully built around the idea of having generic data for building a strong and reliable model for HTR of Latin manuscripts. Each manuscript should have around 10 columns (5 bi-columns pages or 10 pages of single column).

Data follow the Segmonto guidelines.

> [!NOTE]
> The repository contains two XML files per image. The ones suffixed with `.chocomufin.xml` are normalized in order to be compliant with other datasets following the same guidelines. The others are more specific to this repository. We recommend using the normalized documents.


## Credits

- Transcriptions: Anthony Glaise.
- Supervision and manuscript selection: Thibault Clérice, Federic Boschetti, Franz Fischer.
- Project management: Thibault Clérice & Alix Chagué.

<!-- Rien ne doit être modifié manuellement après la balise Start Auto -->

<!-- Start Auto -->

## Transcription guidelines

The transcription guidelines are described in a paper available on [HAL](https://hal-enc.archives-ouvertes.fr/hal-03828353) and published in the Journal for Open Humanities Data. The paper provides specific details about the selection process, the transcription methods and choices, as well as details about the output (mainly the [Generic CREMMA Model for Medieval Manuscripts (Latin and Old French)](https://zenodo.org/record/7234166#.Y7f69afMJhE) for [Kraken](https://kraken.re))

## Data

ALTO and images can be found in the directory called `data/`. Each subfolder of `data/` corresponds to a 
single manuscript, identified by its shelfmark.

<!-- BeginTable -->

| Shelfmark                                                                  | Links                           | Range                         | Type   |   Century | Color   |   Pages |   Main Zones |   Lines |   Characters | Genre                 | Content                                                                                                                                                                                                                                                                                                                         |
|----------------------------------------------------------------------------|---------------------------------|-------------------------------|--------|-----------|---------|---------|--------------|---------|--------------|-----------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [BnF, lat. 13388](https://gallica.bnf.fr/ark:/12148/btv1b105423611)        | [📁](data/bnf-lat-13388)        | 17-27                         | -      |         9 | ✗       |      10 |           10 |     185 |         5046 | Treatises             | _                                                                                                                                                                                                                                                                                                                               |
| [BnF, lat. 9768](https://gallica.bnf.fr/ark:/12148/btv1b84238417)          | [📁](data/bnf-lat-9768)         | 1r-3r                         | prose  |        10 | ✗       |       3 |           12 |     330 |         9522 | Narratives            | Historiarum Libri Quatuor, Nithard                                                                                                                                                                                                                                                                                              |
| [BnF, lat. 17901](https://gallica.bnf.fr/ark:/12148/btv1b10545020t)        | [📁](data/bnf-lat-17901)        | 63r-67v (1f32.item-f141.item) | -      |        11 | ✗       |      10 |           10 |     467 |        16136 | Narratives            | _                                                                                                                                                                                                                                                                                                                               |
| [BnF, lat. 15176](https://gallica.bnf.fr/ark:/12148/btv1b6000962w)         | [📁](data/bnf-lat-15176)        | 5r-7r (f15.item-f19.item)     | -      |        11 | ✗       |       5 |           10 |     556 |        19728 | Narratives            | _                                                                                                                                                                                                                                                                                                                               |
| [BnF, lat. 12449](https://gallica.bnf.fr/ark:/12148/btv1b100342534)        | [📁](data/bnf-lat-12449)        | 196-198                       | -      |        12 | ✗       |       3 |           12 |     512 |        13463 | Treatises             | _                                                                                                                                                                                                                                                                                                                               |
| [BnF, lat. 130](https://gallica.bnf.fr/ark:/12148/btv1b105437719)          | [📁](data/bnf-lat-130)          | 78v-80v                       | mixed  |        12 | ✓       |       5 |            5 |     199 |        11776 | Treatises             | Gregorius Magnus, Homiliae in Ezechielem, 2, HOMILIA II                                                                                                                                                                                                                                                                         |
| [BnF, lat. 12270](https://gallica.bnf.fr/ark:/12148/btv1b10545284v)        | [📁](data/bnf-lat-12270)        | 7-11                          | -      |        12 | ✗       |       5 |           11 |     517 |        12914 | Treatises             | _                                                                                                                                                                                                                                                                                                                               |
| [BnF, lat. 10996](https://gallica.bnf.fr/ark:/12148/btv1b100389713)        | [📁](data/bnf-lat-10996)        | 1r-3r                         | prose  |        13 | ✗       |       3 |            5 |     109 |         4770 | Documents of practice | Chartularium Abbatiæ Beatæ Mariæ                                                                                                                                                                                                                                                                                                |
| [BnF, lat. 8001](https://gallica.bnf.fr/ark:/12148/btv1b52514166k)         | [📁](data/bnf-lat-8001)         | 51v-53v (f106.item-f110.item) | verse  |        13 | ✓       |       5 |           10 |     506 |        16856 | Poetry                | Ovid. met. XI, 671sqq                                                                                                                                                                                                                                                                                                           |
| [BnF, lat. 16085](https://gallica.bnf.fr/ark:/12148/btv1b525140219)        | [📁](data/bnf-lat-16085)        | 63v-65v (f128.item-f132.item) | prose  |        13 | ✓       |       5 |           10 |     392 |         9056 | Treatises             | Arist. Latin. - Metaphysica I, 3sqq                                                                                                                                                                                                                                                                                             |
| [BnF, lat. 17903](https://gallica.bnf.fr/ark:/12148/btv1b52500967c)        | [📁](data/bnf-lat-17903)        | 37r-39r (f128.item-f132.item) | mixed  |        13 | ✓       |       5 |           10 |     439 |        13847 | Poetry                | Flor. Gall.                                                                                                                                                                                                                                                                                                                     |
| [BnF, lat. 14354](https://gallica.bnf.fr/ark:/12148/btv1b9080772d)         | [📁](data/bnf-lat-14354)        | 68b-69ra                      | prose  |        13 | ✗       |       2 |            8 |     546 |        20982 | Narratives            | Collatio Alexandri et Dindimi                                                                                                                                                                                                                                                                                                   |
| [BnF, lat. 16204](https://gallica.bnf.fr/ark:/12148/btv1b52504905c)        | [📁](data/bnf-lat-16204)        | 333-337                       | prose  |        13 | ✓       |       5 |           10 |     462 |        15859 | Treatises             | Albumasar, Tractatus revolutione annorum mundi (De Experimentis); Albumasar, Flores                                                                                                                                                                                                                                             |
| [BnF, lat. 16657](https://gallica.bnf.fr/ark:/12148/btv1b52516888n)        | [📁](data/bnf-lat-16657)        | 82v-84r                       | prose  |        13 | ✓       |       4 |            4 |     199 |         8333 | Treatises             | Almagesti Minor                                                                                                                                                                                                                                                                                                                 |
| [BnF, lat. 5657](https://gallica.bnf.fr/ark:/12148/btv1b10039103d)         | [📁](data/bnf-lat-5657)         | 42v,36v-37r,46v-47r           | prose  |        13 | ✗       |       3 |           13 |     152 |         7255 | Documents of practice | Charte de Renaud Musavène (f42v); Don d'une maison par Mathieu II (f36v); Philippe de Beaumont & Don de la mairie de Champagne par Jehan (f37r); Don d'Hémery Aladent (fin), (?), Bouchard VI de Montmorency (46v); Le Culte de Saint Guillaume établi à Pontoise, Concession par l'abbé de S. Denis du fief de Teleuse (f47r); |
| [BnF, NAL 730](https://gallica.bnf.fr/ark:/12148/btv1b10032547z)           | [📁](data/bnf-nal-730)          | f.13                          | -      |        14 | ✗       |       4 |            8 |     285 |        12510 | Narratives            | _                                                                                                                                                                                                                                                                                                                               |
| [BnF, lat. 14137](https://gallica.bnf.fr/ark:/12148/btv1b52000994w)        | [📁](data/bnf-lat-14137)        | 1r-5v (f5.item-f14.item)      | vers   |        14 | ✓       |       5 |            5 |     193 |         4985 | Poetry                | Catull.                                                                                                                                                                                                                                                                                                                         |
| [BnF, NAL 775](https://gallica.bnf.fr/ark:/12148/btv1b52509205f)           | [📁](data/bnf-nal-775)          | 91r-93r                       | prose  |        14 | ✓       |       5 |           10 |     492 |        14752 | Narratives            | Legenda aurea, De sancto Petro martyre, De sancto Philippo apostolo, De sancto Iacobo apostolo                                                                                                                                                                                                                                  |
| [BnF, lat. 7720](https://gallica.bnf.fr/ark:/12148/btv1b8446940n)          | [📁](data/bnf-lat-7720)         | 100v-102v                     | prose  |        14 | ✓       |       5 |           10 |     580 |        13711 | Treatises             | Quintilien, Inst. 11.2.44 seq                                                                                                                                                                                                                                                                                                   |
| [BnF, lat. 14650](https://gallica.bnf.fr/ark:/12148/btv1b90683756)         | [📁](data/bnf-lat-14650)        | 342v-344r                     | -      |        15 | ✗       |       2 |            4 |     174 |         9305 | Narratives            | Vita Gengulfi                                                                                                                                                                                                                                                                                                                   |
| [BnF, Smith-Lesouëf 11](https://gallica.bnf.fr/ark:/12148/btv1b10085732n)  | [📁](data/bnf-smith-lesouëf-11) | 7-9                           | -      |        15 | ✗       |       3 |            6 |     195 |         7199 | Poetry                | _                                                                                                                                                                                                                                                                                                                               |
| [BnF, Smith-Lesouëf 12](https://gallica.bnf.fr/ark:/12148/btv1b525133052)  | [📁](data/bnf-smith-lesouëf-12) | 7-11                          | -      |        15 | ✗       |       5 |            5 |     119 |         4274 | Narratives            | _                                                                                                                                                                                                                                                                                                                               |
| [BnF, Arsenal, ms. 1046](https://gallica.bnf.fr/ark:/12148/btv1b55013208c) | [📁](data/bnf-arsenal-ms-1046)  | 1r-5v                         | -      |        15 | ✓       |      10 |           10 |     397 |        13417 | Poetry                | Ovide, Les Métamorphoses                                                                                                                                                                                                                                                                                                        |
| [BnF, NAL 632](https://gallica.bnf.fr/ark:/12148/btv1b525060135)           | [📁](data/bnf-nal-632)          | 36r-40v (f75.item-f84.item)   | -      |        15 | ✗       |      10 |           10 |     195 |         7327 | Treatises             | _                                                                                                                                                                                                                                                                                                                               |
| [BnF, NAL 1909](https://gallica.bnf.fr/ark:/12148/btv1b52501128g)          | [📁](data/bnf-nal-1909)         | 46r-52v (f95.item-f108.item)  | vers   |        16 | ✓       |      10 |           10 |     220 |         7333 | Poetry                | Carmina Varia (?)                                                                                                                                                                                                                                                                                                               |
| [BnF, lat. 6337](https://gallica.bnf.fr/ark:/12148/btv1b8452769g)          | [📁](data/bnf-lat-6337)         | 1r-3r (f9.item-f13.item)      | -      |        16 | ✗       |       5 |            7 |     260 |        11546 | Narratives            | _                                                                                                                                                                                                                                                                                                                               |
| [BnF, Smith-Lesouëf 16](https://gallica.bnf.fr/ark:/12148/btv1b10085734j)  | [📁](data/bnf-smith-lesouëf-16) | 21-23                         | -      |        16 | ✗       |       3 |            6 |     151 |         5612 | Documents of practice | _                                                                                                                                                                                                                                                                                                                               |
| [BnF, lat. 6337](https://gallica.bnf.fr/ark:/12148/btv1b8452769g)          | [📁](data/bnf-lat-6337)         | 1r-5v                         | prose  |        16 | ✓       |       5 |            7 |     260 |        11546 | Narratives            | Tusculanarum quaestionum libri quinque                                                                                                                                                                                                                                                                                          |

<!-- EndTable -->

## Metrics

<!-- StartMetric -->

### Total number of pages

145

### Regions

- MarginTextZone (230)
- MainZone (238)
- NumberingZone (146)
- DropCapitalZone (80)
- RunningTitleZone (36)
- StampZone (9)
- DamageZone (4)
- GraphicZone (19)
- Not specified (2)
- TitlePageZone (1)
- DigitizationArtefactZone (2)

### Lines

- DefaultLine (8701)
- InterlinearLine (61)
- HeadingLine (300)
- Not specified (13)
- DropCapitalLine (17)

<!-- EndMetric -->

## Funding

This project was funded by the Bibliothèque nationale de France through the 2022 project calls from
[Datalab](https://www.bnf.fr/fr/bnf-datalab) for 2023.

## Cite the project

> Clérice, T., Chagué, A., Gille-Levenson, M., Brisville-Fertin, O., Pinche, A., Camps, J., Fischer, F., Boschetti, F., Guadagnini, E., Guilhem Couffignal, G., Canteaut, O., Romary, L., Reboul, M., Perreaux, N., Poibeau, T., Smith, M., Norindr, J., Glaise, A., Navas Farré, M., Bordier, J., Leroy, N., Alba, R., & Rubin, G. *HTRomance* [Data set]. https://htromance-project.github.io/
```
@misc{Clerice_HTRomance,
author = {Clérice, Thibault and Chagué, Alix and Gille-Levenson, Matthias and Brisville-Fertin, Olivier and Pinche, Ariane and Camps, Jean-Baptiste and Fischer, Franz and Boschetti, Federico and Guadagnini, Elisa  and Guilhem Couffignal, Gilles and Canteaut, Olivier and Romary, Laurent and Reboul, Marianne and Perreaux, Nicolas and Poibeau, Thierry and Smith, Marc and Norindr, Jade and Glaise, Anthony and Navas Farré, Marina and Bordier, Julie and Leroy, Noé and Alba, Rachele and Rubin, Giorgia},
title = {{HTRomance}},
url = {https://htromance-project.github.io/}
}
```

## Infrastructure

This project relied on the [CREMMA infrastructure](https://www.dim-map.fr/projets-soutenus/cremma/).

