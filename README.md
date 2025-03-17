# 🌿 Plant Disease Classification using CNN (TensorFlow + DirectML)

This project is a simple yet effective Convolutional Neural Network (CNN) for classifying plant leaf images using the [PlantVillage dataset](https://www.kaggle.com/datasets/emmarex/plantdisease).

## 🚀 Features
- Uses Intel GPU via DirectML (for systems without CUDA support)
- Image preprocessing and augmentation
- Train-validation-test pipeline
- Supports multiple classes
- Clean and modular training script

## 📁 Dataset
Place the PlantVillage dataset inside a folder named `PlantVillage` in the project root. It should follow the `image_folder/class_name/image.jpg` format.

## ⚙️ Setup

```bash
pip install -r requirements.txt
```

## 🏃‍♂️ Run Training

```bash
python train.py
```

After training, the model will be saved as `plant_disease_model.h5`.

## 🧠 Model Architecture

- Multiple Conv2D layers with ReLU
- MaxPooling for downsampling
- Dense layer with Softmax for classification

## 🖼 Example Output

Supports real-time image classification and can be extended for mobile deployment or web apps.

## 📌 Note
DirectML is useful for Intel/AMD GPUs. If not available, training falls back to CPU automatically.

---

🔬 Built with ❤️ for Deep Learning + Plant Health
