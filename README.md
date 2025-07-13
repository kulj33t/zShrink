# zShrink: VAE-based Image Compression

![Model](https://img.shields.io/badge/model-VAE-red)
![Compression](https://img.shields.io/badge/focus-Latent%20Space%20Compression-blue)

**zShrink** is a research-oriented image compression pipeline using **Variational Autoencoders (VAEs)** that compress images by shrinking their latent representations rather than directly reducing pixel data.

---

## 🚀 Highlights

* 🔍 Compresses at the **latent space** level for intelligent and content-aware image compression.
* 🧠 Built upon **VAE** architecture — capturing meaningful data distribution.
* 💡 Custom modules for shrinkage, entropy evaluation, and image reconstruction.
* 📊 Evaluates compression quality using PSNR, SSIM, and latent size.

---



## 🧬 Methodology

1. **VAE Encoder** learns a latent distribution from image space.
2. **Latent Shrinking** applies vector quantization or thresholding to minimize latent dimensionality.
3. **Decoder** reconstructs image from compressed latent code.
4. **Evaluation** is performed comparing original vs. reconstructed images.

---

## 🏋️‍♂️ Training 

* Model training
* Latent shrink experiments
* Visual results
* Metric calculation

---

## 📊 Results

| Metric                  | Value (Sample) |
| ----------------------- | -------------- |
| **PSNR**                | \~28.5 dB      |
| **SSIM**                | \~0.89         |
| **Latent Shrink Ratio** | \~65%          |

> Metrics may vary based on image resolution and shrink method.

---




---

## 🔧 Requirements

```bash
pip install -r requirements.txt
```

* PyTorch
* NumPy
* Matplotlib
* scikit-image
* Jupyter

---

## 📌 TODO

* [ ] Add multi-stage compression pipeline
* [ ] Support custom datasets
* [ ] Deploy as Streamlit/Web demo
* [ ] Add comparative study with JPEG/PNG

---

## 🙌 Acknowledgements

* Based on foundational work in **Variational Autoencoders (Kingma & Welling)**
* Inspired by techniques in **learned compression** and **information bottlenecks**

