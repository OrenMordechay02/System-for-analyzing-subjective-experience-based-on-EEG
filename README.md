# 🧠 System for Analyzing Subjective Experience Based on EEG

[![MATLAB](https://img.shields.io/badge/MATLAB-R2021a%2B-blue)](https://www.mathworks.com/products/matlab.html)
[![Signal Processing Toolbox](https://img.shields.io/badge/Toolbox-Signal%20Processing-informational)](https://www.mathworks.com/products/signal.html)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Made with ❤️ by Oren](https://img.shields.io/badge/Made%20by-Oren%20Mordechay02-%23ff69b4)](https://github.com/OrenMordechay02)
[![Issues](https://img.shields.io/github/issues-raw/OrenMordechay02/System-for-analyzing-subjective-experience-based-on-EEG)](#-support--issues)

<p align="center">
  <img src="https://img.shields.io/badge/EEG-subjective%20experience-%23A855F7" alt="EEG Subjective Experience Badge">
</p>

---

## 🔍 Overview

A comprehensive MATLAB-based system designed to analyze and visualize subjective human experiences through EEG (Electroencephalography) data.
The system enables researchers to preprocess, extract features, create datasets, and visualize EEG patterns related to cognitive and emotional states.

---

## 🗂️ Project Structure

```
System-for-analyzing-subjective-experience-based-on-EEG/
├── main.m                       # Entry point script
├── EEG_Profile.m                # EEG profile processing
├── EEG_Profile_Creator.mlapp    # GUI for creating EEG profiles
├── EEG_Result_Viewer.mlapp      # GUI for viewing results
├── analyze_datasets.m           # Dataset analysis module
├── extract_features.m           # EEG feature extraction
├── Remove_noisy.m               # Noise removal
├── findNoisyChannels.m          # Detects noisy EEG channels
├── load_files.m                 # Loads EEG datasets
├── plot_result.m                # Visualization utilities
├── generate_dataset.m           # Builds structured EEG dataset
├── metadata.txt                 # Configuration and metadata
└── ...
```

---

## 🧬 Requirements

* MATLAB R2021a or newer
* Signal Processing Toolbox
* (Recommended) Statistics and Machine Learning Toolbox
* App Designer (for `.mlapp` GUIs)

---

## ⚙️ Installation & Usage

1. **Clone the Repository**

   ```bash
   git clone https://github.com/OrenMordechay02/System-for-analyzing-subjective-experience-based-on-EEG.git
   cd System-for-analyzing-subjective-experience-based-on-EEG
   ```

2. **Open MATLAB** and set the project folder as your *Current Folder*.

3. **Run the main entry point:**

   ```matlab
   main
   ```

4. **Alternatively, use the GUIs:**

   * `EEG_Profile_Creator.mlapp` → Create EEG profiles
   * `EEG_Result_Viewer.mlapp` → Visualize and interpret EEG results interactively

---

## 📊 Example Workflow

1. Load EEG dataset → `load_files.m`
2. Preprocess (remove noise) → `Remove_noisy.m`, `findNoisyChannels.m`
3. Extract features → `extract_features.m`
4. Generate dataset → `generate_dataset.m`
5. Visualize → `plot_result.m`, `EEG_Result_Viewer.mlapp`

```matlab
% Minimal example
raw = load_files('data/session01');
clean = Remove_noisy(raw);
features = extract_features(clean);
dataset = generate_dataset(features);
plot_result(dataset);
```

---

## 🔧 Outputs

* Frequency and time-domain visualizations
* Feature tables (`.mat` / `.csv`)
* Optional summary report from `extract_summary_results.m`

---

## 🛠️ Tips for Better Accuracy

* Use consistent reference (e.g., average reference)
* Remove epochs with high motion or blink artifacts (EMG/EOG)
* Verify sampling rate and event timing consistency
* Keep versioned pipelines for reproducibility

---

## 👥 Contributing

Contributions are welcome!

1. Open an **Issue** describing your idea or bug.
2. Fork the repo → Create a **feature branch** (e.g., `feature/artifact-detection`).
3. Submit a **Pull Request** with screenshots or data samples if relevant.

Please maintain respectful communication and ensure your code runs before submitting.

---

## 🔖 License

Distributed under the **MIT License**. See `LICENSE` for more information.

---

## 📩 Support & Issues

If you encounter problems:

* Open an [Issue](../../issues) with MATLAB version, OS, reproduction steps, and screenshots/logs.
* Or contact: **[orenmor02@gmail.com](mailto:orenmor02@gmail.com)**

---

## 🌐 English Summary

**System for Analyzing Subjective Experience Based on EEG** is a MATLAB toolkit for EEG preprocessing, feature extraction, dataset generation, and visualization. It supports channel-noise detection, segmenting signals, and statistical/ML-based analysis.

**Quick Start:**

```matlab
main
```

**License:** MIT
**Author:** [Oren Mordechay02](https://github.com/OrenMordechay02)

---

### 📖 Citation

```bibtex
@software{mordechay2025eegsubjective,
  author  = {Oren Mordechay},
  title   = {System for Analyzing Subjective Experience Based on EEG},
  year    = {2025},
  url     = {https://github.com/OrenMordechay02/System-for-analyzing-subjective-experience-based-on-EEG}
}
```
