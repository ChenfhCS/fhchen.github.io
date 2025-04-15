---
title: "DGC: Training Dynamic Graphs with Spatio-Temporal Non-Uniformity using Graph Partitioning by Chunks"
collection: publications
category: conferences
permalink: /publication/paper-3
excerpt: '<strong><u>Fahao Chen</u></strong>, Peng Li, and Celimuge Wu'
date: 2024-06-09
venue: 'ACM SIGMOD (CCF A)'
# slidesurl: 'http://academicpages.github.io/files/slides1.pdf'
paperurl: 'https://arxiv.org/pdf/2309.03523'
# bibtexurl: 'http://academicpages.github.io/files/bibtex1.bib'
# citation: 'Your Name, You. (2009). &quot;Paper Title Number 1.&quot; <i>Journal 1</i>. 1(1).'
---
Dynamic Graph Neural Network (DGNN) has shown a strong capability of learning dynamic graphs by exploiting both spatial and temporal features. Although DGNN has recently received considerable attention by AI community and various DGNN models have been proposed, building a distributed system for efficient DGNN training is still challenging. It has been well recognized that how to partition the dynamic graph and assign workloads to multiple GPUs plays a critical role in training acceleration. Existing works partition a dynamic graph into snapshots or temporal sequences, which only work well when the graph has uniform spatio-temporal structures. However, dynamic graphs in practice are not uniformly structured, with some snapshots being very dense while others are sparse. To address this issue, we propose DGC, a distributed DGNN training system that achieves a 1.25× - 7.52× speedup over the state-of-the-art in our testbed. DGC’s success stems from a new graph partitioning method that partitions dynamic graphs into chunks, which are essentially subgraphs with modest training workloads and few inter connections. This partitioning algorithm is based on graph coarsening, which can run very fast on large graphs. In addition, DGC has a highly efficient run-time, powered by the proposed chunk fusion and adaptive stale aggregation techniques. Extensive experimental results on 3 typical DGNN models and 4 popular dynamic graph datasets are presented to show the effectiveness of DGC.