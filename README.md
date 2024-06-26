# Mechanical Fatigue Prediction Project

![Project Banner](https://yasincapar.com/wp-content/uploads/2021/05/Pic-2-1140x646.png)
![Project Banner](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQyFX3ztTKjWSp2bwG480jCCT37_3iSxdoYdWaGbx8ybw&s)



## Table of Contents
- [Introduction](#introduction)
- [Project Overview](#project-overview)
- [Data](#data)
- [Methods](#methods)
  - [Gradient Boosting Machines (GBM)](#gradient-boosting-machines-gbm)
  - [AdaBoost](#adaboost)
  - [CatBoost](#catboost)
- [Results](#results)
- [Conclusion](#conclusion)
- [Project Impact](#project-impact)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

## Introduction
Welcome to our Mechanical Fatigue Prediction Project, where we explore machine learning models for predicting mechanical fatigue in various materials, contributing to safety and reliability in engineering applications.

## Project Overview
Mechanical fatigue prediction is a critical aspect of engineering, ensuring the safety and reliability of components and systems. In this project, we focus on predicting fatigue life for three important materials: Ti-6Al-4V, IN718 (Inconel 718), and AlSi10Mg.

## Specific Materials Details

### Titanium Alloy (Ti-6Al-4V)

Ti-6Al-4V is a widely used titanium alloy known for its excellent corrosion resistance and high strength-to-weight ratio. It finds applications in aerospace, biomedical implants, and automotive industries. The alloy's fatigue behavior is crucial in structural design and durability assessment.

### Inconel 718 (IN718)

IN718 is a nickel-based superalloy known for its high temperature and corrosion resistance properties. It is extensively used in aerospace, gas turbines, and automotive applications. Understanding its fatigue behavior is vital for ensuring component reliability under extreme conditions.

### Aluminum Alloy (AlSi10Mg)

AlSi10Mg is an aluminum-silicon-magnesium alloy commonly used in additive manufacturing (3D printing). Its lightweight properties and good mechanical strength make it suitable for aerospace and automotive applications. Predicting its fatigue life aids in optimizing component design and performance.


## Data
The project utilizes a curated dataset encompassing critical features relevant to mechanical fatigue behavior. The data preprocessing phase handled outliers, missing values, and feature scaling to prepare the dataset for machine learning models.

## Methods
### Gradient Boosting Machines (GBM)
GBM techniques, such as XgBoost and LightGBM, excel in capturing intricate patterns in fatigue data. Their ensemble-based learning enhances predictive accuracy.

### AdaBoost
AdaBoost, known for its adaptive boosting, provides improved predictive performance by sequentially training weak models to focus on previously misclassified samples.

### CatBoost
CatBoost, designed to handle categorical data efficiently, is well-suited for datasets with mixed feature types. Its robustness and accuracy make it a valuable choice for fatigue life prediction.

## Results
### R-squared Scores
| Material     | GBM R-squared | AdaBoost R-squared | CatBoost R-squared |
|--------------|---------------|--------------------|--------------------|
| Ti-6Al-4V    | 0.6136        | 0.5618             | 0.7288             |
| IN718        | 0.1733        | 0.4061             | 0.1064             |
| AlSi10Mg     | 0.9513        | -1.9033            | 0.2754             |

### RMSE Scores
| Material     | GBM RMSE      | AdaBoost RMSE      | CatBoost RMSE      |
|--------------|---------------|--------------------|--------------------|
| Ti-6Al-4V    | 3.92e-07      | 4.17e-07           | 3.28e-07           |
| IN718        | 2.36e-07      | 3.56e-07           | 1.88e-07           |
| AlSi10Mg     | 1.42e-06      | 2.54e-06           | 1.27e-06           |

## Conclusion
Our analysis indicates varying performance across different materials and models. While CatBoost generally performed well across materials, GBM showed exceptional accuracy for AlSi10Mg despite challenges in fatigue prediction for this material. Further research and model refinement are recommended to enhance predictive capabilities for all materials, contributing to safer and more reliable engineering practices.

## Project Impact
Accurate fatigue life prediction is instrumental in ensuring the reliability and safety of mechanical components and systems. By improving predictive models, we contribute to reducing failures, maintenance costs, and downtimes in various industries, ranging from aerospace to manufacturing.

## Usage
To replicate our results or further explore the models:
1. Clone this repository.
2. Install the required dependencies specified in `requirements.txt`.
3. Run the provided scripts or notebooks to train and evaluate the models.

## Contributing
Contributions to enhance model performance, expand the dataset, or refine preprocessing techniques are welcome. Please follow the established guidelines for contributions.

## License
This project is licensed under the [MIT License](LICENSE).


