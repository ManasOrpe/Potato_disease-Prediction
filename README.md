# Potato Disease Classification using Deep Learning

**Introduction**

Hi there! I'm Manas, and I want to share an exciting project I’ve been working on. If you’re curious about how technology can transform agriculture, you’re in the right place. Farmers often struggle with identifying diseases in potato plants, such as early blight or late blight, or even determining if the plant is healthy. This can lead to delays in applying treatments and, ultimately, reduced yield and quality. That’s where this project steps in! 

Using deep learning, specifically TensorFlow and Convolutional Neural Networks (CNN), we’ve built a model that makes disease identification straightforward and efficient. This solution is designed to help farmers apply treatments on time, improve resource management, and boost crop quality. Let’s dive in!

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

To get started with this project, you’ll need to install a few dependencies. Here’s how:

```bash
pip install tensorflow
pip install opencv-python
pip install pillow
pip install numpy
pip install matplotlib
pip install streamlit
pip install streamlit_extras
```

**Note:** If you run into any issues with TensorFlow, especially the dreaded "ImportError: DLL load failed," use this:

```bash
pip uninstall tensorflow
pip install tensorflow==2.12.0 --upgrade
```

<br />

**Usage**

Here’s how you can use this project:

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
5. Open your browser and access the app at:
```http://localhost:8501```

<br />

**Features**

#### Dataset Details:
   - I sourced the dataset from Kaggle. It includes images of potato leaves categorized into "Early Blight," "Healthy," and "Late Blight."
   - The dataset is split into training, validation, and testing subsets for better evaluation.

📙 Dataset Link: [Kaggle - Plant Disease Dataset](https://www.kaggle.com/datasets/emmarex/plantdisease)

#### Data Preprocessing:
   - **Image Resizing:** All images were resized to 256x256 pixels.
   - **Batching:** Images were grouped into batches of 32.
   - **Data Augmentation:** Techniques like random flips, rotations, and brightness adjustments were applied to make the model robust.
   - **Caching and Prefetching:** These TensorFlow features were used to speed up training by optimizing the data pipeline.

#### Model Architecture:
   - The model was built using Keras, featuring layers for resizing, rescaling, convolution, pooling, and dense connections.
   - Dropout layers were added to reduce overfitting and improve performance.

#### Deployment:
   - The trained model was saved and integrated into a Streamlit app.
   - The app allows users to upload images and receive real-time disease classification results.


<br />

**Future Scope**

This is just the beginning! Here are some ways I plan to expand this project:

1. **Extended Crop Support:** Incorporate datasets for other crops to widen the scope of disease classification.
2. **Mobile App Integration:** Create a mobile app so farmers can get real-time predictions directly in the field.
3. **Automated Alerts:** Combine this with IoT devices to send notifications about potential outbreaks.
4. **Improved Datasets:** Add more diverse images to make the model even more robust.
5. **Real-Time Video Analysis:** Enable live disease detection through video streams.

<br />

**Sample Output:**

Here’s a quick look at what the model can do:

![Model Inference](https://github.com/ManasOrpe/Potato_disease-Prediction/blob/main/image/Output.png.png)

<br />

Thanks for stopping by and checking out my project! If you have any questions or suggestions, feel free to reach out. Let’s work together to make agriculture smarter and more efficient!
