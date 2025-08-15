Date: June-July 2025

**The complete project analysis and details are available in 'main.ipynb'**


**The datasets used for this project are available in the 'data/' folder**

<h1>Predicting Breast Cancer Diagnosis Using Cell Nuclei Morphology</h1>

This project focuses on building and evaluating a machine learning model to classify breast cancer diagnoses (malignant or benign) based on the morphology of cell nuclei specimens. The dataset comes from the Diagnostic Wisconsin Breast Cancer Database and was accessed via Kaggle (1). The dataset includes various features for cell morphology, including radius, texture, perimeter and symmetry. For each characteristic, the mean, standard error and worst/largest value were documented in separate features. Cell nuclei were observed using fine needle aspiration (FNA) of breast masses.

Malignant cell nuclei typically exhibit larger size and irregular shapes. Additional changes may include alterations in surface, volume, density, structure, and homogeneity (2). Prior research has linked specific cell morphologies to increased risk of metastasis and tumorigenicity(3) which facilitates widespread cancerous invasions to other organs such as bones, lungs, liver and brain (4). By integrating articifical intelligence and transforming the diagnosis process with machine learning models, identification of breast cancer identification can be performed more quickly and with greater precision, guided by historical data. This project aims to help patients receive faster diagnoses, support doctors' findings and increase the efficency in healthcare processes.

The model will be trained on cell nuclei morphology to classify samples as malignant or benign using classification-supervised machine learning. It can be used as a tool to efficiently classify samples. It will also highlight the most influential features contributing to the classification, thereby enhancing the interpretability of the output.

<h2>Project Takeaways:</h2>

* Best Model: Logistic regression (C = 100) achieved the highest performance for breast cancer diagnosis using the Wisconsin Breast Cancer Dataset. It delivered strong precision and recall (both approximately 0.99) and offers the added benefit of model interpretability for clinical explainability.

* Limitations: This project relies on historical data, which may carry biases related to specific population groups. As a result, the model's generalizability in real-world applications may be limited or misleading.

* Key Features: The most influential features in prediction were related to cell nucleus characteristics — particularly area (both worst and mean) and concave points (mean), which had the strongest impact on the model's decisions.


<h2>References</h2>

(1) Wolberg, W., Mangasarian, O., Street, N., & Street, W. (1993). *Breast Cancer Wisconsin (Diagnostic)* [Dataset]. UCI Machine Learning Repository. https://doi.org/10.24432/C5DW2B.
 
(2) Baba, A. I., & Câtoi, C. (2007). *Comparative oncology* (Chapter 3: Tumor cell morphology). The Publishing House of the Romanian Academy. https://www.ncbi.nlm.nih.gov/books/NBK9553/

(3) Conner, S. J., Guarin, J. R., Le, T. T., et al. (2024). Cell morphology best predicts tumorigenicity and metastasis *in vivo* across multiple TNBC cell lines of different metastatic potential. *Breast Cancer Research*, 26, 43. https://doi.org/10.1186/s13058-024-01796-8

(4) Liang, Y., Zhang, H., Song, X., & Yang, Q. (2020). Metastatic heterogeneity of breast cancer: Molecular mechanism and potential therapeutic targets. *Seminars in cancer biology*, 60, 14–27. https://doi.org/10.1016/j.semcancer.2019.08.012
