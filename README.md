# Explainable Deep Multi-Branch Neural Network for Recognizing Autonomic Activation States from Multimodal Physiological Signals
## 1.Project Overview
This project, developed as part of the **graduation thesis**, proposes an **explainable deep multi-branch neural network** designed to recognize **autonomic activation states** from **multimodal physiological signals**. Using the WESAD dataset, the model integrates signals such as ECG, EDA, and respiration to detect stress and affect states. 
The project demonstrates:
- The application of deep learning techniques to wearable physiological data.
- The use of explainability methods (e.g., attention maps) to interpret model decisions.
- Training and evaluation using GPU resources on Kaggle for efficient experimentation.
## 2. Dataset
- **Dataset used**: [WESAD Wearable Stress and Affect Detection](https://ubi29.informatik.uni-siegen.de/usi/data_wesad.html) 
- **Disclaimer**: You may use this data for scientific, non-commercial purposes, provided that you give credit to the owners when publishing any work based on this data.
## 3. Environment & Requirements
- **Platform**: Kaggle Notebook
- **Accelerator**: GPU T4 x2
- **Python version**: 3.10+
- **Libraries**: See [requirements.txt](requirements.txt)
- GPU acceleration is strongly recommended for model training.
## 4. Instructions to Run 
### Step 1: Setup Kaggle Notebook
- Open a new Kaggle Notebook.
- Upload the project code folder to your Kaggle workspace.
- Make sure the **WESAD dataset** is added from Kaggle Datasets.
  - For example:
  ```python
  WESAD_PATH = '/kaggle/input/wesad-dataset/WESAD'
  ```
  - If you fork/run this notebook, please update `WESAD_PATH` to match your own dataset path on Kaggle.
### Step 2: Install dependencies
Simply run the provided `!pip install ...` commands inside the main notebook to install required libraries.
### Step 3: Run the main notebook
- Open and execute `notebooks/main-notebook.ipynb`.
- The notebook includes:
  - **Data preprocessing** (signal filtering, feature extraction).
  - **Model training** (multi-branch neural network on GPU).
  - **Evaluation & Explainability** (metrics, attention maps).
## 5. Results & Outputs
- Trained models, figures, and evaluation metrics will be saved in the outputs/ folder.
- Include key metrics: Accuracy, F1-score, Confusion Matrix, and explainability visualizations.
## 6. References
Schmidt, P., Reiss, A., Duerichen, R., Marberger, C., & Van Laerhoven, K. (2018). Introducing WESAD, a multimodal dataset for wearable stress and affect detection. In Proceedings of the 20th ACM International Conference on Multimodal Interaction (pp. 400–408). ACM. doi:[10.1145/3242969.3242985](https://doi.org/10.1145/3242969.3242985)
## 7. Author
- **Do Ngoc Phuong Anh** - Graduation Thesis, University of Economics Ho Chi Minh City (UEH)
- **Contact**: anhdo.31221020325@st.ueh.edu.vn (during thesis) | anhdo5058@gmail.com (personal) | Github: [dnp-anh](https://github.com/dnp-anh)

