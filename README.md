# Autoencoder for Simulated Rings with Noise

## 🧠 Summary
I finalized my project goals and completed data source explorations. The data processing pipeline is now ready for data ingestion, cleaning, and normalization with realistic 2D crystallographic synthetic image data. Thousands of images were generated with random intensity values and counts, Gaussian noise was added to simulate imperfections, and radial background noise with higher intensity near the center was added. I also finalized a baseline autoencoder model in TensorFlow with Keras, using encoders to reduce the data into a smaller latent space and decoders to reconstruct it. In addition, I reviewed GAN and U-Net research directions and developed and tested the autoencoder model with different synthetic images to ensure stable performance.

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
2. Upload the file **Example: Autoencoder_simulated_rings_with_noise_2025.ipynb**.  
3. Run all cells in order.  

---

## 📈 Output
- Denoised, reconstructed crystallographic images.  
- Loss curve showing training progress.  
- Visual comparison between noisy and reconstructed samples.
