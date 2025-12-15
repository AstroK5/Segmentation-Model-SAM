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
