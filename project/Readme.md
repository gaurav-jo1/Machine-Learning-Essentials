# Transfer-ViT-Classifier 🧠

Welcome to **Transfer-ViT-Classifier**, a modular PyTorch portfolio project showcasing an end-to-end transfer learning workflow for image classification. This notebook adapts a pre-trained Vision Transformer (ViT-B/16) to a custom 3-class food dataset (pizza, steak, sushi), freezing the backbone for efficient fine-tuning while achieving ~98% top-1 accuracy. It emphasizes reproducibility, GPU acceleration, and production prototyping—going beyond basic models to deliver scalable, high-performance results.

Key highlights:
- **Efficient Adaptation**: Leverage pre-trained ViT weights; train only the classifier head on ~750 images for quick convergence.
- **Robust Evaluation**: Comprehensive metrics (accuracy, precision, recall, F1) with confusion matrix and sample predictions.
- **Reproducible Setup**: Seeded random states, data augmentation via torchvision transforms, and modular functions for easy extension.

<img width="1214" height="624" alt="download" src="https://github.com/user-attachments/assets/03557ac4-5e23-4700-aaad-d6c72d22a367" />

## Getting Started 🔥

Follow these steps to run the project locally:

1. Clone the repository (or navigate to the project folder in your existing repo):
   ```sh
   git clone https://github.com/gaurav-jo1/Machine-Learning-Essentials.git
   ```

2. Navigate to the project directory:
   ```sh
   cd project
   ```

## Troubleshooting

- **GPU Issues**: Set `device = 'cpu'` if no CUDA; check with `torch.cuda.is_available()`.
- **Dataset Errors**: Verify folder structure matches ImageFolder expectations.
- **Dependencies**: If using Colab, copy-paste cells and mount Drive for data.
