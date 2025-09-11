 
 # Pneumonia Classification Web App

This project is a Streamlit web application designed to classify chest X-ray images as either PNEUMONIA or NORMAL.

## Features

*   **AI-Powered Classification:** Utilizes a machine learning model (trained with Teachable Machine) to analyze X-ray images.
*   **Intuitive Interface:** Built with Streamlit for easy image uploads and instant classification results.
*   **Accuracy Improvement:** Achieved significant improvement in pneumonia detection accuracy on normal cases (from 30% to 69%).

## Dataset

The model was trained on the **Chest X-Ray Images (Pneumonia)** dataset:
*   **Source:** [https://data.mendeley.com/datasets/rscbjbr9sj/2](https://data.mendeley.com/datasets/rscbjbr9sj/2 )
*   **License:** CC BY 4.0
*   **Citation:** [http://www.cell.com/cell/fulltext/S0092-8674(18 )30154-5](http://www.cell.com/cell/fulltext/S0092-8674(18 )30154-5)

## How to Run Locally

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/SoukaynaHamdani/-ChestXRay-pneumonia-classification-web-app-python-streamlit.git
    cd -ChestXRay-pneumonia-classification-web-app-python-streamlit
    ```
2.  **Install dependencies:**
    ```bash
    pip install streamlit keras tensorflow pillow numpy
    ```
    *(Note: Ensure TensorFlow/Keras versions are compatible with your system and the model. )*
3.  **Place your model files:** Ensure `pneumonia_classifier.h5` and `labels.txt` (exported from Teachable Machine) are in a `./model/` directory.
4.  **Run the Streamlit app:**
    ```bash
    streamlit run main.py
    ```
    The application will open in your web browser.

## Project Structure

*   `code.py`: Main Streamlit application script.
*   `util.py`: Utility functions for background setting and image classification.
*   `./model/`: Contains the trained model (`pneumonia_classifier.h5`) and class labels (`labels.txt`).
 

