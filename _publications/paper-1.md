---
title: "SPIN: Accelerating Large Language Model Inference with Heterogeneous Speculative Models"
collection: publications
category: conferences
permalink: /publication/paper-1
excerpt: '<strong><u>Fahao Chen</u></strong>, Peng Li, Tom H. Luan, Zhou Su, and Jing Deng'
date: 2025-05-19
venue: 'IEEE International Conference on Computer Communications (CCF A)'
# slidesurl: 'http://academicpages.github.io/files/slides1.pdf'
paperurl: 'https://arxiv.org/pdf/2503.15921'
# bibtexurl: 'http://academicpages.github.io/files/bibtex1.bib'
# citation: 'Your Name, You. (2009). &quot;Paper Title Number 1.&quot; <i>Journal 1</i>. 1(1).'
---
Speculative decoding has been shown as an effective way to accelerate Large Language Model (LLM) inference by using a Small Speculative Model (SSM) to generate candidate tokens in a so-called speculation phase, which are subsequently verified by the LLM in a verification phase. However, current state-of-the-art speculative decoding approaches have three key limitations: handling requests with varying difficulty using homogeneous SSMs, lack of robust support for batch processing, and insufficient holistic optimization for both speculation and verification phases. In this paper, we introduce SPIN, an efficient LLM inference serving system based on speculative decoding, designed to address these challenges through three main innovations. First, SPIN improves token speculation by using multiple heterogeneous SSMs, with a learning-based algorithm for SSM selection that operates without prior knowledge of request difficulty. Second, SPIN employs a request decomposition method to minimize batching overhead during LLM verification. Finally, SPIN orchestrates speculation and verification phases by pipelining their executions on GPUs to achieve further acceleration. Experimental results demonstrate that SPIN significantly outperforms state-of-the-art methods, achieving a performance increase of approximately 2.28×.
