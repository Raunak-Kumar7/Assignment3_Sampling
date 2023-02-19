# Comparing Sampling Techniques for 5 Machine Learning Models

## Introduction

The objective of this project is to investigate various sampling techniques that can be used to generate a balanced dataset for a machine learning model. The original dataset is imbalanced, and to address this, both random over-sampling and under-sampling methods are employed. Subsequently, five distinct sampling techniques are employed on the balanced dataset, and the resulting samples' accuracies are evaluated using five different machine learning models.

## Sampling Techniques

The following five sampling techniques were used in this project:

1. **Simple Random Sampling:** A basic sampling technique where each data point in the dataset has an equal probability of being selected in the sample.

2. **Stratified Sampling:** A sampling technique where the population is divided into subgroups (strata) based on a specific characteristic, and samples are taken from each stratum in proportion to the population.

3. **Systematic Sampling:** A sampling technique where every nth element in the population is selected for the sample, with n being a fixed interval.

4. **Cluster Sampling:** A sampling technique where the population is divided into clusters, and a sample of clusters is randomly selected. Then, all members of the selected clusters are included in the sample.

5. **Convenience Sampling:** A non-probability sampling technique where the sample is chosen based on its convenience to the researcher.

## Comparison Table

The table below shows the accuracies of each sampling technique on five different machine learning models. The dataset used for all models is a balanced version of the original unbalanced dataset using random over-sampling and under-sampling techniques.

| Sampling Technique | Decision Tree | SVM | Logistic Resgression | KNN | Naive Bayes |
|:---------------:|:---------------:|:---------------:|:---------------:|:---------------:|:---------------:|
| Simple Random Sampling | 0.9778 | 0.8954 | 0.8917 | 0.8915 | 0.7275 |
| Systematic Sampling | 0.9813 | 0.8989 | 0.9213 | 0.9493 | 0.6854 |
| Stratified Sampling | 0.9851 | 0.8937 | 0.9217 | 0.9498 | 0.6890 |
| Cluster Sampling | **0.9868** | 0.9000 | 0.9088 | 0.9691 | 0.9235 |
| Convenience Sampling | 0.9849 | 0.9190 | 0.9322 | 0.9623 | 0.7740 |

The findings suggest that Cluster Sampling outperforms all other sampling techniques on all five machine learning models, while Simple Random Sampling performs the worst across all models. The remaining sampling techniques exhibit mixed performance depending on the model being used. Furthermore, the results indicate that the Decision Tree model yields the highest accuracy for all five samples.

## Conclusion

The recommended approach for this dataset is to use cluster sampling, as it consistently outperforms other sampling techniques across all models. However, it may be worthwhile to explore alternative sampling methods for different datasets or models.
 
