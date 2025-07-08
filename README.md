

````markdown
# 🤖 LLM Model Comparison using Ensemble Scoring

This project evaluates and compares various **Large Language Models (LLMs)** based on their performance metrics such as **accuracy**, **inference speed**, and **latency**. A composite score is generated using **ensemble-based normalization and weighted scoring**. The notebook is designed to be run directly in **Google Colab**.

---

## 📌 Features

- 📈 Visual comparison of LLMs based on multiple metrics
- 📊 Composite scoring using normalization and weighted aggregation
- 📤 Upload-and-analyze format (no local setup required)
- 🧮 Customizable weights for Accuracy, Speed, and Latency
- ✅ Clean visual outputs (bar plots, composite score rankings)

---

## 📂 Input Format

Upload a CSV file in the following structure:

| Model      | Accuracy | Speed (tokens/sec) | Latency (sec) |
|------------|----------|--------------------|----------------|
| GPT-4      | 0.91     | 310                | 3.12           |
| Gemini     | 0.89     | 295                | 3.17           |
| Claude     | 0.87     | 250                | 2.90           |

> 🔧 You can extend this dataset with additional columns such as `Cost` or `Memory` if needed.

---

## ⚙️ How It Works

1. **Upload your dataset** when prompted in the Colab notebook:
   ```python
   from google.colab import files
   files.upload()
````

2. **Run all cells** to:

   * Normalize metrics
   * Calculate a weighted composite score
   * Visualize top-performing LLMs

3. **Customize Weights**:
   You can edit the weights to match your priorities:

   ```python
   w_accuracy = 0.5
   w_speed = 0.3
   w_latency = 0.2
   ```

---

## 📊 Output Previews

### 🔹 Accuracy Comparison

<img src="assets/model_accuracy.png" width="600"/>

### 🔹 Composite Score Ranking

<img src="assets/composite_score_output.png" width="600"/>

---

## 📁 File Structure

```
ML_Project/
├── ML_Project.ipynb         # Main notebook
├── assets/
│   ├── model_accuracy.png   # Accuracy bar plot
│   └── composite_score_output.png  # Composite score graph
└── README.md                # You're here!
```

---

## 🛠️ Built With

* 🐍 Python 3
* 📊 Pandas, Matplotlib
* 📈 Scikit-learn
* ☁️ Google Colab (zero local setup)

---

## 📌 Use Cases

* Model selection for enterprise LLM applications
* Benchmarking custom-trained models
* Research comparisons across API-based LLMs

---

## 📬 Contact

Developed by **Vaishnavi Bhosale**
📧 [bhosalevaishnavi2019@gmail.com](mailto:bhosalevaishnavi2019@gmail.com)

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).

---

## 🌟 Star This Repo

If you found this useful, consider giving it a ⭐ on GitHub!

```

Let me know if you’d like help:
- Converting the notebook into a `.py` script.
- Creating a sample CSV dataset.
- Deploying it on GitHub with the correct structure.
```
