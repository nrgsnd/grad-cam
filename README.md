# 🔍 Grad-CAM Visualization for DiffAD

This notebook provides a visualization of model attention using **Grad-CAM** (Gradient-weighted Class Activation Mapping) for the **DiffAD** model — a diffusion-based framework for time series anomaly detection.

## 📥 Download DiffAD

Before running this notebook, download and set up the original **DiffAD** repository from the official GitHub page:

👉 [https://github.com/ChunjingXiao/DiffAD/tree/main](https://github.com/ChunjingXiao/DiffAD/tree/main)

Follow the instructions in their README to install dependencies and prepare data/models.

---

## 📁 Notebook

### `Grad_cam.ipynb`

This notebook demonstrates how to apply Grad-CAM to visualize which parts of the input time series influence the model's anomaly predictions.

### Highlights:
- Uses hooks to extract gradients and feature maps from internal layers of the DiffAD model.
- Supports time series visualization overlaid with class activation maps.
- Helpful for model interpretability and understanding how DiffAD reacts to anomalous segments.

---

## 🛠️ Requirements

Install dependencies (in the same environment as DiffAD):

```bash
pip install matplotlib numpy torch torchvision opencv-python
```

---

## ▶️ Running the Notebook

1. Clone the DiffAD repository:
   ```bash
   git clone https://github.com/ChunjingXiao/DiffAD.git
   cd DiffAD
   ```

2. Place `Grad_cam.ipynb` inside the project directory.

3. Launch Jupyter:
   ```bash
   jupyter notebook Grad_cam.ipynb
   ```

4. Run the notebook cells to generate Grad-CAM visualizations for a sample or your own time series input.

---

## 📚 References

- **DiffAD**: Xiao et al. (2023), *Diffusion Models for Anomaly Detection in Time Series*
- **Grad-CAM**: Selvaraju et al. (2017), [Paper](https://arxiv.org/abs/1610.02391)

