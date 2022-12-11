# Graph Rewiring: From Theory to Applications in Fairness <br>(Tutorial LoG 2022)
This repository holds code and other relevant files for the [**Learning on Graphs 2022**](https://logconference.org/) tutorial **["Graph Rewiring: From Theory to Applications in Fairness"](https://ellisalicante.org/tutorials/GraphRewiring)**. This tutorial will be presented at Learning on Graphs 2022 on **December 11, 2022 at 10am - 1pm ET (16 - 19 CET)**. The tutorial will consist on 2 hours of theory and hand-on content followed by a 1 hour panel discussion. More information [here](https://ellisalicante.org/tutorials/GraphRewiring).


![header_grey](https://user-images.githubusercontent.com/33413560/204992639-8fdb4ebe-0389-4950-b6e7-de414cc3d7b8.png)


#### Organizers: [*Adrián Arnaiz*](https://ellisalicante.org/tutorials/GraphRewiring), [*Francisco Escolano*](https://ellisalicante.org/tutorials/GraphRewiring), [*Nuria Oliver*](https://ellisalicante.org/tutorials/GraphRewiring), [*Edwing Hancock*](https://ellisalicante.org/tutorials/GraphRewiring)
#### Panelists: [*Marika Zitnik*](https://ellisalicante.org/tutorials/GraphRewiring), [*Petar Veličković*](https://ellisalicante.org/tutorials/GraphRewiring), [*Francesco Di Giovanni*](https://ellisalicante.org/tutorials/GraphRewiring)

|Sections|
|-|
| [Installation](#installation)|
| [Code Explanation](#code-explanation)|
| [Slides](#slides)|
| [Tutorial Content](#tutorial-content)|
| [Troubleshooting](#troubleshooting)|
| [Aknowledgments](#aknowledgments) |


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

## Slides
**["Official Tutorial Web Page"](https://ellisalicante.org/tutorials/GraphRewiring)**

## Tutorial Content

<div class="table-responsive">
<table class="table table-bordered text-center table-striped">
  <thead>
    <tr>
      <th scope="col" class="text-right">Section</th>
      <th scope="col" class="text-left">Content</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th class="text-right align-middle">Introduction<br><small>10am ET (16:00 CET)</small></th>
      <td class="text-left align-middle">
      <ul>
        <li>Background and motivation</li>
        <li>Key challenges and Related Problems</li>
        <li>Basics of Spectral Theory</li>
        <ul> 
          <li>Laplacian Eigenfunctions</li>
          <li>Fiedler Vector and Dirichlet Energies</li>
          <li>Spectral Theorem</li>
          <li>Spectral Commute Times</li>
        </ul>
      </ul></td>
    </tr>
    <tr>
      <th class="text-right align-middle">Transductive Rewiring</th>
      <td class="text-left align-middle">
      <ul> 
        <li>Diffusive Rewiring</li>
        <li>Curvature-Based Rewiring</li>
        <ul>
          <li>Cheeger Constant and over-squashing</li>
          <li>Definitions of Curvature</li>
        </ul>
        <li>Graph Structure Learning</li>
      </ul></td>
    </tr>
    <tr>
      <th class="text-right align-middle">Inductive Rewiring<br><span style="color:green">Hands-on</span></th>
      <td class="text-left align-middle">
      <ul>
        <li>The Lovász Bound</li>
        <li><b>CT-Layer</b></li>
        <ul>
          <li>Principled Sparsification and Dirichlet Energies</li>
          <li>CT as an Optimization Problem and its Relation with Eigenfunctions</li>
          <li>CT-Layer and its Loss function</li>
          <li>Implications</li>
          <ul>
            <li>Differentiable Curvature</li>
            <li>Stable Cheeger constant</li>
            <li>Node Classification. CT as diffusion or Positional Encoding.</li>
          </ul>
        </ul>
        <li><b>GAP-Layer</b></li>
        <ul>
          <li>Spectral Derivatives</li>
          <li>Learning the Fiedler vector</li>
        </ul>
      </ul></td>
    </tr>
    <tr>
      <th class="text-right align-middle">Graph Fairness</th>
      <td class="text-left align-middle">
      <ul>
        <li>Algorithmic Fairness Concepts</li>
        <li>Structure: a New Dimension</li>
        <li>Dyadic Fairness</li>
        <li>Graph Rewiring Methods for Fairness</li>
      </ul></td>
    </tr>
    <tr>
      <th class="text-right align-middle">Panel<br><small>12am-1pm ET<br> (18:00-19:00 CET)</small></th>
      <td class="text-left align-middle">
      <ul>
        <li>Nuria Oliver (Moderator)</li>
        <li>Marinka Zitnik</li>
        <li>Petar Veličković</li>
        <li>Francesco Di Giovanni</li>
      </ul></td>
    </tr>
    <tr>
      <th class="text-right align-middle">Q<span>&#38;</span>A</th>
      <td class="text-left align-middle">Questions</td>
    </tr>
  </tbody>
</table>
</div>

## Troubleshooting

In case that clicking the icon does not work, you can open it in COLLAB manually. To open the notebooks directly in COLLAB, go to the path of the notebook and change `https://github.com/[notebook_path]` to `https://colab.research.google.com/github/[notebook_path]`. For example, if you want to open `https://github.com/ellisalicante/GraphRewiring-Tutorial/blob/main/0-Spectral-Background.ipynb` in COLLAB, you should go to https://colab.research.google.com/github/ellisalicante/GraphRewiring-Tutorial/blob/main/0-Spectral-Background.ipynb

To generate such links in one click, you can use the [Open in Colab](https://chrome.google.com/webstore/detail/open-in-colab/iogfkhleblhcpcekbiedikdehleodpjo) Chrome extension.

**Contact adrian@ellisalicante.org**.

## Aknowledgments

A. Arnaiz-Rodriguez and N. Oliver are supported by a nominal grant received at the **ELLIS Unit Alicante Foundation** from the **Regional Government of Valencia in Spain** (Convenio Singular signed with Generalitat Valenciana, Conselleria d’Innovació, Universitats, Ciència i Societat Digital, Dirección General para el Avance de la Sociedad Digital). A. Arnaiz-Rodriguez is also funded by a grant by the **Banc Sabadell Foundation**. F. Escolano is funded by the project **RTI2018-096223-B-I00** of the Spanish Government. 
