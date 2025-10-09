# Problem Statement

Skin cancer is one of the most common cancers worldwide, and early detection is critical for effective treatment and improved patient outcomes. Manual diagnosis of skin lesions through visual inspection and dermoscopy can be time-consuming and prone to errors, especially in regions with limited access to dermatologists.  

This project aims to develop a **deep learning-based system** capable of automatically detecting and classifying skin lesions into nine categories using dermoscopic images:

1. Actinic Keratosis (130 images)  
2. Basal Cell Carcinoma (392 images)  
3. Dermatofibroma (111 images)  
4. Melanoma (454 images)  
5. Nevus (373 images)  
6. Pigmented Benign Keratosis (478 images)  
7. Seborrheic Keratosis (80 images)  
8. Squamous Cell Carcinoma (197 images)  
9. Vascular Lesion (142 images)  

By leveraging convolutional neural networks (CNNs), this system can assist dermatologists in early and accurate diagnosis, reducing misdiagnosis and improving patient care.

# Objectives

- Build a robust deep learning model to classify skin lesions into nine classes.  
- Analyze dermoscopic images to automatically extract meaningful features.  
- Address class imbalance and improve performance on underrepresented lesion types.  
- Evaluate model performance using metrics like accuracy, precision, recall, F1-score, and AUC.  
- Deploy a REST API using FastAPI for real-time prediction of skin lesions.  

# Challenges

- **Class Imbalance:** Some lesion types have very few samples (e.g., seborrheic keratosis: 80 images), making model training challenging.  
- **High Visual Similarity:** Certain lesions, such as melanoma and nevus, are visually similar.  
- **Data Quality:** Images vary in lighting, resolution, and orientation.  
- **Overfitting:** Small datasets may lead deep learning models to overfit without careful regularization.  
- **Interpretability:** Deep learning models are often black boxes, which can be a barrier for clinical adoption.  
- **Deployment:** Ensuring low-latency predictions in a production API using FastAPI.