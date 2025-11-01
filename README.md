# Autoencoder for Simulated Rings with Noise

## 🧠 Summary
This project trains an **autoencoder** — a type of neural network — to **denoise and reconstruct crystallographic ring-shaped data** that has been corrupted with noise. The dataset is made up of simulated diffraction-like patterns containing rings and dots with varying intensities, designed to resemble noisy experimental images.  

The notebook demonstrates how the model learns to compress (encode) and rebuild (decode) the data, showing how neural networks can extract key structural features from noisy input images.

---

## ⚙️ How It Works
1. **Data Generation:**  
   - Creates realistic synthetic 2D crystallographic data with rings and dots.  
   - Generates rings and dots with random intensity values and counts.  
   - Adds Gaussian noise to simulate imperfections.  
   - Adds radial background noise with higher intensity near the image center.  

2. **Model Setup:**  
   - Builds an autoencoder model with an **encoder** (to reduce the data to a smaller latent space) and a **decoder** (to reconstruct it).  
   - Uses **TensorFlow** with **Keras** for model creation and training.  

3. **Training:**  
   - The network learns by minimizing the **mean squared error (MSE)** between original and reconstructed images.  
   - The optimizer gradually improves reconstruction quality over multiple epochs.  

4. **Results:**  
   - Shows side-by-side comparisons of noisy and reconstructed images.  
   - Displays training loss over time to visualize model improvement.

---

## ▶️ To Run
1. Open [Google Colab](https://colab.research.google.com).  
2. Upload the file **Autoencoder_simulated_rings_with_noise_2025.ipynb**.  
3. Run all cells in order.  

---

## 📈 Output
- Denoised, reconstructed crystallographic images.  
- Loss curve showing training progress.  
- Visual comparison between noisy and reconstructed samples.
