# CSE559-Algorithms-in-Computational-Biology-Team1-Project
Link for models: https://drive.google.com/drive/folders/1zLLbGb9PtOCs2VoD15dQ_eRUHYXWE3nT?usp=sharing

# Team Members:
1. Shreyas Srinivasan - 1229139888
2. Praveen Raj Mohanraj - 1229519956
3. Mohankrishna Chandrasekhar - 1219474685
4. Ganeshkumar Govindaraju - 1229782322
5. Pooja Laxmi Shanmuganathan - 1229598957

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

tcr-bert-finetuned-tchard
This model is a fine-tuned version of wukevin/tcr-bert on the TChard dataset. It achieves the following results on the evaluation set:

Loss: 0.7212
Perplexity: 11.32

Model can be found at Part A folder

# Code
The code for this project, including model implementation, enhancements, and comparative analysis, is provided in the repository. Please refer to the project files for detailed information on implementation and execution.

# Usage
Clone the repository:
git clone https://github.com/Sh0702/CSE559-Algorithms-in-Computational-Biology-Team1-Project.git 

cd tcrbert-enhancement-project

Follow the instructions in the code documentation to replicate the experiments and explore the findings.

# Performance

Baseline Model:
1. AUC: 0.6536143979534137
2. precision_recall_fscore_macro (0.6116898028620932, 0.6098090931880342, 0.6082848407042718, None)
3. accuracy is 0.6100182565038795
4. precision1 is 0.6245672925626771
5. precision0 is 0.5988123131615093
6. recall1 is 0.5452630614954898
7. recall0 is 0.6743551248805787
8. f1macro is 0.6082848407042718
9. f1micro is 0.6100182565038795

Custom Model:
1. AUC: 0.6720369844364315
2. precision_recall_fscore_macro (0.6347539702855138, 0.6323815574010831, 0.6302615384287922, None)
3. accuracy is 0.6526243724326792
4. precision1 is 0.6489017837954008
5. precision0 is 0.6206061567756268
6. recall1 is 0.5574508906085443
7. recall0 is 0.7173122241936218
8. f1macro is 0.5902615384287922
9. f1micro is 0.6026243724326792

# Results
The project outcomes provide a comparative study on the effectiveness of TCRBert in Amino Acid Embedding compared to other models. The identified best practices for model enhancement offer valuable insights for optimizing TCRBert's performance in various scenarios.

# Future Work

1. Embeddings Exploration:
The success of the model heavily relies on the quality of embeddings. While we initially used TCRBert with pretrained weights and fine-tuning, we hypothesize that training the TCRBert model from scratch could yield superior results. This avenue will be explored to unlock the full potential of the model.

2. Activation Layer Modification:
The activation layer plays a crucial role in shaping the model's behavior. In this work, we propose experimenting with Rectified Linear Unit (ReLU) as an alternative to the existing siLU activation layer. The impact of this modification will be assessed to determine its influence on the model's performance.

3. Layer-Specific Activation Experimentation:
Recognizing the varying importance of activation functions across different layers, we plan to conduct experiments using both ReLU and siLU activations. By tailoring the activation layers to specific model layers, we aim to identify optimal configurations that enhance the model's expressive capabilities.


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
