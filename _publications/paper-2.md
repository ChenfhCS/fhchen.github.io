---
title: "MELL: Memory-Efficient Large Language Model Serving via Multi-GPU KV Cache Management"
collection: publications
category: conferences
permalink: /publication/paper-2
excerpt: 'Qianli Liu, Zicong Hong, Peng Li, Fahao Chen, and Song Guo'
date: 2025-05-19
venue: 'IEEE International Conference on Computer Communications (CCF A)'
# slidesurl: 'http://academicpages.github.io/files/slides1.pdf'
paperurl: 'https://arxiv.org/pdf/2501.06709'
# bibtexurl: 'http://academicpages.github.io/files/bibtex1.bib'
# citation: 'Your Name, You. (2009). &quot;Paper Title Number 1.&quot; <i>Journal 1</i>. 1(1).'
---
Serving large language models (LLMs) for massive users is challenged by the significant memory footprint of the transient state, known as the key-value (KV) cache, which scales with sequence length and number of requests. Instead of renting or buying more expensive GPUs, the load imbalance of the KV cache across GPUs, coupled with recent advances in inter-GPU communication, provides an opportunity to serve more requests via request migration. However, high migration overhead and unpredictable request patterns make it challenging. Therefore, this paper proposes MELL, a memory-efficient LLM serving system via multi-GPU KV cache management. It saves the number of GPUs needed in the system by considering the dynamic KV cache load and the costly request migration. Specifically, we first develop an adaptive request migration mechanism to balance the computational and communication overheads and adapt to diverse resource conditions. Then, we design an online algorithm tailored to a multi-LLM request and multi-GPU scheduling problem with migration enabled. It aims to minimise the required GPUs while limiting the number of migrations. Finally, we implement a prototype of MELL and demonstrate that it reduces the number of GPUs by 31% and increases the GPU utilization by 43% at most compared to existing LLM serving systems.