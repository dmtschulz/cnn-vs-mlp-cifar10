# CNN vs MLP on CIFAR-10

This project compares Convolutional Neural Networks (CNNs) and Multilayer Perceptrons (MLPs) on the CIFAR-10 image classification task.  
We evaluate both architectures in terms of accuracy, number of parameters, robustness to input translations, and feature map interpretability.

## 📌 Key Highlights

- **Model Architectures**: MLP (3 layers) vs CNN (3 conv blocks)
- **Dataset**: CIFAR-10 (reduced for faster experimentation)
- **Robustness Test**: Accuracy drop on translated images
- **Visualization**: Feature maps from CNN layers
- **Plotting**: Training curves, boxplots for accuracy and robustness

## 🧰 Tools Used

- Python
- PyTorch
- torchvision
- matplotlib
- tqdm

## 🚀 Results Summary

| Metric                       | MLP      | CNN      |
|-----------------------------|----------|----------|
| Test Accuracy (avg)         | `41.12%` | `64.88%` |
| Accuracy (with translations)| `31.21%` | `57.14%` |
| Trainable Params            | `3.705K`   | `486K`   |

## 📁 Files

- `cnn_mlp_cifar10_analysis.ipynb` — Main notebook with code and visualizations
- `plots/` — Output plots (training curves, accuracy boxplots, feature maps)

## 🧠 Insights

CNNs outperform MLPs not just in accuracy but also in generalization to perturbed inputs.  
Their local connectivity and weight sharing give them a clear advantage for image-based tasks.

## 🔗 To Run
Requires Python 3.10+, CUDA optional but recommended.
```bash
pip install -r requirements.txt
````
Disclaimer: This project was originally an academic assignment. It was refactored and extended for inclusion in a public portfolio.