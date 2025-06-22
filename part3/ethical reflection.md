# 🧠 Ethical Reflection: Bias & Fairness in Predictive Analytics  
**(Related to Part 2 - Task 3)**

## Prompt  
*Your predictive model from Task 3 is deployed in a company. Discuss potential biases in the dataset (e.g., underrepresented teams). How fairness tools like IBM AI Fairness 360 could address these biases?*

---

## 🔍 Potential Biases in the Dataset

Although the breast cancer dataset is originally medical, it was adapted in Task 3 to simulate software issue priority. In a real software engineering context, several ethical risks may arise:

### 1. **Label Simulation Bias**  
- Mapping diagnosis (Malignant/Benign) to issue priority (High/Low) is artificial.
- This may introduce unfair interpretations and lead to faulty predictions in production systems.

### 2. **Underrepresented Classes**  
- If high-priority cases are rare, the model may overfit on low-priority examples.
- Real-world logs might underrepresent certain teams, creating skewed learning patterns.

### 3. **Feature Selection Bias**  
- In actual projects, features like reporter names or team IDs might correlate with biased patterns.
- This could cause the model to prioritize or ignore certain groups unfairly.

### 4. **Historical Bias**  
- Past human decisions may reflect biased judgments (e.g., always resolving backend issues faster).
- These biases can be absorbed and amplified by the model over time.

---

## 🛠️ How IBM AI Fairness 360 Can Help

The **AI Fairness 360 (AIF360)** toolkit by IBM offers multiple strategies to promote fairness:

### ✅ 1. **Bias Detection**  
- Offers metrics like Disparate Impact and Equal Opportunity to check if the model treats subgroups differently.
- Can identify whether a department’s issues are consistently under-prioritized.

### ✅ 2. **Preprocessing Techniques**  
- Adjusts dataset distribution (e.g., reweighing classes, oversampling).
- Ensures balanced learning before model training.

### ✅ 3. **In-processing Methods**  
- Applies fairness constraints during model training.
- Prevents learning from imbalanced features or biased outcomes.

### ✅ 4. **Post-processing Audits**  
- Analyzes predictions and makes fairness corrections if disparities are found.
- Helps build trust in model decisions when deployed.

---

## ✅ Takeaway

In software engineering, it's not enough for predictive models to be accurate — they must also be fair. By applying tools like IBM’s AIF360 and reviewing training data critically, we can develop AI systems that are responsible, transparent, and inclusive.
