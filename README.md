# MedTech - Disease Prediction System 🩺

MedTech is an intelligent, user-friendly disease prediction system designed to provide preliminary health insights based on user-reported symptoms. By leveraging a comprehensive database of diseases and their corresponding symptoms, this tool helps users identify potential health conditions, understand the associated risk levels, and find the appropriate medical specialist for consultation.

![MedTech Logo](finalwhite.png)

## 📋 Table of Contents

- [Features](#-features)
- [How It Works](#-how-it-works)
- [Technologies Used](#-technologies-used)
- [Setup and Installation](#-setup-and-installation)
- [How to Use](#-how-to-use)
- [Disclaimer](#%EF%B8%8F-disclaimer)

## ✨ Features

-   **Symptom-Based Diagnosis**: Select your symptoms from an extensive, alphabetized list to get instant predictions.
-   **Disease Information**: Identifies one or more likely diseases based on the combination of selected symptoms.
-   **Risk Level Assessment**: Each predicted disease is assigned a risk level (High, Moderate, or Low) to help users understand the severity.
-   **Specialist Recommendation**: Recommends the type of medical specialist to consult for the predicted condition (e.g., Pulmonologist, Neurologist, etc.).
-   **User-Friendly Interface**: Built with Streamlit for a clean, interactive, and easy-to-navigate web interface.
-   **Informational Sections**: Includes "About Us" and "Contact" sections for more information and support.

## ⚙️ How It Works

The application works by matching the user's selected symptoms against a predefined dictionary of diseases and their common symptoms.

1.  The user selects symptoms from a multi-select dropdown.
2.  The `detect_diseases` function calculates how many of the selected symptoms match the symptoms of each disease in the database.
3.  It identifies the disease(s) with the highest number of matches.
4.  For each likely disease, it retrieves and displays the predefined risk level and the recommended medical specialist(s).

## 💻 Technologies Used

-   **Python**: The core programming language.
-   **Streamlit**: For building and deploying the interactive web application.

## 🚀 Setup and Installation

To run this project locally, follow these steps:

1.  **Clone the repository:**
    ```sh
    git clone [https://github.com/your-username/MedTech.git](https://github.com/your-username/MedTech.git)
    cd MedTech
    ```

2.  **Install the required libraries:**
    Make sure you have Python installed. Then, install Streamlit.
    ```sh
    pip install streamlit
    ```

3.  **Run the application:**
    Open your terminal in the project directory and run the following command:
    ```sh
    streamlit run MedTech.py
    ```
    Your web browser will automatically open with the application running.

## 📖 How to Use

1.  Launch the application.
2.  You will see a dropdown menu labeled "Select your symptoms:".
3.  Click on the dropdown and select all the symptoms you are experiencing. You can type to search for symptoms.
4.  Once you have selected your symptoms, click the **"Get Diagnosis"** button.
5.  The system will display the predicted disease(s), the risk level, and the recommended specialist(s) to consult.
6.  Scroll down to read the disclaimer and learn more about the project in the "About Us" and "Contact" sections.

## ⚠️ Disclaimer

This tool is for informational purposes only and is not a substitute for professional medical advice, diagnosis, or treatment. Always seek the advice of a qualified healthcare provider with any questions you may have regarding a medical condition.

---

### Risk Assessment Criteria

-   **High**: Diseases with a high fatality rate, rapid progression, or potential for outbreaks.
-   **Moderate**: Diseases with significant health impacts but lower fatality rates or slower progression.
-   **Low**: Diseases that are usually manageable or cause mild symptoms.
