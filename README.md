# GLAD: Gossip Learning in Heterogeneous Networks

## Abstract

Federated Learning (FL) has recently grown up significantly, due to the looming needs of privacy among companies or institutions and the rapid development of powerful devices that makes Edge Computing advantageous.
Current research on FL is mainly focused on privacy and performance improving, and researchers are often dealing with one metric per time, leaving open the issues concerning the integration between the diversity in data quality, in resources capability and network topology, which characterizes highly heterogeneous networks.
In this paper, we firstly analyze Federated Learning, presenting some use cases and applications, the metrics involved and its different types of architecture.
Therefore, we propose GLAD (Gossip Learning Averaging Distance), a totally decentralized and synchronous system, based on gossip fashion, which aims to introduce metrics, such as resource capability and data quality, in aggregating several models. By computing a score for each node based on the metrics, we present a weighted averaging process that is effectively executed only when the Euclidean distance among the weights of neurons with the same coordinates between different nodes is under a certain threshold.
This allows to achieve better performance, in terms of global accuracy, in particularly heterogeneous networks compared to other traditional FL algorithms, advantaging nodes with better resources and data quality over poorer nodes during the merging step.
Furthermore, we discuss how performance changes respect to the network topology and to variation of the analyzed metrics.

## Content



## License

The project is available as open source under the terms of the [GPL License](https://opensource.org/licenses/GPL-3.0).