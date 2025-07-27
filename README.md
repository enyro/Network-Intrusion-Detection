# 🛡️ Network Intrusion Detection System (REST API)

A Flask-based REST API that predicts whether incoming network connections are **malicious (intrusions)** or **normal**, using a pre-trained machine learning model. Built for use in security systems and intrusion detection pipelines.

---

## 🚀 Features

- 🔍 **Single Request Prediction**: Send JSON data of a single network connection to get a real-time prediction.
- 📁 **Bulk Prediction via CSV Upload**: Upload a CSV file of multiple connections to get intrusion predictions in batch.
- 🤖 **Deep Learning Backend**: Powered by a Keras-based neural network trained on the NSL-KDD / KDD Cup 1999 dataset.
- 🧠 **Encodes categorical features**: Protocols, flags, and services are automatically encoded for model compatibility.
- 🔐 **Returns "Good" or "Bad"**: Each connection is classified as either safe or suspicious.

---

## 📦 Tech Stack

- Python 3
- Flask
- Keras + TensorFlow
- Pandas, NumPy
- REST API
- CORS enabled

---

## 📥 Installation

```bash
# Clone the repo
git clone https://github.com/enyro/Network-Intrusion-Detection.git
cd network-intrusion-detector

# Set up a virtual environment (optional)
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Run the server
python app.py
