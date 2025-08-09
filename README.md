# Dense-U-Net_Urban_Builtup_Extraction
Dense U-Net model for high-resolution satellite image segmentation to extract urban built-up areas. Supports preprocessing, training, evaluation, and prediction for real-world urban mapping applications.
Urban Built-up Area Extraction using Dense U-Net
📌 Description
Dense U-Net model for high-resolution satellite image segmentation, focusing on automated extraction of urban built-up areas. The project includes preprocessing, training, evaluation, and prediction modules for real-world urban mapping applications.

🚀 Features
Dense U-Net architecture for improved feature retention and precise segmentation.

High-resolution satellite imagery support (256×256 to 512×512).

Binary classification masks for built-up vs. non-built-up areas.

Data augmentation (rotation, flipping, brightness, noise) for better generalization.

Evaluation metrics: Accuracy, IoU, Dice Coefficient, Precision, Recall, F1-Score.

Post-processing for refined building boundary detection.

📂 Dataset
Source: Open-access platforms (Kaggle, Google Earth Engine).

Composition: 30 high-resolution image–mask pairs for testing, with train/validation/test splits.

Format: PNG/TIFF with pixel sizes from 256×256 to 512×512.

Masks: Built-up (1) and non-built-up (0) classes.


# Install dependencies
pip install -r requirements.txt
📜 Usage
1️⃣ Preprocess Data
python
Copy
Edit
python preprocess.py
2️⃣ Train Model
python
Copy
Edit
python train.py
3️⃣ Evaluate Model
python
Copy
Edit
python evaluate.py
4️⃣ Predict Segmentation Mask
python
Copy
Edit
python predict.py --image_path sample_image.png
📊 Model Performance
Metric	Score (%)
Accuracy	90+
IoU	High
F1-Score	High
Precision	High
Recall	High

Dense U-Net showed robust generalization across urban, suburban, and semi-rural settings with minimal overfitting.

🏙 Real-world Applications
Urban Planning – Automated building footprint extraction.

Disaster Management – Damage assessment after floods, earthquakes, etc.

Infrastructure Monitoring – Detecting changes over time.

Smart City Development – Supporting geospatial decision-making.

📌 Project Architecture
text
Copy
Edit
├── data/               # Dataset directory
├── preprocess.py       # Data preprocessing
├── train.py            # Model training
├── evaluate.py         # Model evaluation
├── predict.py          # Generate segmentation masks
├── models/             # Dense U-Net implementation
├── requirements.txt    # Dependencies
└── README.md           # Documentation


