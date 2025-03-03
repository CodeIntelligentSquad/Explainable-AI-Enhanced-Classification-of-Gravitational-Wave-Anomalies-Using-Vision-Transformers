# Gravitational Wave Classification with Machine Learning, Vision Transformers, and Explainable AI (XAI)

## Project Overview

This project focuses on classifying gravitational wave signals using a combination of image and tabular data. The dataset used is the Gravity Spy dataset, which includes spectrogram images and metadata features such as frequency and amplitude. The goal is to enhance classification performance by leveraging Vision Transformer (ViT) and Swin Transformer feature extractors, followed by machine learning models.

## Dataset

The dataset used in this study was collected by LIGO (Laser Interferometer Gravitational-Wave Observatory).
The dataset consists of:

- Spectrogram Images: Visual representations of gravitational wave events.

- Tabular Data: Metadata features including peak frequency, bandwidth, signal-to-noise ratio (SNR), and other relevant attributes.

 The dataset contains 22 unique classes representing different types of gravitational wave anomalies.
## Methodology

1- Data Preprocessing:

- Load metadata from CSV files.

- Extract key tabular features and encode labels.

- Load and preprocess spectrogram images (resize to 224×224, normalize values).

2- Feature Extraction:

- Use Vision Transformer (ViT) and Swin Transformer models to extract high-level features from images.

- Combine extracted image features with tabular data.

3- Model Training:

- Train traditional machine learning models (ANN, Random Forest, Decision Tree, SVM, XGBoost) on the combined feature set.

- Perform 5-fold cross-validation to evaluate performance.

4- Evaluation Metrics:
- Accuracy

- F1 Score

- Precision

- Recall

Pipeline

Below is the visual representation of the pipeline followed in this project:

![pipeline](https://github.com/user-attachments/assets/1ba4bacf-36da-4182-af08-537370ebd661)


## Explainable AI (XAI)

To improve the interpretability of our model predictions, we applied Explainable AI (XAI) techniques. The primary methods used include:

- SHAP (SHapley Additive exPlanations): Used to understand feature contributions and interactions in the model's decision-making process. The SHAP interaction plots highlight which features have the most significant influence.

![SHAP_Explanation](https://github.com/user-attachments/assets/23f92a13-07e6-4870-8758-0e4aac8093c5)


- LIME (Local Interpretable Model-agnostic Explanations): Applied to generate local explanations for individual predictions, showing which features contributed the most to a specific classification decision.

![lime_explanation](https://github.com/user-attachments/assets/d5c77699-242c-413f-a4ad-b8445adba772)


These techniques help provide transparency into the model's decision process, ensuring reliability and trust in our classification system.

## Scientific Explanation: What Are Gravitational Waves?

Gravitational waves are ripples in the fabric of spacetime caused by the acceleration of massive objects, such as merging black holes or neutron stars. First predicted by Albert Einstein in 1916 as a consequence of his General Theory of Relativity, these waves propagate at the speed of light, carrying energy away from their sources.

## How Do Gravitational Waves Form?

When massive objects, like black holes or neutron stars, orbit each other closely, they generate gravitational waves. These waves cause tiny distortions in space and time as they pass through the universe. The first direct detection of gravitational waves was made in 2015 by the LIGO (Laser Interferometer Gravitational-Wave Observatory) collaboration, confirming Einstein's predictions and opening a new era in astrophysics.

## Importance of Gravitational Wave Detection

Detecting gravitational waves allows scientists to explore the universe in a new way, providing insights into cosmic events that are otherwise invisible through traditional telescopes. These detections help us understand fundamental physics, test Einstein’s theory of relativity, and study exotic astrophysical phenomena like black hole mergers and neutron star collisions.

## Gravitational Waves Visualization

To help visualize the concept of gravitational waves, see the animation below:

https://github.com/user-attachments/assets/dd324a38-82b2-4166-a319-262f33444a49


https://github.com/user-attachments/assets/626cb909-480a-4744-bb22-2492d243cc8b

## Results

The final performance comparison of ML models with Swin and ViT feature extractors is documented in:

`5Fold final results for ML models and Swin features extractor.csv`

`5Fold final results for ML models and ViT features extractor.csv`

Repository Contents

`Gravitational_Waves.ipynb`: Jupyter notebook containing the full workflow for data loading, preprocessing, feature extraction, and model training.

CSV Files: Store cross-validation results for different feature extraction methods.

## Contributors

[Youssef Husseiny Maaod](https://github.com/yuseiff)

[Ahmed Ashraf Abou-El-Ela](https://github.com/Ashraf1625)

[Osama Fawzy Adel](https://github.com/OsamaElswesy)

## License

This project is licensed under the [Creative Commons Attribution 4.0 International License](https://creativecommons.org/licenses/by/4.0/).

