# Softcomputing_a_datamining-2026

## 1. **Python Plotting**

---
## 2. **KNN ( K-Nearest Neighbors ) :**
- Standard Scaler  → to ensure all features stand the same weight   
 &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;→ calculate "Euclidean Distance"  
  &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;→ find the closest **K** data  
- **Feature:**
  * boundary irregularly serrated
  * If K is too small ---> easily influenced by noise **(overfitting)**
  * If K is too large --> boundary is too blurry **(underfitting)**
  * K usually choose **odd numbers** to avoid even

---
## 3. **NB ( Naive Bayes ) :**
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

* In Gaussian Distribution (常態/鐘形分布) : 
  * Mean (μ): average && the highest point in distribution  
&emsp;&emsp;&emsp; the more data closer to mean → likelihood get higher
  * Variance (σ²): the dispersion of dataset (變異數 → 離散程度)

---
## 4. **SVM ( Support Vector Machine ) :**  
- **Goal :** to find the **maximum Margin**  
- Hyperplane : a plane best separates classes  
- Margin : the distance between Hyperplane and data points closest to the hyperplane from each class (Support Vectors)  
&emsp;&emsp;&emsp;&emsp; use **Soft Margin** → to avoid influence from noise
- Support Vectors : data points lie on or within margin boundaries  
&emsp;&emsp;&emsp; &emsp; → directly influence the position of the hyperplane

- Explanation :
  * **Hard Margin SVM:** For perfectly linearly separable data; no misclassifications allowed.
  * **Soft Margin SVM:** For non-linearly separable data or when tolerating some misclassifications/margin violations; uses slack variables ($\xi_i$) and a regularization parameter ($C$)
 
* **Dual Problem:** The optimization formulation that is typically solved, leading to the use of kernel functions
  
* **Kernel Trick:** Allows SVM to learn non-linear decision boundaries  
&emsp;&emsp;&emsp; → mapping data to higher-dimensional where might linearly separable  
&emsp;&emsp;&emsp; → without computing the high-dimensional coordinates  
&emsp;&emsp;&emsp; → simply using dot product :  
  
$$
K(x_i, x_j) = \phi(x_i) \cdot \phi(x_j)
$$


* **KKT Conditions:** Explain the relationship between the Lagrange multipliers ($\alpha_i$) and the data points (support vectors vs. non-support vectors).


---
*To Be continued......*


