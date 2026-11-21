## Day 1 – Foundations of CBIR  

| Time | Activity | Details |
|------|----------|---------|
| 9:00 – 9:30 | **Intro to CBIR** | What is Content‑Based Image Retrieval? Why it matters (search by visual content, not keywords). |
| 9:30 – 10:30 | **Image Representation Basics** | • Pixels, color spaces (RGB, HSV, Lab)  <br>• Why we need a compact representation. |
| 10:30 – 10:45 | **Break** | – |
| 10:45 – 12:00 | **Color Features** | • Color histograms (global & regional)  <br>• Normalisation, quantisation, similarity (e.g., histogram intersection). |
| 12:00 – 13:00 | **Lunch** | – |
| 13:00 – 14:30 | **Texture Features** | • Co‑occurrence matrices, GLCM  <br>• Local Binary Patterns (LBP)  <br>• Simple texture descriptors (contrast, homogeneity). |
| 14:30 – 14:45 | **Break** | – |
| 14:45 – 16:00 | **Shape Features** | • Edge detection, contour descriptors  <br>• Fourier descriptors, moment invariants. |
| 16:00 – 16:30 | **Recap & Quick Quiz** | Write down three types of visual features and one advantage of each. |

---

## Day 2 – Matching, Indexing & Evaluation  

| Time | Activity | Details |
|------|----------|---------|
| 9:00 – 9:30 | **Review of Day 1** | Quick Q&A, clarify any doubts. |
| 9:30 – 10:30 | **Similarity Measures** | • Euclidean, Manhattan, Chi‑square distances  <br>• Cosine similarity for high‑dimensional vectors. |
| 10:30 – 10:45 | **Break** | – |
| 10:45 – 12:00 | **Feature Extraction Pipelines** | Hands‑on coding: extract colour histogram & texture (LBP) from a sample image set (Python + OpenCV). |
| 12:00 – 13:00 | **Lunch** | – |
| 13:00 – 14:30 | **Indexing Structures** | • Linear scan vs. inverted file vs. KD‑tree vs. LSH (Locality Sensitive Hashing). |
| 14:30 – 14:45 | **Break** | – |
| 14:45 – 15:45 | **Evaluation Metrics** | • Precision, Recall, MAP (Mean Average Precision)  <br>• PR curves, ROC. |
| 15:45 – 16:30 | **Mini‑Project Planning** | Choose a small dataset (e.g., 100 images) and decide which features & index you will use. Write a one‑page plan. |

---

## Day 3 – Advanced Topics & Putting It All Together  

| Time | Activity | Details |
|------|----------|---------|
| 9:00 – 9:30 | **Deep Learning Features** | Overview of CNN embeddings (e.g., VGG, ResNet) as image descriptors. |
| 9:30 – 10:30 | **Relevance Feedback** | How user feedback can refine results (Rocchio algorithm, query expansion). |
| 10:30 – 10:45 | **Break** | – |
| 10:45 – 12:00 | **Building a Simple CBIR System** | Step‑by‑step: <br>1. Feature extraction (choose colour + deep features). <br>2. Store vectors in an index (FAISS or Annoy). <br>3. Query processing and display top‑k results. |
| 12:00 – 13:00 | **Lunch** | – |
| 13:00 – 14:30 | **Performance Optimisation** | • Dimensionality reduction (PCA, t‑SNE for visualisation). <br>• Approximate nearest neighbour trade‑offs. |
| 14:30 – 14:45 | **Break** | – |
| 14:45 – 15:45 | **Ethical & Practical Considerations** | Copyright, bias in visual datasets, user privacy. |
| 15:45 – 16:30 | **Final Review & Quiz** | Go over key concepts, answer any remaining questions. |

---

# Quick Quiz – Content‑Based Image Retrieval  

| # | Question | Answer |
|---|----------|--------|
| 1 | **What is the main purpose of a colour histogram in CBIR?** | To capture the distribution of colours in an image, providing a compact descriptor that can be compared across images. |
| 2 | **Name two distance metrics commonly used to compare feature vectors.** | Euclidean distance and Chi‑square distance (others include Manhattan and cosine similarity). |
| 3 | **What advantage does Locality Sensitive Hashing (LSH) give over a linear scan?** | LSH speeds up nearest‑neighbour search by hashing similar vectors into the same buckets, reducing the number of comparisons needed. |
| 4 | **Briefly describe what “relevance feedback” means in a CBIR system.** | The system asks the user to mark retrieved images as relevant or not, then adjusts the query (or feature weights) to improve future results. |
| 5 | **Why might you use a pre‑trained CNN (e.g., ResNet) as a feature extractor instead of hand‑crafted features?** | CNN embeddings capture high‑level semantic information automatically, often leading to better retrieval performance than low‑level hand‑crafted descriptors. |

Feel free to revisit any day’s material if a question feels tricky—understanding the “why” behind each concept makes the whole system click!