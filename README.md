# Traffic Sign Recognition using Deep Learning 🚦

A comprehensive deep learning project that classifies German traffic signs using CNN and ResNet50 architectures, achieving over 97% accuracy on the GTSRB dataset.

## 📋 Project Overview

This project implements and compares two deep learning approaches for traffic sign classification:
- **Custom CNN**: Built from scratch with batch normalization and dropout
- **ResNet50**: Transfer learning approach using pre-trained ImageNet weights

## 🎯 Key Results

| Model | Test Accuracy |
|-------|---------------|
| Custom CNN | **97.52%** |
| ResNet50 | **98.37%** |

## 🗂️ Dataset

- **Dataset**: GTSRB (German Traffic Sign Recognition Benchmark)
- **Classes**: 43 different traffic sign categories
- **Images**: 40x40 pixels (CNN) / 224x224 pixels (ResNet50)
- **Split**: 70% Training, 30% Validation + Separate Test Set

## 🔧 Features

### Core Implementation
- ✅ Image preprocessing (resizing, normalization, BGR to RGB conversion)
- ✅ Custom CNN architecture with batch normalization
- ✅ Transfer learning with ResNet50
- ✅ Comprehensive model evaluation

### Advanced Features
- 🚀 **Data Augmentation**: Rotation, zoom, shift, and shear transformations
- 📊 **Performance Visualization**: Training curves, confusion matrices
- 🔄 **Model Comparison**: Side-by-side performance analysis
- 💾 **Model Checkpointing**: Saves best performing models

## 🏗️ Architecture

### Custom CNN
```
Conv2D(32) → BatchNorm → MaxPool → 
Conv2D(64) → BatchNorm → MaxPool → 
Conv2D(128) → BatchNorm → MaxPool → 
Dense(512) → Dropout(0.4) → Dense(43)
```

### ResNet50 Transfer Learning
```
ResNet50(pretrained) → GlobalAvgPool → 
Dense(256) → Dropout(0.5) → Dense(43)
```

## 🛠️ Technologies Used

- **Python 3.x**
- **TensorFlow/Keras** - Deep learning framework
- **OpenCV** - Image processing
- **NumPy & Pandas** - Data manipulation
- **Matplotlib & Seaborn** - Visualization
- **Scikit-learn** - Model evaluation

## 📈 Performance Metrics

### CNN Model Performance
- **Test Accuracy**: 97.52%
- **Training Time**: ~30 epochs
- **Model Size**: Lightweight custom architecture

### ResNet50 Model Performance  
- **Test Accuracy**: 98.37%
- **Training Time**: ~20 epochs
- **Transfer Learning**: Leverages ImageNet pre-training

## 📊 Visualizations

The project generates:
- Class distribution histograms
- Training/validation accuracy curves
- Training/validation loss curves
- Detailed confusion matrices
- Model performance comparisons

## 🎓 Key Learnings

- **Data Augmentation** significantly improves model generalization
- **Transfer Learning** with ResNet50 achieves superior performance
- **Batch Normalization** helps stabilize training
- **Proper preprocessing** is crucial for model performance

## 🤝 Contributing

Feel free to fork this project and submit pull requests for any improvements!

## 🙏 Acknowledgments

- GTSRB dataset creators
- TensorFlow/Keras community
- Elevvo Pathways internship program

---

**Built with ❤️ for computer vision and deep learning**
