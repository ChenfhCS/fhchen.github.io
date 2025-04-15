---
title: "TCB: Accelerating Transformer Inference Services with Request Concatenation"
collection: publications
category: conferences
permalink: /publication/paper-5
excerpt: 'Boqian Fu, Fahao Chen, Peng Li, and Deze Zeng'
date: 2023-01-13
venue: 'ACM ICPP (CCF B)'
paperurl: 'https://chenfhcs.github.io/fhchen.github.io/files/TCB_ACM_ICPP.pdf'
# citation: 'Your Name, You. (2024). &quot;Paper Title Number 3.&quot; <i>GitHub Journal of Bugs</i>. 1(3).'
---

Transformer has dominated the field of natural language processing because of its strong capability in learning from sequential input data. In recent years, various computing and networking optimizations have been proposed for improving transformer training efficiency. However, transformer inference, as the core of many AI services, has been seldom studied. A key challenge of transformer inference is variable-length input. In order to align these input, existing work has proposed batching schemes by padding zeros, which unfortunately introduces significant computational redundancy. Moreover, existing transformer inference studies are separated from the whole serving system, where both request batching and request scheduling are critical and they have complex interaction. To fill the research gap, we propose TCB, a Transformer inference system with a novel ConcatBatching scheme as well as a jointly designed online scheduling algorithm. ConcatBatching minimizes computational redundancy by concatenating multiple requests, so that batch rows can be aligned with reduced padded zeros. Moreover, we conduct a systemic study by designing an online request scheduling algorithm aware of ConcatBatching. This scheduling algorithm needs no future request information and has provable theoretical guarantee. Experimental results show that TCB can significantly outperform state-of-the-art.
