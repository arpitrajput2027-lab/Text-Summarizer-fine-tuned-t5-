# Text Summarizer

A simple Text Summarization web application built using FastAPI and a fine-tuned T5 Transformer model.

---

## Folder Structure

```text
text-summarizer/
├── app.py
├── templates/
│   └── index.html
├── saved_summary_model/
├── requirements.txt
└── README.md
```

---

## WorkFlow

# Model Traing

### Step 1: Prepare Dataset

Collect and preprocess dialogue-summary pairs for training.

```text
Dialogue
    ↓
Summary
```

---

### Step 2: Fine-Tune T5

Train a pre-trained T5 model on the custom summarization dataset.

```text
Pretrained T5
      ↓
Custom Dataset
      ↓
Fine-Tuning
      ↓
Text Summarization Model
```

---

### Step 3: Save Trained Model

After training, save the model and tokenizer.

```python
trainer.save_model("./saved_summary_model")
tokenizer.save_pretrained("./saved_summary_model")
```


### Step 04 



#### 1. Install Dependencies

```bash
pip install -r requirements.txt
```

### 2. Run the Server

```bash
uvicorn app:app --reload
```

### 5. Open in Browser

```text
http://localhost:8000
```

---

## Tech Stack

* Backend — FastAPI
* Frontend — HTML, CSS, JavaScript
* AI Model — Fine-Tuned T5
* Framework — Hugging Face Transformers
* Deep Learning — PyTorch
# Text Summarizer

A Text Summarization web application built using FastAPI and a fine-tuned T5 Transformer model.

---


