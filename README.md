# Machine Learning upon RDF Knowledge Graphs for drug safety: a case study on Reactome data

Welcome to the repository for the supplementary material associated with the poster "Machine Learning upon RDF Knowledge Graphs for drug safety: a case study on Reactome data" submitted to the MIE 2024 conference.

## Contents

This repository contains a single Jupyter Notebook file (`MIE.ipynb`) which includes the supplementary Python code that supports the findings and visualizations presented in the poster.

## Poster abstract

Artificial Intelligence (AI), particularly Machine Learning (ML), has gained attention for its potential in various domains. However, approaches integrating symbolic AI with ML on Knowledge Graphs have not gained significant focus yet. We argue that exploiting RDF/OWL semantics while conducting ML could provide useful insights. We present a use case using signaling pathways from the Reactome database to explore drug safety. Promising outcomes suggest the need for further investigation and collaboration with domain experts.

## Visual representation

### Hidden node logic and link prediction

```mermaid
graph LR
    A[Drug] -->|interacts with| B[Protein]
    B -->|part of| C[Pathway]
    C -->|involves| D[Gene]
    X[Another Interaction] --> E[Hidden Node]
    E -.->|potential link| B
    E -.->|potential link| C
    B -->|potential prediction| F[Drug Safety Indicator]
    D -->|potential prediction| F
```
In this diagram:

* Drug interacts with Protein, which is part of a Pathway.
* The Pathway involves a Gene.
* Another Interaction points to a Hidden Node.
* The Hidden Node represents potential undiscovered relationships.
* Hidden Node has potential links to both Protein and Pathway.
* Protein and Gene can potentially predict a Drug Safety Indicator.

## Requirements

The Jupyter Notebook includes all the necessary code to install the required packages in the initial cells. The key dependency is:
- `mowl-borg`

## Usage

1. Clone this repository:
    ```bash
    git clone https://github.com/inab-certh/MIE2024---Machine-Learning-and-Knowledge-Graphs.git
    ```
2. Navigate to the repository directory:
    ```bash
    cd MIE2024---Machine-Learning-and-Knowledge-Graphs
    ```
3. Open the Jupyter Notebook:
    ```bash
    jupyter notebook MIE.ipynb
    ```
4. Run the cells in the notebook to reproduce the results and visualizations presented in the poster.

## Conference

This work is presented at the MIE 2024 conference. For more information about the conference, visit the [MIE 2024 website](https://mie2024.org/).

## Authors

- **Kalliopi Kastampolidou** - Institute of Applied Biosciences, Centre for Research & Technology Hellas, Thermi, Thessaloniki, Greece. [ORCID](https://orcid.org/0000-0003-3607-9569)
- **George I. Gavriilidis** - Institute of Applied Biosciences, Centre for Research & Technology Hellas, Thermi, Thessaloniki, Greece. [ORCID](https://orcid.org/0000-0003-2575-4354)
- **Pantelis Natsiavas** - Institute of Applied Biosciences, Centre for Research & Technology Hellas, Thermi, Thessaloniki, Greece. [ORCID](https://orcid.org/0000-0002-4061-9815)

## Contact

For any questions or further information, please contact Dr. Kalliopi Kastampolidou at [kkastampolidou@certh.gr](mailto:kkastampolidou@certh.gr).

---

Thank you for your interest in our work!
