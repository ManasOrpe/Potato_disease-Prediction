# Potato Disease Classification using Deep Learning

**Introduction**

The agricultural sector frequently grapples with the challenge of identifying diseases in potato plants, such as early blight, late blight, or determining if the plant is healthy. These difficulties hinder timely and accurate application of treatments, adversely affecting yield and quality. To address this, we present a robust deep learning-based solution for potato disease classification, utilizing TensorFlow and a Convolutional Neural Network (CNN). This project not only streamlines disease identification but also fosters precision in farming practices, ultimately boosting productivity and quality.

<br />

**Table of Contents**

1. Key Technologies and Skills
2. Installation
3. Usage
4. Features
5. Future Scope

<br />

**Key Technologies and Skills**
- Python
- TensorFlow
- Keras
- Convolutional Neural Network (CNN)
- OpenCV
- Pillow
- Numpy
- Matplotlib
- Streamlit

<br />

**Installation**

Install the following dependencies to run this project:

```bash
pip install tensorflow
pip install opencv-python
pip install pillow
pip install numpy
pip install matplotlib
pip install streamlit
pip install streamlit_extras
```

**Note:** For compatibility issues with TensorFlow, use the following command:

```bash
pip uninstall tensorflow
pip install tensorflow==2.12.0 --upgrade
```

<br />

**Usage**

1. Clone the repository:
```bash
git clone https://github.com/ManasOrpe/Potato_disease-Prediction.git
```
2. Navigate to the project directory:
```bash
cd Potato_disease-Prediction
```
3. Install the required dependencies:
```bash
pip install -r requirements.txt
```
4. Run the Streamlit app:
```bash
streamlit run app.py
```
5. Access the app in your browser at:
```http://localhost:8501```

<br />

**Features**

#### Dataset Details:
   - The dataset was sourced from Kaggle and consists of images categorized as "Early Blight," "Healthy," and "Late Blight."
   - Dataset includes training, validation, and testing subsets to ensure reliable performance evaluation.
   
📙 Dataset Link: [Kaggle - Plant Disease Dataset](https://www.kaggle.com/datasets/emmarex/plantdisease)

#### Data Preprocessing:
   - **Image Resizing:** Images resized to 256x256 pixels.
   - **Batching:** Batches of 32 images are created.
   - **Data Augmentation:** Implemented random flips, rotations, and brightness adjustments.
   - **Caching and Prefetching:** Optimized the pipeline for faster training using TensorFlow's `cache` and `prefetch` utilities.

#### Model Architecture:
   - Utilized Keras to design a CNN with layers for resizing, rescaling, convolution, pooling, and dense connections.
   - Incorporated dropout layers to prevent overfitting and improve generalization.
   

#### Deployment:
   - The trained model was saved for deployment.
   - A Streamlit app provides a user-friendly interface for image upload and real-time disease classification.


<br />

**Future Scope**

1. **Extended Crop Support:** Expand the model to classify diseases in other crops.
2. **Mobile App Integration:** Develop a mobile application for real-time predictions in the field.
3. **Automated Alerts:** Integrate with IoT devices to notify farmers of potential outbreaks.
4. **Improved Datasets:** Augment dataset size and diversity to enhance model robustness.
5. **Real-Time Video Analysis:** Implement real-time disease detection via live camera feeds.

<br />

**Sample Output:**
![Model Inference](https://github.com/ManasOrpe/Potato_disease-Prediction/blob/main/image/Output.png.png)

<br />
