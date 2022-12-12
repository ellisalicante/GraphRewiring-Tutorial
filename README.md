# Graph Rewiring: From Theory to Applications in Fairness <br>(Tutorial LoG 2022)
This repository holds code and other relevant files about **["Graph Rewiring: From Theory to Applications in Fairness"](https://ellisalicante.org/tutorials/GraphRewiring)**, following the tutorial presented at [**Learning on Graphs 2022**](https://logconference.org/). Go to the [official tutorial webpage](https://ellisalicante.org/tutorials/GraphRewiring) for more information about the tutorial, the speakers, the slides and the video.



![header_grey](https://user-images.githubusercontent.com/33413560/204992639-8fdb4ebe-0389-4950-b6e7-de414cc3d7b8.png)


#### Organizers: [*Adrián Arnaiz*](https://ellisalicante.org/tutorials/GraphRewiring), [*Francisco Escolano*](https://ellisalicante.org/tutorials/GraphRewiring), [*Nuria Oliver*](https://ellisalicante.org/tutorials/GraphRewiring), [*Edwing Hancock*](https://ellisalicante.org/tutorials/GraphRewiring), [*Ahmed Begga*](https://ellisalicante.org/tutorials/GraphRewiring)
#### Panelists: [*Marika Zitnik*](https://ellisalicante.org/tutorials/GraphRewiring), [*Petar Veličković*](https://ellisalicante.org/tutorials/GraphRewiring), [*Francesco Di Giovanni*](https://ellisalicante.org/tutorials/GraphRewiring)

- [Installation](#installation)
- [Code Explanation](#code-explanation)
- [Slides and Tutorial Outline](#slides-and-tutorial-outline)
- [Troubleshooting](#troubleshooting)
- [Aknowledgments](#aknowledgments)
- [Citation](#citation)

## Installation

### COLLAB

As most of the content is aimed to Google COLLAB, we developed self-contained jupyter notebooks with cells to install the libraries at the beginning of those. However, we will provide instructions to install the enviroment locally.

**Each jupyter notebook has an icon at the top to open it in COLLAB by simply clicking on it**: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ellisalicante/GraphRewiring-Tutorial/blob/main/0-Spectral-Background.ipynb).

| File | Collab|
|-|-|
| Introduction to Spectral Theory |[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ellisalicante/GraphRewiring-Tutorial/blob/main/0-Spectral-Background.ipynb)|
| Transductive RW|[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ellisalicante/GraphRewiring-Tutorial/blob/main/1-Transductive-Rewiring.ipynb)|
| Lovász Bound and Commute Times | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ellisalicante/GraphRewiring-Tutorial/blob/main/2-Lovasz-Bound-and-CT.ipynb) |
| CT-Layer |[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ellisalicante/GraphRewiring-Tutorial/blob/main/3-Inductive-Rewiring-CTLayer.ipynb) |


### Local

Future instructions to be added
#TBA - environment installations

```bash
git clone https://github.com/ellisalicante/GraphRewiring-Tutorial
git submodule update --init --recursive
#TBA - environment installations
```

## Code Explanation

```bash
code
├── DiffWire #Original Repositori of DiffWire (CT-Layer, GAP-Layer, trained models...)
├── *.ipynb #Notebooks for each of the parts of the tutorial
```

## Slides and Tutorial Outline
* **[Official Tutorial Web Page](https://ellisalicante.org/tutorials/GraphRewiring)**
* **[Outline](https://ellisalicante.org/tutorials/GraphRewiring#outline)**

## Troubleshooting

In case that clicking the icon does not work, you can open it in COLLAB manually. To open the notebooks directly in COLLAB, go to the path of the notebook and change `https://github.com/[notebook_path]` to `https://colab.research.google.com/github/[notebook_path]`. For example, if you want to open `https://github.com/ellisalicante/GraphRewiring-Tutorial/blob/main/0-Spectral-Background.ipynb` in COLLAB, you should go to https://colab.research.google.com/github/ellisalicante/GraphRewiring-Tutorial/blob/main/0-Spectral-Background.ipynb

To generate such links in one click, you can use the [Open in Colab](https://chrome.google.com/webstore/detail/open-in-colab/iogfkhleblhcpcekbiedikdehleodpjo) Chrome extension.

For more problems, suggestions or feedback, **please contact *adrian@ellisalicante.org***.

## Aknowledgments

A. Arnaiz-Rodriguez and N. Oliver are supported by a nominal grant received at the **ELLIS Unit Alicante Foundation** from the **Regional Government of Valencia in Spain** (Convenio Singular signed with Generalitat Valenciana, Conselleria d’Innovació, Universitats, Ciència i Societat Digital, Dirección General para el Avance de la Sociedad Digital). A. Arnaiz-Rodriguez is also funded by a grant by the **Banc Sabadell Foundation**. F. Escolano is funded by the project **RTI2018-096223-B-I00** of the Spanish Government. 

## Citation

If you use the code or the tutorial in your research, please cite as follows:

* If you use the code or the tutorial from parts ***Introduction to Spectral Theory***, ***Introduction to Lovász Bound***, ***Transductive RW*** or ***Inductive Rewiring (DiffWire)***, please cite:

```bibtex
@inproceedings{
arnaiz-rodriguez2022diffwire,
title={DiffWire: Inductive Graph Rewiring via the Lov\'asz Bound},
author={Adrian Arnaiz-Rodriguez and Ahmed Begga and Francisco Escolano and Nuria Oliver},
booktitle={Learning on Graphs Conference},
year={2022},
url={https://openreview.net/forum?id=IXvfIex0mX6f}
}
```

 If you use the code or the tutorial from Graph Rewiring part, please cite: ***To Be Added***.