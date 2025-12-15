# Segment Anything Model (SAM) Usage Examples

A practical Jupyter Notebook demonstrating various usage modes of the **Segment Anything Model (SAM)** by Meta AI. This repository provides a complete guide for running SAM, focusing on:
* Prompt-based segmentation (using points and bounding boxes).
* Full automatic image mask generation.

---

## ⚙️ Requirements and Setup

To run the `SAM_example.ipynb` notebook successfully, you need to set up your environment with these prerequisites:

### 1. Python Libraries

The notebook requires the following core packages, which can be installed via `pip`:

```bash
# Install PyTorch and related libraries
pip install torch torchvision

# Install the Segment Anything library and utility packages
pip install segment-anything opencv-python Pillow
```

## SAM Model Checkpoint

You must download the pre-trained weights for the Segment Anything Model.

  1. Download a checkpoint file (e.g., sam_vit_h_4b8939.pth for the largest model) from the official SAM repository or checkpoint source.

  2. Crucially: Place the downloaded .pth file in the same directory as the SAM_example.ipynb notebook.

## 🚀 Usage Guide
The included SAM_example.ipynb file is designed to be executed cell-by-cell in a sequential manner within a Jupyter environment (such as Jupyter Notebook, JupyterLab, or Google Colab).

### Key Demonstrations in the Notebook:

| Task | Description | Output File Example |
| :--- | :--- | :--- |
| **Point Prompting** | Generating a precise mask by supplying a single coordinate (point) within the target object. | `point_mask.png` |
| **Box Prompting** | Generating a mask by supplying a bounding box around the target object. | `polygon_mask.png` |
| **Automatic Masking** | Generating high-quality, discrete masks for all recognizable entities in the image. | `auto_mask_0.png`, `auto_mask_1.png`, etc. |


## ⚖️ Credits

This example code is built around the **Segment Anything Model (SAM)**, which was developed and released by **Meta AI**.
Research Paper (Segment Anything): arxiv.org/abs/2304.02643
