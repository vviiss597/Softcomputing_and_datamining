# Softcomputing_a_datamining-2026

## 1. **Python Plotting**

---
## 2. **KNN ( K-Nearest Neighbors ):**
- Standard Scaler  → to ensure all features stand the same weight   
 &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;→ calculate "Euclidean Distance"  
  &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;→ find the closest **K** data  
- **Feature:**
  * boundary irregularly serrated
  * If K is too small ---> easily influenced by noise **(overfitting)**
  * If K is too large --> boundary is too blurry **(underfitting)**
  * K usually choose **odd numbers** to avoid even

---
## 3. **NB ( Naive Bayes ):**
- Assume : data are independent to each other
- Bayes’ theorem :

$$
\text{Posterior} = \frac{\text{Likelihood} \times \text{Prior}}{\text{Evidence}}
$$

$$
P(C=c \mid \mathbf{x}) = \frac{P(\mathbf{x} \mid C=c) \cdot P(C=c)}{P(\mathbf{x})}
$$

- Explain :  
  - Prior probability : overall probability of class C __ P(C)
  - Evidence : overall probability of feature x __P(x)
  - Posterior : given feature x, the probability of class C __ P(C|x)  
 &emsp; &emsp; &emsp; **→ the Ans. we want**
  - Likelihood : in class C the probability of feature x __ P(x|C)

$$
P(x_j \mid C=c) = \frac{1}{\sqrt{2 \pi \sigma_{c,j}^2}} \exp \left( -\frac{(x_j - \mu_{c,j})^2}{2 \sigma_{c,j}^2} \right)
$$

* In Gaussian Distribution (常態/鐘形分布): 
  * Mean (μ): average && the highest point in distribution  
&emsp;&emsp;&emsp; the more data closer to mean → likelihood get higher
  * Variance (σ²): the dispersion of dataset (變異數 → 離散程度)

---
## 4. **SVM ( Support Vector Machine):**
    - 


*To Be continued......*

