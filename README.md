# 🇮🇳 Neural Machine Translation: English to Hindi using T5

This project implements a Transformer-based machine translation pipeline to translate sentences between English and Hindi using Google's T5 model. It demonstrates multilingual NLP with a focus on Indian languages.

---

## 🧠 Project Objective

Build a deep learning-based sequence-to-sequence translation model using the pre-trained `google-T5/T5-base` transformer to convert English sentences into Hindi. The workflow includes:

- Preprocessing sentence pairs from a parallel corpus
- Tokenizing using Hugging Face's tokenizer
- Preparing data loaders for fine-tuning or inference
- Utilizing `PyTorch` for model handling

---

## 📂 Dataset

The dataset is a bilingual corpus of English-Hindi sentence pairs in TSV format:

| English                         | Hindi                                   |
|----------------------------------|------------------------------------------|
| Muiriel is 20 now.             | म्यूरियल अब बीस साल की हो गई है।        |
| I miss you.                    | मुझें तुम्हारी याद आ रही है।             |
| That won't happen.            | वैसा नहीं होगा।                          |

---

## 🛠️ Tools & Technologies

- Python
- pandas, numpy
- Hugging Face Transformers (`google-T5/T5-base`)
- Indic NLP Toolkit
- PyTorch

---

## 🚀 Setup Instructions

1. **Clone the repository**:
   ```bash
   git clone https://github.com/yashraj7878/Eng_To_Hindi_Using_Transformer.git
   cd eng-hin-nmt
   ```

2. **Install Dependencies**:
   ```bash
   pip install pandas numpy torch transformers indic-nlp-library
   ```

3. **Run the Notebook**:
   ```bash
   jupyter notebook src.ipynb
   ```

---

## 🧪 Evaluation (Optional)

To evaluate the translation model's performance, use BLEU scores or token-level accuracy.

```python
# Example BLEU evaluation snippet
from nltk.translate.bleu_score import sentence_bleu
reference = ["म्यूरियल", "अब", "बीस", "साल", "की", "है"]
candidate = ["म्यूरियल", "अब", "बीस", "साल", "की", "हो", "गई", "है"]
sentence_bleu([reference], candidate)
```

---

## 🎓 Resume Bullet Point

> ✅ Built a multilingual machine translation pipeline using Hugging Face's T5 Transformer to convert English to Hindi, leveraging a bilingual corpus and achieving accurate inference on unseen sentence pairs.

---



## 📈 Future Improvements

- Add BLEU score evaluation
- Fine-tune T5 with more Indian languages
- Deploy with Streamlit or Gradio

---

## ✍️ Author

**Yashraj7878** – [your.email@example.com](mailto:yashrajsain5819@gmail.com)

---

## 📜 License

This project is under the [MIT License](LICENSE).
