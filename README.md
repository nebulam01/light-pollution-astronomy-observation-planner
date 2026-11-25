# 🌌 Local Light Pollution & Astronomy Observation Planner

An interactive light-pollution mapping and nightly observation planning tool I built in Google Colab using `Gradio`, `NumPy`, `Pandas`, and `Matplotlib` to evaluate candidate observation sites around Kozan and surrounding corridors, inspect directional light domes, and generate a structured observation schedule.

## ✨ Key Features
- **Candidate Site & Target Selection:** Switch between candidate observation sites with elevation metadata and choose target categories (such as Open & Globular Star Clusters, Bright Planets & Moon, Faint Nebulae & Galaxies (DSO), or Visible Satellite Passes).
- **Sky & Viewing Constraints:** Tune Moon illumination (%), maximum acceptable cloud cover (%), and minimum target elevation (degrees) to tailor recommendations.
- **2D Light Pollution Map & Directional Light Dome:** Generates a dark-mode `Matplotlib` figure pairing a regional sky-brightness contour map (`mag/arcsec²`) with an azimuthal light-dome curve highlighting the darkest azimuth and brightest glare direction.
- **Full-Width Action Plan & Nightly Schedule:** Displays metric cards (Bortle class, zenith SQM, best azimuth, estimated limiting magnitude), an actionable observation plan, and a full-width nightly observation schedule table without horizontal clipping.

## 🛠️ Tech Stack
- **Environment:** Google Colab
- **Modeling, Plotting & UI:** Python, `Gradio`, `NumPy`, `Pandas`, `Matplotlib`

## ⚙️ How to Run the Project
1. **Open in Google Colab:**
   - Upload the notebook or script to Google Colab (`colab.research.google.com`).
2. **Run & Launch:**
   - Run the cell to install `gradio`, `numpy`, `pandas`, and `matplotlib` and launch the dashboard.
3. **Configure & Generate:**
   - Select a candidate site and target type, adjust Moon, cloud, and elevation sliders, and click **Map Light Pollution & Build Observation Plan**.

## 📌 Scope & Assumptions
- Designed for preliminary observation planning and educational modeling rather than certified photometric surveying or real-time weather forecasting.
- Uses an empirical radial light-decay and elevation model around regional light sources to estimate relative sky glow, SQM, Bortle class, and directional light-dome profiles.
