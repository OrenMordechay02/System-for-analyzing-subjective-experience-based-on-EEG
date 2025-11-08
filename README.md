 🧠 System for Analyzing Subjective Experience Based on EEG

A MATLAB-based system designed to analyze and visualize subjective human experiences through EEG (Electroencephalography) data.  
The project provides tools for preprocessing, feature extraction, dataset generation, and visualization of EEG patterns related to cognitive and emotional responses.



## 📘 Overview

This project implements a modular workflow for analyzing EEG recordings collected from participants under different subjective conditions.  
It enables researchers to:
- Load and preprocess EEG data  
- Remove noise and identify bad channels  
- Extract features from multiple EEG sessions  
- Generate structured datasets for statistical or machine learning analysis  
- Visualize results in an interactive GUI



## ⚙️ Project Structure



System-for-analyzing-subjective-experience-based-on-EEG/
├── main.m                       # Entry point script
├── EEG_Profile.m                # EEG profile processing script
├── EEG_Profile_Creator.mlapp    # GUI for creating EEG profiles
├── EEG_Result_Viewer.mlapp      # GUI for viewing results
├── analyze_datasets.m           # Main analysis module
├── extract_features.m           # EEG feature extraction
├── Remove_noisy.m               # Removes noisy signals/channels
├── findNoisyChannels.m          # Detects noisy EEG channels
├── load_files.m                 # Handles loading of EEG datasets
├── plot_result.m                # Visualization utilities
├── split_EEG.m                  # Splits EEG data into segments
├── generate_dataset.m           # Creates clean, structured EEG dataset
├── metadata.txt                 # Contains metadata and configuration info
└── .git/                        # Git repository configuration





## 🧩 Requirements

- MATLAB R2021a or newer  
- Signal Processing Toolbox  
- Statistics and Machine Learning Toolbox (recommended)  

Optional (for GUI apps):  
- MATLAB App Designer support



## 🚀 How to Run

1. Clone the repository:
 
   git clone https://github.com/<your-username>/System-for-analyzing-subjective-experience-based-on-EEG.git
   cd System-for-analyzing-subjective-experience-based-on-EEG


2. Open MATLAB and set the project folder as the current directory.

3. Run the main entry point:

   main
   

4. Alternatively, you can use the GUI tools:

   * **EEG_Profile_Creator.mlapp** → Create EEG profiles
   * **EEG_Result_Viewer.mlapp** → Explore analysis results interactively



## 📊 Example Workflow

1. Load EEG dataset (`load_files.m`)
2. Preprocess signals (`Remove_noisy.m`, `findNoisyChannels.m`)
3. Extract features (`extract_features.m`)
4. Generate dataset for analysis (`generate_dataset.m`)
5. Visualize and interpret results (`plot_result.m`, `EEG_Result_Viewer.mlapp`)



## 🧠 Applications

* Cognitive and affective neuroscience
* Brain–computer interface (BCI) studies
* Subjective experience modeling
* EEG signal preprocessing pipelines
* Data-driven emotional analysis




## 🪪 License

This project is licensed under the **MIT License** 



## ⭐ Acknowledgments

Special thanks to all contributors and researchers who provided datasets, feedback, and insights related to EEG signal processing and subjective experience analysis.

