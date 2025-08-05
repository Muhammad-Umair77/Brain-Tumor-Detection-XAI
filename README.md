brain-tumor-detection/
│
├── model/                         # Saved model file (.h5)
│   └── brain_tumor_model.h5
│
├── Testing/                      # Sample test images
│   ├── glioma_tumor/
│   ├── meningioma_tumor/
│   ├── pituitary_tumor/
│   └── no_tumor/
│
├── app.py                        # Main Streamlit app
├── predict.py                    # Prediction and preprocessing logic
├── lime_explain.py               # LIME explanation generation
├── requirements.txt              # Required libraries
└── README.md                     # This file

#Installation
1. Clone the repository

   git clone https://github.com/yourusername/brain-tumor-detection.git
cd brain-tumor-detection

2. Create virtual environment and activate
  python -m venv venv
source venv/bin/activate   # On Windows: venv\Scripts\activate

3.Install dependencies
pip install -r requirements

4.🚀 Run the Streamlit App
streamlit run app.py

🧪 Dataset
Dataset used: Brain MRI Images for Brain Tumor Detection

Source: Kaggle Dataset

📊 Model Details
Input size: 224x224x3

Architecture: Custom CNN with Conv2D, MaxPooling, and Dense layers

Output: 4-class Softmax

Loss: Categorical Crossentropy

Accuracy: ~97% on test set

💡 LIME Explanation
LIME explains individual predictions by perturbing input and observing the effect.

Highlights most influential regions of the image that affect the decision.

Helps build trust in model's predictions, especially for medical professionals.

📚 Future Enhancements
Support for DICOM images

Integration of patient metadata

Doctor feedback loop

Deployment to cloud or mobile

👤 Author
Your Name
Muhammad-Umair77

📝 License
This project is licensed under the MIT License.
