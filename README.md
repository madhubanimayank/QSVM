# 🌌 **Quantum SVM for Stock Fraud Detection** 
---

In this project, we will learn how to implement Quantum-enhanced Support Vector Machines (QSVM) for stock fraud detection. We will use it to classify the manipulated stocks from genuine ones. The QSVM algorithm is mostly similar to the classical SVM. The  only difference between the two is that QSVM integrates quantum mechanics to replace the kernel method which is used in its classical counterpart. The kernal functions are used to compute the dot product of two feature vectors to find the similarity between them in a higher feature space. The kernel method is replaced here by a quantum feature map and a measure of similarity through various state measurement strategies. This quantum approach promises a potential speedup, especially when dealing with datasets rich in features.

To get a quick overview of classical support vector classifiers, one can read this [blog](https://medium.com/analytics-vidhya/introduction-to-svm-and-kernel-trick-part-1-theory-d990e2872ace). Now, for QSVM, here is a nice [introdution](github.com/PatrickHuembeli/QSVM-Introduction)          .

In this project, we will follow a simplified version of the approach described in the paper: [Mixed Quantum–Classical Method for Fraud Detection With Quantum Feature Selection](https://doi.org/10.1109/TQE.2022.3213474). Feature selection is based on the same paper with some modifications and draws the approach from the detailed code for quantum feature selection, as described in the paper, by Christophe Pere which can be viewed on his github repository [here](https://github.com/Christophe-pere/Quantum-Feature-Importance-Selection).

---



---
## 📊 **Dataset Details and objective:**

The dataset we're using is hosted on Kaggle and can be downloaded from this [link](https://www.kaggle.com/datasets/neeoon/flcs-stock-market-transaction-2021-2022?select=flc_2013_2022_notime.csv). It comprises historical data on stock prices and transaction volumes. The dataset consists of 2,170 rows and 7 columns. The columns are named '**open**', '**high**', '**low**', '**close**', '**Volume**', '**Volume MA**', and '**manipulated**'. All columns contain numerical values. The last column, which is our target, has two classes: '**1**' and '**0**'. These represent whether the stock is manipulated or not, respectively. Using the first six columns as features, our algorithm aims to predict the manipulation status of the stock. Our goal is to achieve a recall of 0.9 for class 1, meaning we should accurately detect more than 90 out of every 100 manipulated stocks.




---
## **Libraries**
![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white) ![Qiskit](https://img.shields.io/badge/Qiskit-%236929C4.svg?style=for-the-badge&logo=Qiskit&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-%23ffffff.svg?style=for-the-badge&logo=Matplotlib&logoColor=black)
![scikit-learn](https://img.shields.io/badge/scikit--learn-%23F7931E.svg?style=for-the-badge&logo=scikit-learn&logoColor=white) ![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)

`pandas==1.3.5`

`seaborn==0.12.2`

`imbalanced-learn==0.11`

`scikit-learn==1.1.3`

`matplotlib==3.5.2`

`pylatexenc==2.10`

`qiskit==0.43.3`

`qiskit-aer==0.12.2`

`qiskit-ibm-runtime==0.9.4`

`qiskit-ibmq-provider==0.20.2`

`qiskit-machine-learning==0.6.1`


---

---
## 📚 **Reference**:
- **Title**: [Mixed Quantum–Classical Method for Fraud Detection With Quantum Feature Selection](https://doi.org/10.1109/TQE.2022.3213474)

    M. Grossi *et al.*, "**Mixed Quantum–Classical Method for Fraud Detection With Quantum Feature Selection**," in IEEE Transactions on Quantum Engineering, vol. 3, pp. 1-12, 2022, Art no. 3102812, doi: 10.1109/TQE.2022.3213474.
---
