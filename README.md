# Autoencoder for Simulated Rings with Noise

## 🧠 Summary
This project trains an **autoencoder** — a type of neural network — to **denoise and reconstruct ring-shaped data** that has been corrupted with random noise. The dataset is made up of simulated circular patterns, which are useful for testing how well an autoencoder can learn underlying geometric structures even when the input data is noisy.

The notebook shows how the model learns to compress (encode) and then rebuild (decode) the rings, highlighting how neural networks can extract meaningful patterns from messy data.

---

## ⚙️ How It Works
1. **Data Generation:**  
   - Creates synthetic 2D ring data.  
   - Adds Gaussian noise to simulate imperfections.  

2. **Model Setup:**  
   - Builds a simple **encoder** (to reduce the data to a smaller latent space) and a **decoder** (to reconstruct it).  
   - Uses **PyTorch** for model creation and training.  

3. **Training:**  
   - The network learns by minimizing the **mean squared error (MSE)** between original and reconstructed rings.  
   - The optimizer gradually improves reconstruction quality over multiple epochs.  

4. **Results:**  
   - Shows side-by-side comparisons of noisy and reconstructed images.  
   - Displays training loss over time to visualize model improvement.

---

## ▶️ To Run
1. Install dependencies:
   ```bash
   pip install torch numpy matplotlib scikit-learn
   ```
2. Open the notebook:
   ```bash
   jupyter notebook Autoencoder_simulated_rings_with_noise_2025.ipynb
   ```
3. Run all cells in order.  
4. Adjust parameters (e.g., noise level, learning rate, epochs) to see how they affect reconstruction.

---

## 📈 Output
- Cleaned, reconstructed ring images.  
- Loss curve showing training progress.  
- Optional latent space visualization.
