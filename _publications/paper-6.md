---
title: "Non-Clairvoyant Scheduling of Distributed Machine Learning With Inter-Job and Intra-Job Parallelism on Heterogeneous GPUs"
collection: publications
category: manuscripts
permalink: /publication/paper-6
excerpt: '<strong><u>Fahao Chen</u></strong>, Peng Li, Celimuge Wu, and Song Guo'
date: 2024-06-14
venue: 'IEEE TCC (CCF C)'
paperurl: 'https://chenfhcs.github.io/fhchen.github.io/Scheduling_IEEE_TCC.pdf'
# citation: 'Your Name, You. (2024). &quot;Paper Title Number 3.&quot; <i>GitHub Journal of Bugs</i>. 1(3).'
---

Distributed machine learning (DML) has shown great promise in accelerating model training on multiple GPUs. To increase GPU utilization, a common practice is to let multiple learning jobs share GPU clusters, where the most fundamental and critical challenge is how to efficiently schedule these jobs on GPUs. However, existing works about DML job scheduling are constrained to settings with homogeneous GPUs. GPU heterogeneity is common in practice, but its influence on multiple DML job scheduling has been seldom studied. Moreover, DML jobs have internal structures that contain great parallelism potentials, which have not yet been fully exploited in the heterogeneous computing environment. In this paper, we propose Hare, a DML job scheduler that exploits both inter-job and intra-job parallelism in a heterogeneous GPU cluster. Hare adopts a relaxed fixed-scale synchronization scheme that allows independent tasks to be flexibly scheduled within a training round. Given full knowledge of job arrival time and sizes, we propose a fast heuristic algorithm to minimize the average job completion time and derive its theoretical bound is derived.Without prior knowledge of jobs, we propose an online algorithm based on the Heterogeneity-aware Least-Attained Service (HLAS) policy.We evaluate Hare using a small-scale testbed and a trace-driven simulator. The results show that it can outperform the state-of-the-art, achieving a performance improvement of about 2.94×.
