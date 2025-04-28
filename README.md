
# Data Augmentation with DCGANs

![DCGAN Example Output](./dcgan_training_progress.gif)

## 📜 Project Overview

Medical imaging datasets, especially for conditions like pneumonia, often suffer from limited availability. This project leverages **Deep Convolutional Generative Adversarial Networks (DCGANs)** to generate synthetic chest X-ray images, augmenting the existing **Chest X-ray Pneumonia** dataset. By doing so, we aim to improve the robustness and diversity of training datasets for deep learning models used in medical diagnostics.

---

## 🚀 Highlights

- **Model:** Deep Convolutional GAN (DCGAN)
- **Dataset:** [Chest X-ray Pneumonia Dataset](https://www.kaggle.com/datasets/paultimothymooney/chest-xray-pneumonia)
- **Purpose:** Generate realistic synthetic X-ray images for data augmentation
- **Framework:** PyTorch

---

## 🏗️ Architecture

### Generator
- Random noise vector → 64x64 RGB image
- Transposed convolutions, BatchNorm, ReLU/Tanh activations

### Discriminator
- 64x64 RGB image → Real/Fake probability
- Convolutions, BatchNorm, LeakyReLU activations

---

## 🛠️ Dataset & Preprocessing

- Resize to **64x64**
- Normalize to **[-1, 1]**
- Batch Size: **128**

---

## 📈 Training Details

- **Epochs:** 20
- **Optimizer:** Adam
- **Loss Function:** Binary Cross Entropy (BCE)
- **Checkpoint:** Save model every 5 epochs

---

## 🎞️ Training Progress

![DCGAN Training Progress](./dcgan_training_progress.gif)

---

## 📚 References

- [DCGAN Paper](https://arxiv.org/pdf/1511.06434)
- [PyTorch DCGAN Tutorial](https://pytorch.org/tutorials/beginner/dcgan_faces_tutorial.html)

---

## 📬 Contact

**Sharon Dev Saseendran**  
Email: [your-email@example.com]  
LinkedIn: [your-linkedin-profile]  

---

# License

This project is licensed under the MIT License.
