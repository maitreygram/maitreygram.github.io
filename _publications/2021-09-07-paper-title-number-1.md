---
title: "CuRL: Coupled Representation Learning of Cards and Merchants to Detect Transaction Frauds"
collection: publications
permalink: /publications/CuRL
excerpt: 'In this paper, we propose CuRL and tCuRL, coupled representation learning methods that can effectively capture the higher-order interactions in a bipartite graph of payment entities to detect transaction fraud.'
date: 2021-09-07
venue: '30th International Conference on Artificial Neural Networks (ICANN)'
paperurl: 'https://link.springer.com/chapter/10.1007/978-3-030-86383-8_2'
---

<style>

/* Style the counter cards */
.card {
<!--   box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2); /* this adds the "card" effect */ -->
  padding: 16px;
<!--   text-align: center; -->
<!--   background-color: #f1f1f1; -->
}

a:link {
  text-decoration: none;
}
</style>

<div class="card">
  <img src="https://user-images.githubusercontent.com/24911348/195767144-15cb4b40-5808-4739-9d87-657bdf465190.png" alt="CuRL system diagram"/>
</div>

Payment networks like Mastercard or Visa process billions of transactions every year. A significant number of these transactions are fraudulent that cause huge losses to financial institutions. Conventional fraud detection methods fail to capture higher-order interactions between payment entities i.e., cards and merchants, which could be crucial to detect out-of-pattern, possibly fraudulent transactions. Several works have focused on capturing these interactions by representing the transaction data either as a bipartite graph or homogeneous graph projections of the payment entities. In a homogeneous graph, higher-order cross-interactions between the entities are lost and hence the representations learned are sub-optimal. In a bipartite graph, the sequences generated through random walk are stochastic, computationally expensive to generate, and sometimes drift away to include uncorrelated nodes. Moreover, scaling graph-learning algorithms and using them for real-time fraud scoring is an open challenge.

In this paper, we propose CuRL and tCuRL, coupled representation learning methods that can effectively capture the higher-order interactions in a bipartite graph of payment entities. Instead of relying on random walks, proposed methods generate coupled session-based interaction pairs of entities which are then fed as input to the skip-gram model to learn entity representations. The model learns the representations for both entities simultaneously and in the same embedding space, which helps to capture their cross-interactions effectively. Furthermore, considering the session constrained neighborhood structure of an entity makes the pair generation process efficient. This paper demonstrates that the proposed methods run faster than many state-of-the-art representation learning algorithms and produce embeddings that outperform other relevant baselines on fraud classification task.

[paper link](https://link.springer.com/chapter/10.1007/978-3-030-86383-8_2)

Cite this paper as:
<pre>
  <code>
    @article{gramopadhye2021curl,
    author="Gramopadhye, Maitrey and Singh, Shreyansh and Agarwal, Kushagra and Srivasatava, Nitish and Singh, Alok Mani and Asthana, Siddhartha and Arora, Ankur",
    title="CuRL: Coupled Representation Learning of Cards and Merchants to Detect Transaction Frauds",
    booktitle="Artificial Neural Networks and Machine Learning -- ICANN 2021",
    year="2021",
    publisher="Springer International Publishing",
    pages="16--29",
    isbn="978-3-030-86383-8"
    }
  </code>
</pre>
