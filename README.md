
# Aspect Sentiment Triplet Extraction Task
[AAAI 2020] [Knowing What, How and Why: A Near Complete Solution for Aspect-based Sentiment Analysis (In AAAI 2020)](https://arxiv.org/pdf/1911.01616.pdf)


[EMNLP 2020] [Position-Aware Tagging for Aspect Sentiment Triplet Extraction (In EMNLP 2020)](https://arxiv.org/abs/2010.02609)

- Please refer to this **[site](https://github.com/xuuuluuu/Position-Aware-Tagging-for-ASTE)** for source code.




# UPDATE on Sep 2020
The files in the **ASTE-Data-V2-EMNLP2020** folder are the refined data. We remove triplets that have conflicting sentiments in both training, validation and test sets and also append the gold triplets at the end of each sentence to ease the triplet evaluation. We also remove the tagged sentences from the the previous ASTE-Data-V1 data released in AAAI-2020, as the tagging format results in incomplete aspect sentiment triplets. 

The data has the following format: 

> sentence####[(target position, opinion position, sentiment)]

If there are multiple triplets in the same sentence:

> sentence####[(target position, opinion position, sentiment), ..., (target position, opinion position, sentiment)]

For example:

> The screen is very large and crystal clear with amazing colors and resolution .####[([1], [4], 'POS'), ([1], [7], 'POS'), ([10], [9], 'POS'), ([12], [9], 'POS')]
