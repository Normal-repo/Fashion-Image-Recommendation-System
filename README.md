# 🧥 Fashion Image Recommendation System  
### Deep Learning + FAISS Similarity Search

This project implements a **content-based fashion image recommendation system**.  
It extracts image embeddings using **ResNet50** and performs fast similarity search using **FAISS**.

---

## 🚀 Features

- 🔍 Image-based similarity search  
- 🧠 2048-dim embeddings from **ResNet50**  
- ⚡ Fast KNN search using **FAISS**  
- 💾 Precomputed embeddings stored in `embeddings_store.npz`  
- 📘 Jupyter Notebook included for the full pipeline  
- 🔧 Easy to extend for large datasets  

---

## 📂 Repository Structure

- fashion-recommendation.ipynb # Main notebook (feature extraction + FAISS search)
- embeddings_store.npz # Precomputed embeddings (Git LFS)
- README.md # Project documentation


---

## 🛠️ Installation

Install required packages:

```bash
pip install tensorflow faiss-cpu numpy pillow matplotlib
```

## ▶️ Usage

### **1. Open the notebook**
```bash
jupyter notebook fashion-recommendation.ipynb
```

## Inside the notebook you can:
 - Load your dataset
 - Extract image embeddings
 - Save them to .npz
 - Build a FAISS index
-  Query similar images
 - Visualize top-K results

## 🧠 How It Works
 1️⃣ Embedding Extraction

Images → ResNet50 → 2048-dimensional feature vector

## 2️⃣ Indexing

All embeddings are stored in a FAISS index for fast vector search.

## 3️⃣ Similarity Search

Given a query image →
FAISS retrieves the nearest neighbors based on embedding similarity.

## 📌 Future Improvements

Streamlit web app

CLIP embeddings (text + image)

Category filtering

Custom CNN trained specifically for fashion data

## ⭐ Support

If you found this project helpful, consider giving it a ⭐ on GitHub!

