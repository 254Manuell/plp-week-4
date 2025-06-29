# Task 1: AI-Powered Code Completion

## 🛠️ Tool Used
- **Code Completion Tool:** GitHub Copilot (or Tabnine)

## 📝 Task Overview
This project demonstrates how to sort a list of dictionaries in Python by a specific key. It includes:
- A manual implementation of the sorting function.
- An example of AI-suggested code (from Copilot/Tabnine).
- A comparison of both approaches in terms of efficiency.

## 📄 Code Summary

The main function:
```python
def sort_list_of_dictionaries(data_list, sort_key, reverse=False):
    """
    Sort a list of dictionaries by a specific key.
    """
    return sorted(data_list, key=lambda item: item[sort_key], reverse=reverse)
```

### Usage Examples
- **Sort by age (ascending)**
- **Sort by name (descending)**
- **Sort by grade, then by age**

### Example Output
The script prints the sorted student dictionaries for each case.

## 🤖 AI vs Manual Implementation

Both the manual and AI-suggested implementations use Python’s built-in `sorted()` function with a lambda for the key. For multi-key sorting, a tuple is used in the lambda. The AI-suggested code is nearly identical to the manual version, showing that this is a standard Python approach.

## ⚡ Efficiency

- Both versions are equally efficient, leveraging Python’s optimized sorting.
- No significant performance difference exists, as both use the same algorithm and idioms.

## 🏆 Conclusion

- Both manual and AI-generated solutions are Pythonic and efficient.
- AI tools like Copilot or Tabnine can help you quickly write such utility functions, but understanding the logic is important for customization and debugging.

---

✨ **Happy Coding!** ✨

# Task 3: Predictive Analytics for Resource Allocation 🩺

## 📋 Goal

- **Preprocess data:** Clean images, encode labels, and split into training/testing sets.
- **Train a model:** Use a Random Forest classifier to predict breast cancer priority (high/low).
- **Evaluate:** Assess model performance using accuracy and F1-score.
- **Deliverable:** Jupyter Notebook with code, visualizations, and performance metrics.
- **Ethical Reflection:** Discuss dataset bias and fairness tools.

---

## 🛠️ Workflow Overview

1. **Import Dependencies:** Load Python libraries for data handling, image processing, and machine learning.
2. **Load Raw Image Data:** Read and label images from the dataset directory.
3. **Clean the Data:** Remove images that are too small or failed to load.
4. **Preprocess & Extract Features:** Resize images and flatten them into feature vectors.
5. **Encode Labels:** Map 'benign' and 'malignant' to 'low' and 'high' priority, then encode numerically.
6. **Split Dataset:** Divide data into training and test sets.
7. **Train the Model:** Fit a Random Forest classifier on the training data.
8. **Evaluate Performance:** Calculate accuracy, F1-score, and display a classification report.
9. **Visualize Predictions:** Show a grid of test images with true and predicted labels, highlighting correct and incorrect predictions.
10. **Model Parameters:** Display information about the trained Random Forest.

---

## 📊 Performance Metrics

- **Accuracy:** Measures the proportion of correct predictions.
- **F1 Score:** Weighted average of precision and recall, useful for imbalanced datasets.
- **Classification Report:** Detailed breakdown of model performance by class.

---

## 🧑‍⚖️ Ethical Reflection

### Potential Biases

- **Dataset Bias:** If certain categories (e.g., 'benign' or 'malignant') are underrepresented, the model may perform poorly on those cases.
- **Sampling Bias:** If images come from a limited demographic or imaging device, predictions may not generalize.
- **Labeling Bias:** Human error or subjective labeling can introduce inaccuracies.

### Addressing Bias with Fairness Tools

- **IBM AI Fairness 360:** This toolkit can help detect and mitigate bias in datasets and models. It provides metrics to assess fairness and algorithms to reduce disparate impact.
    - **Example:** Use fairness metrics to check if the model's accuracy is consistent across different subgroups (e.g., age, gender, imaging device).
    - **Mitigation:** Apply reweighting or adversarial debiasing to improve fairness.

---

## 📁 Deliverable

- **Jupyter Notebook:** Contains all code, visualizations, and performance metrics for reproducibility and review.

---

✨ **For best results, ensure your dataset is balanced and consider using fairness tools to audit and improve your model!**