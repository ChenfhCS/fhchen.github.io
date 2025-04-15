---
title: "FedGraph: Federated Graph Learning With Intelligent Sampling"
collection: publications
category: manuscripts
permalink: /publication/paper-7
excerpt: '<strong><u>Fahao Chen</u></strong>, Peng Li, Toshiaki Miyazaki, and Celimuge Wu'
date: 2022-08-01
venue: 'IEEE TPDC (CCF A)'
paperurl: 'https://chenfhcs.github.io/fhchen.github.io/files/FedGraph_IEEE_TPDS.pdf'
# citation: 'Your Name, You. (2024). &quot;Paper Title Number 3.&quot; <i>GitHub Journal of Bugs</i>. 1(3).'
---

Federated learning has attracted much research attention due to its privacy protection in distributed machine learning. However, existing work of federated learning mainly focuses on Convolutional Neural Network (CNN), which cannot efficiently handle graph data that are popular in many applications. Graph Convolutional Network (GCN) has been proposed as one of the most promising techniques for graph learning, but its federated setting has been seldom explored. In this article, we propose FedGraph for federated graph learning among multiple computing clients, each of which holds a subgraph. FedGraph provides strong graph learning capability across clients by addressing two unique challenges. First, traditional GCN training needs feature data sharing among clients, leading to risk of privacy leakage. FedGraph solves this issue using a novel cross-client convolution operation. The second challenge is high GCN training overhead incurred by large graph size.We propose an intelligent graph sampling algorithm based on deep reinforcement learning, which can automatically converge to the optimal sampling policies that balance training speed and accuracy.We implement FedGraph based on PyTorch and deploy it on a testbed for performance evaluation. The experimental results of four popular datasets demonstrate that FedGraph significantly outperforms existing work by enabling faster convergence to higher accuracy.
