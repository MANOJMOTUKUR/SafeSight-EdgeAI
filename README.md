# SafeSight: Offline Edge AI for Visually Impaired Safety

## 🎥 Project Demonstration
**[WATCH THE DEMO VIDEO HERE](PASTE_YOUR_YOUTUBE_OR_DRIVE_LINK_HERE)**

## 📝 Project Description
SafeSight is a privacy-first Edge AI system designed to assist visually impaired individuals. Using the **FOMO (Faster Objects, More Objects)** architecture, it detects and distinguishes between "Safe Consumables" (e.g., water bottles) and "Danger/Chemicals" (e.g., cleaning fluid) in milliseconds, running entirely offline on edge devices.

## 📂 Dataset Preparation
- **Source:** Custom collected dataset using Smartphone Camera.
- **Size:** 120+ images.
- **Classes:** `Safe_Item` vs `Danger_Item`.
- **Preprocessing:** Images were resized to 96x96 Grayscale to optimize for latency on Cortex-M4 microcontrollers.
- **Augmentation:** Random rotation, zoom, and noise were applied during training to improve generalization.

## 🧠 Model Training
- **Platform:** Edge Impulse Studio.
- **Architecture:** MobileNetV2 0.35 (FOMO).
- **Parameters:**
  - Epochs: 50
  - Learning Rate: 0.005
  - Batch Size: 32
- **Performance:** Achieved >85% F1 Score on the Test Set.

## 💻 Application Development
The model was deployed as a C++ Library optimized for Arduino/embedded usage. The system performs inferencing locally without WiFi, ensuring privacy and speed.

## 🔗 Links
- **Edge Impulse Project:** [PASTE_YOUR_EDGE_IMPULSE_PUBLIC_LINK_HERE]
