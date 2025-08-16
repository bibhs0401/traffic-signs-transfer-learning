# 🚦 Stop Sign Classifier  

Classify images into **Stop** or **Not Stop** using **Transfer Learning** with pre-trained CNNs: InceptionV3, MobileNet, and ResNet50.  

---

## 📂 Project Structure
Datasets are organized into train and test folders with stop and not_stop subfolders.
signs/

  ┣ train/stop, train/not_stop

  ┣ test/stop, test/not_stop

## ⚙️ Setup
```bash
pip install tensorflow keras matplotlib numpy scikit-learn opendatasets
```

## 🛠 Training

1. Use ImageDataGenerator for augmentation.
2. Freeze pre-trained CNN layers and add:
3. Flatten → Dense(1024, relu) → Dropout(0.2) → Dense(1, sigmoid)
4. Compile with RMSprop and binary_crossentropy.
5. Fit model with EarlyStopping.

## Models Used
1. InceptionV3
2. MobileNet
3. ResNet50


