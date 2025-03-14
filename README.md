# sms_spam_detector

This project is an **SMS Spam Detector** built using **Gradio** for the user interface and a machine learning model to classify SMS messages as **Spam or Not Spam**.

## 🚀 **Getting Started**

### **Installation**

Ensure you have Python installed, then install the required dependencies:

# Import pandas
import pandas as pd
# Import the required dependencies from sklearn
from sklearn.model_selection import train_test_split
from sklearn.pipeline import Pipeline
from sklearn.feature_extraction.text import TfidfVectorizer
from sklearn.svm import LinearSVC

# Set the column width to view the text message data.
pd.set_option('max_colwidth', 200)

# Import Gradio
import gradio as gr

### **Running the Application**

To start the Gradio app, run:

```bash
python gradio_sms_text_classification.py
```

If you're using a Jupyter Notebook, execute all the cells.

Once running, the app will open in your browser. Enter an SMS message, and the model will classify it as **Spam or Not Spam**.

## 🔠 **Troubleshooting**

### **1. Gradio Template Not Found (`jinja2.exceptions.TemplateNotFound`)**
- Ensure Gradio is installed via `pip` and not from source.
- Try reinstalling Gradio:
  ```bash
  pip uninstall gradio -y
  pip install --no-cache-dir gradio
  ```

### **2. Prediction Returns `None`**
- Check if the model is loading correctly.
- Add debugging print statements inside the classification function.

### **3. DataFrame is Empty**
- Ensure that valid input is passed to the classifier before making predictions.

---

## 🐍 **License**
This project is for educational purposes. Feel free to modify and improve it.