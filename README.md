# 🧠 Image Classification of Sperm Abnormalities

This project builds an image classification model to detect abnormalities in sperm cells based on four categories: **Acrosome**, **Head**, **Tail**, and **Vacuole**. Each image has 4 binary labels (0 = Normal, 1 = Abnormal).

---

## 📦 Dataset

- **Source**: [MHSMA (Sperm Morphology Analysis Dataset) on Kaggle](https://www.kaggle.com/datasets/orvile/mhsma-sperm-morphology-analysis-dataset)
- **Image Sizes**: `128x128` and `64x64`
- **Image Files**:
  - `x_128_train.npy`, `x_128_valid.npy`, `x_128_test.npy`
  - `x_64_train.npy`, `x_64_valid.npy`, `x_64_test.npy`
- **Labels** (multi-label format: shape = `[n_samples, 4]`):
  - `y_acrosome_*.npy`
  - `y_head_*.npy`
  - `y_tail_*.npy`
  - `y_vacuole_*.npy`

Each image corresponds to a 4-label binary array like `[0, 1, 0, 0]`.

git clone https://github.com/your-username/image-classification-sperm.git
cd image-classification-sperm

pip install -r requirements.txt

python src/train_model.py

python src/predict_single.py --img_path real_images/sample.png

Acrosome: Normal (0.12)
Head: Abnormal (0.89)
Tail: Normal (0.02)
Vacuole: Normal (0.07)

🔧 Requirements
pip install -r requirements.txt

👤 Author
Youssef Elzahar
feel free to reach out on linkedin:https://www.linkedin.com/in/youssef-elzahar/
