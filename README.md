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

| Shelfmark                                                                                     | Folder                                       | Biblissima                                    | Range               | Type   |   Century | Color   |   Main Zones |   Lines |   Characters | Genre              | Content                                                                                                                                                                                                                                                                                                                         |
|-----------------------------------------------------------------------------------------------|----------------------------------------------|-----------------------------------------------|---------------------|--------|-----------|---------|--------------|---------|--------------|--------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [BnF latin 9768](https://gallica.bnf.fr/ark:/12148/btv1b84238417)                             | [🔗](../medieval-latin/data/bnf-latin-9768)  | [→](https://data.biblissima.fr/entity/Q67388) | 1r-3r               | prose  |        10 | ✗       |           12 |     330 |         9522 | histoire           | Historiarum Libri Quatuor, Nithard                                                                                                                                                                                                                                                                                              |
| [BnF latin 16657](https://gallica.bnf.fr/ark:/12148/btv1b52516888n)                           | [🔗](../medieval-latin/data/bnf-latin-16657) |                                               | 82v-84r             | prose  |        13 | ✓       |            4 |     200 |         8337 | Mathématiques      | Almagesti Minor                                                                                                                                                                                                                                                                                                                 |
| [BnF latin 10996](https://gallica.bnf.fr/ark:/12148/btv1b100389713/f27.item.r=10996)          | [🔗](../medieval-latin/data/bnf-latin-10996) |                                               | 1r-3r               | prose  |        13 | ✗       |            5 |     109 |         4770 |                    | Chartularium Abbatiæ Beatæ Mariæ                                                                                                                                                                                                                                                                                                |
| [Latin 5657](https://gallica.bnf.fr/ark:/12148/btv1b10039103d)                                | [🔗](../medieval-latin/data/latin-5657)      | [→](https://data.biblissima.fr/entity/Q64650) | 42v,36v-37r,46v-47r | prose  |        13 | ✗       |           13 |     152 |         7255 | Cartulaire         | Charte de Renaud Musavène (f42v); Don d'une maison par Mathieu II (f36v); Philippe de Beaumont & Don de la mairie de Champagne par Jehan (f37r); Don d'Hémery Aladent (fin), (?), Bouchard VI de Montmorency (46v); Le Culte de Saint Guillaume établi à Pontoise, Concession par l'abbé de S. Denis du fief de Teleuse (f47r); |
| [BnF Latin 16204](https://gallica.bnf.fr/ark:/12148/btv1b52504905c)                           | [🔗](../medieval-latin/data/bnf-latin-16204) |                                               | 333-337             | prose  |        13 | ✓       |           10 |     462 |        15859 | prose (astrologie) | Albumasar, Tractatus revolutione annorum mundi (De Experimentis); Albumasar, Flores                                                                                                                                                                                                                                             |
| [BnF NAL 775](https://gallica.bnf.fr/ark:/12148/btv1b52509205f)                               | [🔗](../medieval-latin/data/bnf-nal-775)     |                                               | 91r-93r             | prose  |        14 | ✓       |           10 |     491 |        14723 | prose              | Legenda aurea, De sancto Petro martyre, De sancto Philippo apostolo, De sancto Iacobo apostolo                                                                                                                                                                                                                                  |
| [BnF Latin 7720](https://gallica.bnf.fr/ark:/12148/btv1b8446940n)                             | [🔗](../medieval-latin/data/bnf-latin-7720)  |                                               | 100v-102v           | prose  |        14 | ✓       |           10 |     580 |        13711 | prose              | Quintilien, Inst. 11.2.44 seq                                                                                                                                                                                                                                                                                                   |
| [BnF Latin 6337](https://gallica.bnf.fr/ark:/12148/btv1b8452769g/f185.item.r=cicero%20cicero) | [🔗](../medieval-latin/data/bnf-latin-6337)  |                                               | 1r-5v               | prose  |        16 | ✓       |            3 |     176 |         7779 | prose              | Tusculanarum quaestionum libri quinque                                                                                                                                                                                                                                                                                          |

<!-- EndTable -->

## Metrics

<!-- StartMetric -->

### Regions

- MarginTextZone (100)
- MainZone (67)
- RunningTitleZone (14)
- GraphicZone (14)
- NumberingZone (44)
- DropCapitalZone (24)
- StampZone (2)

### Lines

- DefaultLine (2469)
- InterlinearLine (11)
- HeadingLine (20)

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
