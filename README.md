# Automated Chest X-ray Report Generation  

## Overview  
This project aims to automate the process of chest X-ray classification and professional radiology report generation. It combines **deep learning** for image classification and **natural language processing (NLP)** for report generation. Using state-of-the-art architectures like **VGG16** and **OpenAI's GPT-4 API**, this project enhances diagnostic efficiency and reduces the workload on radiologists.  

## Features  
- **Image Classification**: Classifies chest X-rays into four categories:  
  - Normal  
  - Pneumonia  
  - Tuberculosis  
  - COVID-19  
- **Automated Report Generation**: Leverages **OpenAI GPT-4** to generate contextual, professional radiology reports.  
- **User Interface**: Implements a Gradio-based web interface for clinician interaction.  

## Project Structure  
The project contains the following key files:  

1. **Data Preparation**  
   - **File**: `Data_Preparation_remaining.ipynb`  
   - Description: Prepares the dataset for training by handling preprocessing tasks like resizing, normalization, and data augmentation.  

2. **VGG Model Implementation**  
   - **File**: `VGG-model.ipynb`  
   - Description: Implements the VGG16 model for multi-class classification of chest X-ray images. Achieved a test accuracy of **92.58%**.  

3. **Other Models**  
   - **File**: `otherModel.ipynb`  
   - Description: Experiments with alternative architectures (e.g., ResNet50, EfficientNetB0, Custom CNN) to compare performance.  

4. **Report Generation**  
   - Integrated **OpenAI GPT-4 API** for generating professional radiology reports based on classification results. 

**Usage**

1.  Data Preparation: Run Data_Preparation_remaining.ipynb to preprocess the dataset.
2.  Model Training:
    -Use VGG-model.ipynb to train the VGG16 model.
    -Use otherModel.ipynb to test alternative architectures.
3.  Report Generation: Integrate classification results with OpenAI GPT-4 for generating automated reports.
4.  Interface: Launch the Gradio-based interface for user interaction.

**Results**

-Classification Performance: VGG16 achieved a test accuracy of 92.58%.
-Report Quality: Generated reports are concise, -professional, and clinically relevant.

**Future Work**

-Integrate additional imaging datasets for broader classification capabilities.
-Enhance the NLP pipeline for generating more detailed multi-paragraph reports.
-Deploy the solution using Docker for scalability and cloud hosting.


## Requirements  
- Python 3.8+  
- Jupyter Notebook  
- Libraries:  
  - TensorFlow  
  - PyTorch  
  - OpenAI API  
  - Gradio  
  - NumPy, Pandas, Matplotlib, Seaborn  
  
Install dependencies using:  
```bash
pip install -r requirements.txt
