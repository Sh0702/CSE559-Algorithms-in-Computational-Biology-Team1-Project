# CSE559-Algorithms-in-Computational-Biology-Team1-Project
CSE 559 - Algorithms in Computational Biology Team 1(A6+B)

# Team Members:
1. Shreyas Srinivasan - 1229139888
2. Praveen Raj Mohanraj - 1229519956
3. Mohankrishna Chandrasekhar - 
4. Ganeshkumar Govindaraju - 
5. Pooja Laxmi Shanmuganathan - 

# Overview
This GitHub project presents a comprehensive study on the effectiveness of the TCRBert model for Amino Acid Embedding. The evaluation involved comparing the baseline TCRBert model with various modifications aimed at improving its performance. The primary focus was on four enhancement methods: regularization, reducing dropout, changing the number of layers, and adjusting the learning rate. The project concludes that adjusting the number of layers is the most effective approach, enhancing connections between nodes, particularly beneficial given the ample amount of available data.

# Dataset
The study utilized a dataset named "TCREpitopePairs.csv," comprising 300,016 data points. Each data point included unique TCR (T-cell receptor), epitope, and binding information. This rich dataset served as the foundation for evaluating the TCRBert model and its variations.

# Model Enhancements
1. Regularization
Introduces regularization techniques to mitigate overfitting and improve model generalization.

2. Dropout Reduction
Examines the impact of reducing dropout rates on model training and performance.

3. Number of Layers Adjustment
Identifies adjusting the number of layers as the most effective enhancement, enhancing connections between nodes in response to the extensive dataset.

4. Learning Rate Adjustment
Explores the effects of adjusting the learning rate on model convergence and accuracy.

Amino Acid Embedding
For Amino Acid Embedding, a variant of TCRBert was employed and compared against the original TCRBert. This comparative analysis provides insights into the relative performance of TCRBert concerning other models in the context of Amino Acid Embedding.

# Code
The code for this project, including model implementation, enhancements, and comparative analysis, is provided in the repository. Please refer to the project files for detailed information on implementation and execution.

# Usage
Clone the repository:
git clone https://github.com/Sh0702/CSE559-Algorithms-in-Computational-Biology-Team1-Project.git 

cd tcrbert-enhancement-project

Follow the instructions in the code documentation to replicate the experiments and explore the findings.

# Results
The project outcomes provide a comparative study on the effectiveness of TCRBert in Amino Acid Embedding compared to other models. The identified best practices for model enhancement offer valuable insights for optimizing TCRBert's performance in various scenarios.

Feel free to contribute, raise issues, or provide feedback to further enhance this research project.

# Citation
# Context-Aware Amino Acid Embedding (catELMo)

This section introduces the catELMo model, a context-aware amino acid embedding designed for advancing the analysis of TCR-epitope interactions. The associated article is available on bioRxiv.

```bibtex
@article {catelmobiorxiv,
	author = {Pengfei Zhang and Seojin Bang and Michael Cai and Heewook Lee},
	title = {Context-Aware Amino Acid Embedding Advances Analysis of TCR-Epitope Interactions},
	elocation-id = {2023.04.12.536635},
	year = {2023},
	doi = {10.1101/2023.04.12.536635},
	publisher = {Cold Spring Harbor Laboratory},
	journal = {bioRxiv}
}
```

# TCRBert

This section provides information on the TCRBert model and its significance in identifying specificity groups within the T-cell receptor repertoire. The model is introduced through the following references:

1. Glanville, J., et al. (2017). Identifying specificity groups in the T cell receptor repertoire. Nature, 547(7661), 94–98.

2. Devlin, J., et al. (2019). BERT: Pre-training of deep bidirectional transformers for language understanding. Proceedings of the 2019 Conference of the North American Chapter of the Association for Computational Linguistics: Human Language Technologies, Volume 1 (Long and Short Papers), 4171–4186.
