# AI-Driven Monitoring and Analysis for Online Examination Management

This project aims to improve fairness and integrity in online examinations by using Artificial Intelligence (AI) technologies.  
It focuses on identity verification, real-time monitoring, plagiarism detection, and automatic reporting to help lecturers manage exams more effectively.

---

## 🎯 Project Objectives
1. To identify the requirements of an AI-driven exam integrity system to solve issues like cheating, impersonation, and plagiarism.  
2. To design the system architecture based on gathered requirements and selected AI techniques.  
3. To develop system modules using CNN, computer vision, and LLM methods.  
4. To evaluate system performance using accuracy, efficiency, and user satisfaction metrics.

---

## 🧩 Main Modules
| Module | Description | Responsible Member |
|--------|--------------|--------------------|
| **Authentication Module** | Verifies student identity using CNN-based face recognition. | Chooi Jun Xiang |
| **Real-Time Monitoring Module** | Uses computer vision to monitor student behaviour during exam. | Chooi Jun Xiang |
| **Plagiarism Detection Module** | Detects copied or AI-generated content using LLM. | Muhammad Nur Irfan Izdiyat bin Mohd Nazri |
| **Report Generation Module** | Summarises results into exam integrity reports. | Venmathy a/p Jaya Kumar |
| **Admin Dashboard Module** | Allows exam administrators to view alerts and reports. | Siti Nuurin Hayati Binti Muran Turkey |

---

## ⚙️ Technology Stack
- **Frontend:** HTML, CSS, JavaScript  
- **Backend:** Flask (Python)  
- **AI Models:** CNN (TensorFlow / PyTorch), MediaPipe, Transformers (LLM)  
- **Database:** SQLite / Firebase (optional)  

---

## 🧠 How to Run
1. Clone this repository  
   ```bash
   git clone https://github.com/Chooi-jun-xiang/AI-Driven-Monitoring-and-Analysis-for-Online-Examination-Management.git
   cd AI-Driven-Monitoring-and-Analysis-for-Online-Examination-Management

2. Install dependencies
pip install -r requirements.txt

3. Run the web app
python app.py

Documents
[Proposal_Form_Workshop II BAXI_Group 37_signed (1).pdf](https://github.com/user-attachments/files/23184343/Proposal_Form_Workshop.II.BAXI_Group.37_signed.1.pdf)
[References of workshop2 Group37.docx](https://github.com/user-attachments/files/23184368/References.of.workshop2.Group37.docx)

License
This project is developed for Workshop 2 (BAXU3923) academic purposes.

# AI-Driven Exam Integrity Module

This repository contains the software for the Plagiarism and AI-Generated Text Detection Module.

## Key Files
* `integrity_module.py`: The final, production-ready Python script containing the core `check_text_integrity` function.
* `1_Semantic_Plagiarism_Test.ipynb`: Notebook used to validate the SBERT model.
* `3_Real_AI_Detector.ipynb`: Notebook used to train the TF-IDF classifier and achieve **98.97% accuracy**.
* `4_Final_Module_Test.ipynb`: Notebook demonstrating the final combined functionality.

## ⚠️ Getting Started (For Teammates)

You must install the dependencies and acquire the data before running the notebooks.

1.  **Create and Activate Environment:**
    ```bash
    python3 -m venv my_env
    source my_env/bin/activate
    ```
2.  **Install Libraries:**
    ```bash
    pip install -r requirements.txt
    ```
3.  **ACQUIRE TRAINING DATA (CRITICAL):**
    The large training file is excluded by `.gitignore`. Please download it and place it in the root folder.
    * **File Name:** `Training_Essay_Data.csv`
    * **Source Link:** [https://www.kaggle.com/datasets/sunilthite/llm-detect-ai-generated-text-dataset](https://www.kaggle.com/datasets/sunilthite/llm-detect-ai-generated-text-dataset)
4.  **Generate Models:** Run the `3_Real_AI_Detector.ipynb` notebook to train the classifier and generate the required `.joblib` model files.

## Module Usage Example (For the Team)
To run the self-test, use your terminal:
```bash
python integrity_module.py
