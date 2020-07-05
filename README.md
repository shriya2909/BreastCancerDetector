# BreastCancerDetector

## **Problem Statement**
I have been tasked with developing a means to help doctors diagnose breast cancer. Data given is about biopsied breast cells; where it is benign (not harmful) or malignant (cancerous).
1. What features of a cell are the largest drivers of malignancy?
2. How would a physician this product?
3. There is a non-zero cost in time and money to collect each feature about a given cell. How would I go about determining the most cost-effective method of
detecting malignancy?

## **Data Features** 
Sample code number: id number 
<br>Clump Thickness: 1 - 10 
<br>Uniformity of Cell Size: 1 - 10 
<br>Uniformity of Cell Shape: 1 - 10 
<br>Marginal Adhesion: 1 - 10 
<br>Single Epithelial Cell Size: 1 - 10 
<br>Bare Nuclei: 1 - 10 
<br>Bland Chromatin: 1 - 10 
<br>Normal Nucleoli: 1 - 10 
<br>Mitoses: 1 - 10 
<br>Class: (2 for benign, 4 for malignant)


## **Quick Answers**

1. *What features of a cell are the largest drivers of malignancy?*
*   Uniformity of Cell Size
*   Uniformity of Cell Shape
*   Normal Nucleoli
*   Clump Thickness
*   Marginal Adhesion

2. *How would a physician use this product?*
<br>Product can be used to predict malignancy with 0.95 Recall i.e. is the ability of a test to correctly identify malignant results to get the true positive rate.

3. *There is a non-zero cost in time and money to collect each feature about a given cell. How would I go about determining the most cost-effective method of detecting malignancy?*
<br>  The product utilises 3 features - Uniformity of Cell Shape, Clump Thickness Mitoses. 
  However, there is a trade off between number of features in the model and the recall of the Malignant class. In order to further increase the recall from 0.95, we can add additional features based on the order of their importance.
Recall is utilised here as the metric for evaluation as we aim to maximize finding all patients who have cancerous cells and minimize any relevent patient go undiagnosed.

Follow the below link to colab notebook:
https://colab.research.google.com/drive/1cNSCxQtUeOKfykzXW0LfceIJJfXlSsyJ?usp=sharing
