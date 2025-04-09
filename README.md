# 🌿 POClassifier

**POClassifier** is a Transformer-based text classification framework tailored for multi-type classification tasks based on the [Plant Ontology (PO)](http://www.plantontology.org/). It supports type-specific label masking and offers intuitive training, evaluation, and visualization features using the Hugging Face ecosystem.

---

## 🚀 Features

- 🌱 Supports multiple PO types with individual label spaces
- 🧠 Built on top of Hugging Face Transformers and Datasets
- 📊 Easy evaluation with type-wise metrics and visualizations
- 📈 Customizable training (early stopping, optimizer config, freezing layers)
- 🔍 Supports prediction with confidence per PO type
- 📉 Plots training history with loss and performance metrics

---

## 🛠 Installation

```bash
git clone https://github.com/your-username/po-classifier.git
cd po-classifier
pip install -r requirements.txt


## 📦 Dependencies
```bash
transformers>=4.30.0
datasets>=2.13.0
scikit-learn>=1.0.0
numpy
matplotlib
torch>=1.10.0

## 🧪 Quick Start
```bash
from po_classifier.model import POClassifier

# 1. Initialize with your dataset
model = POClassifier(texts, labels, types)

# 2. Load a pretrained Transformer model (e.g., BERT)
model.set_model("bert-base-uncased")

# 3. Tokenize and train
model.tokenize().train()

# 4. Evaluate or predict
metrics = model.evaluate()
results = model.predict("leaf and shoot apex")

# 5. Plot training history
model.plot_history()

