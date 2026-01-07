---
title: "Augmenting biomedical named entity recognition with general-domain resources"
collection: publications
permalink: /publication/2024-10-04-bioner-gerbera
date: 2024-10-04
venue: 'Journal of Biomedical Informatics'
paperurl: 'https://doi.org/10.1016/j.jbi.2024.104731'
codeurl: "https://github.com/qingyu-qc/bioner_gerbera"
citation: 'Yu Yin*,  Hyunjae Kim*, Xiao Xiao, Chih Hsuan Wei, Jaewoo Kang, Zhiyong Lu, Hua Xu, Meng Fang, Qingyu Chen.'
abstract: 'Training a neural network-based biomedical named entity recognition (BioNER) model usually requires extensive and costly human annotations. While several studies have employed multi-task learning with multiple BioNER datasets to reduce human effort, this approach does not consistently yield performance improvements and may introduce label ambiguity in different biomedical corpora. We aim to tackle those challenges through transfer learning from easily accessible resources with fewer concept overlaps with biomedical datasets. We proposed GERBERA, a simple-yet-effective method that utilized general-domain NER datasets for training. We performed multi-task learning to train a pre-trained biomedical language model with both the target BioNER dataset and the general-domain dataset. Subsequently, we fine-tuned the models specifically for the BioNER dataset. We systematically evaluated GERBERA on five datasets of eight entity types, collectively consisting of 81,410 instances. Despite using fewer biomedical resources, our models demonstrated superior performance compared to baseline models trained with additional BioNER datasets. Specifically, our models consistently outperformed the baseline models in six out of eight entity types, achieving an average improvement of 0.9% over the best baseline performance across eight entities. Our method was especially effective in amplifying performance on BioNER datasets characterized by limited data, with a 4.7% improvement in F1 scores on the JNLPBA-RNA dataset. This study introduces a new training method that leverages cost-effective general-domain NER datasets to augment BioNER models. This approach significantly improves BioNER model performance, making it a valuable asset for scenarios with scarce or costly biomedical datasets.'
tags: ['Biomedical NLP']
image: '/images/gerbera_abstract.jpg'
---
