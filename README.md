<div id="top"></div>

[![Contributors][contributors-shield]][contributors-url]
[![GPL License][license-shield]][https://opensource.org/licenses/GPL-3.0]

<br />
<div align="center">
<h3 align="center">GLAD: Gossip Learning Averaging Distance</h3>
  <p align="center">
    Federated Learning in Heterogeneous Networks
  </p>
</div>

<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li><a href="#abstract">Abstract</a></li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#installation">Installation</a></li>
      </ul>
    </li>
    <li><a href="#usage">Usage</a></li>
    <li><a href="#contributing">Contributing</a></li>
    <li><a href="#license">License</a></li>
    <li><a href="#contacts">Contacts</a></li>
  </ol>
</details>

## Abstract

>Federated Learning (FL) has recently grown up significantly, due to the looming needs of privacy among companies or institutions and the rapid development of powerful devices that makes Edge Computing advantageous.
>Current research on FL is mainly focused on privacy and performance improving, and researchers are often dealing with one metric per time, leaving open the issues concerning the integration between the diversity in data quality, in resources capability and network topology, which characterizes highly heterogeneous networks.
>In this paper, we firstly analyze Federated Learning, presenting some use cases and applications, the metrics involved and its different types of architecture.
>Therefore, we propose GLAD (Gossip Learning Averaging Distance), a totally decentralized and synchronous system, based on gossip fashion, which aims to introduce metrics, such as resource capability and data quality, in aggregating several models. By computing a score for each node based on the metrics, we present a weighted averaging process that is effectively executed only when the Euclidean distance among the weights of neurons with the same coordinates between different nodes is under a certain threshold.
>This allows to achieve better performance, in terms of global accuracy, in particularly heterogeneous networks compared to other traditional FL algorithms, advantaging nodes with better resources and data quality over poorer nodes during the merging step.
>Furthermore, we discuss how performance changes respect to the network topology and to variation of the analyzed metrics.

<p align="right">(<a href="#top">back to top</a>)</p>


## Getting Started

The repository contains two [Jupyter](https://jupyter.org) notebooks, [node.ipynb](https://github.com/matteosz/GLAD/blob/Tank/node.ipynb) which is used to create and populate the network given the metrics and the dataset and [merge.ipynb](https://github.com/matteosz/GLAD/blob/Tank/merge.ipynb), which is responsable of the aggregation phase.

### Prerequisites

#### Packages required
- [numpy](https://numpy.org/install)
- [pandas](https://pandas.pydata.org/getting_started.html)
- [tensorflow](https://www.tensorflow.org/install)
- [sklearn](https://scikit-learn.org/stable/install.html)

[Jupyter Lab](https://jupyter.org/install) is not required, however it's highly recommended.

### Installation

1. Clone the repo
   ```sh
   git clone https://github.com/matteosz/GLAD
   ```
2. Open [node.ipynb](https://github.com/matteosz/GLAD/blob/Tank/node.ipynb) and configure the setup by tuning the parameters and choosing dataset.
3. Run all cells in [node.ipynb](https://github.com/matteosz/GLAD/blob/Tank/node.ipynb) to create the network on your local device.

<p align="right">(<a href="#top">back to top</a>)</p>

## Usage

After the initial setup, open [merge.ipynb](https://github.com/matteosz/GLAD/blob/Tank/merge.ipynb) and tune hyperparameters and parameters as well, before to run any cell. The notebook is, by default, set to overwrite the old models with the new merged ones, in order to save space, but this feature can be easily changed by specifying a different path. Moreover, the two notebooks are conceived to be used separately, so to conduct more rounds of GLAD you'll need to switch back to [node.ipynb](https://github.com/matteosz/GLAD/blob/Tank/node.ipynb) after the merging and, instead of creating a new model from scratch, you need to load the current ones. Thereafter, you can continue training and saving again the models to repeat the process.

<p align="right">(<a href="#top">back to top</a>)</p>

## Contributing

Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

<p align="right">(<a href="#top">back to top</a>)</p>

## License

Distributed under the GNU License. See [LICENSE](https://github.com/matteosz/GLAD/blob/Tank/LICENSE) for more information.

<p align="right">(<a href="#top">back to top</a>)</p>

<!-- CONTACT -->
## Contacts

Matteo Suez - matteosuez@libero.it
Frédéric Le Mouël - frederic.le-mouel@insa-lyon.fr

Project Link: [https://github.com/matteosz/GLAD](https://github.com/matteosz/GLAD)

<p align="right">(<a href="#top">back to top</a>)</p>


[contributors-shield]: https://img.shields.io/github/contributors/matteosz/GLAD.svg?style=for-the-badge
[forks-shield]: https://img.shields.io/github/forks/matteosz/GLAD.svg?style=for-the-badge
[stars-shield]: https://img.shields.io/github/stars/matteosz/GLAD.svg?style=for-the-badge
[issues-shield]: https://img.shields.io/github/issues/matteosz/GLAD.svg?style=for-the-badge
[license-shield]: https://img.shields.io/github/license/matteosz/GLAD.svg?style=for-the-badge
[license-url]: https://github.com/matteosz/GLAD/blob/Tank/LICENSE
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://linkedin.com/in/matteo-suez