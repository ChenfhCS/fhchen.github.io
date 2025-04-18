---
title: "Hare: Exploiting Inter-job and Intra-job Parallelism of Distributed Machine Learning on Heterogeneous GPUs"
collection: publications
category: conferences
permalink: /publication/paper-4
excerpt: '<strong><u>Fahao Chen</u></strong>, Peng Li, Celimuge Wu, and Song Guo'
date: 2022-06-27
venue: 'ACM HPDC (CCF B)'
paperurl: 'https://chenfhcs.github.io/fhchen.github.io/files/Hare_ACM_HPDC.pdf'
# citation: 'Your Name, You. (2024). &quot;Paper Title Number 3.&quot; <i>GitHub Journal of Bugs</i>. 1(3).'
---

Distributed machine learning (DML) has shown great promise in accelerating model training on multiple GPUs. To increase GPU utilization, a common practice is to let multiple learning jobs share GPU clusters, where the most fundamental and critical challenge is how to efficiently schedule these jobs on GPUs. However, existing works about DML job scheduling are constrained to settings with homogeneous GPUs. GPU heterogeneity is common in practice, but its influence on multiple DML job scheduling has been seldom studied. Moreover, DML jobs have internal structures that contain great parallelism potentials, which have not yet been fully exploited in the heterogeneous computing environment. In this paper, we propose Hare, a DML job scheduler that exploits both inter-job and intra-job parallelism in a heterogeneous GPU cluster. Hare has three novel designs. First, Hare optimizes GPU execution environment to reduce task switching overhead by exploiting unique features of DML scheduling. Second, Hare adopts a relaxed fixed-scale synchronization scheme that allows independent tasks to be flexibly scheduled within a training round. Finally, we propose a fast heuristic algorithm to minimize the total weighted job completion time by jointly considering job features and hardware heterogeneity. Its theoretical bound is derived. We evaluate Hare using a small-scale testbed and a trace-driven simulator. The results show that it can outperform the state-of-the-art by about 2x.
