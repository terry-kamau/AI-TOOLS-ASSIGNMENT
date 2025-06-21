# 🧠 Ethical Reflection: Bias in AI Models

## 1. MNIST Handwritten Digit Classifier

The MNIST dataset is widely used but can have hidden biases:
- It mostly contains neat, center-aligned digits written by American students.
- Real-world digits (e.g., from children, elders, different countries) may be written very differently.
- If deployed globally, such a model might misclassify digits from underrepresented groups.

**Mitigation:**
- Use additional, more diverse datasets like EMNIST or real handwriting samples.
- Use TensorFlow Fairness Indicators to evaluate subgroup accuracy and address gaps.

---

## 2. Amazon Product Reviews – NLP Model

Sentiment analysis using simple rules (e.g., “good” = positive) is prone to:
- Missing context or sarcasm
- Cultural variations in tone or emotion
- Biased sentiment labeling (e.g., gendered product reviews)

**Mitigation:**
- Replace rules with trained models (e.g., TextBlob or VADER) that handle nuance.
- Sample reviews from different demographic groups and evaluate fairness in sentiment scoring.

---

## Conclusion

To ensure AI is ethical and inclusive, we must continually test models against real-world diversity, use fairness tools, and involve human oversight when automating sensitive decisions.
