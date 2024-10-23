

# 🎵 Emotion-Based Music Recommendation System 🎵

This is a web-based application written in Python that analyzes a user's emotions via facial recognition and then recommends music based on their detected emotions. The app leverages **OpenCV** to capture your face, a **machine learning model** to predict the emotions, and **Streamlit** to provide an interactive and user-friendly interface.

## ✨ Features

- Real-time emotion detection using your webcam.
- Recommends music based on your emotions (happy, sad, neutral, etc.).
- Emotion analysis happens 30-40 times in 2-3 seconds to generate a sorted list of emotions.
- Removes duplicates and recommends songs based on the most frequent emotions.

---

## 🚀 Getting Started

Follow these steps to get the project up and running locally.

### 1. Clone the Repository
First, clone this repository to your local machine:
```bash
cd emotion-music-recommendation
```

### 2. Create and Activate a Virtual Environment
It's best practice to use a virtual environment to manage dependencies. You can create and activate one using the following commands:

- **Windows (PowerShell or Command Prompt):**
    ```bash
    python -m venv venv
    .\venv\Scripts\Activate
    ```

- **macOS / Linux:**
    ```bash
    python3 -m venv venv
    source venv/bin/activate
    ```

### 3. Install Dependencies
With your virtual environment activated, install all required libraries:
```bash
pip install -r requirement.txt
```

### 4. Run the Application
Once all dependencies are installed, you can launch the application using Streamlit:
```bash
streamlit run app.py
```

---

## 📚 Libraries Used

- **[Streamlit](https://streamlit.io/)**: For building the interactive web app interface.
- **[OpenCV](https://opencv.org/)**: For facial recognition and image processing.
- **[Numpy](https://numpy.org/)**: For numerical operations.
- **[Pandas](https://pandas.pydata.org/)**: For data manipulation and analysis.
- **[TensorFlow](https://www.tensorflow.org/)** & **[Keras](https://keras.io/)**: For building and running the machine learning model.

---

## 📷 How It Works

1. **Emotion Detection**: The app uses OpenCV to capture video frames from your webcam. It then crops the image of your face from the frame.
   
2. **Machine Learning Model**: The cropped face image is passed to a pre-trained ML model that detects your emotions.

3. **Sorting Emotions**: The app captures multiple emotions within a short time frame (2-3 seconds) and creates a list of emotions sorted by frequency. Duplicate entries are removed, leaving only the most common emotions.

4. **Music Recommendation**: Based on your detected emotions, the app recommends songs that match your emotional state.

---


---

## 🛠️ Additional Configuration

### Webcam Permissions
Make sure your browser has granted permission to use the webcam when accessing the app.

### Virtual Environment (Optional)
To deactivate the virtual environment when you're done, simply run:
```bash
deactivate
```
---
## Screemshot:
![2](https://github.com/user-attachments/assets/b2c6af3b-aa14-4706-b6f0-2327b9b02fa0)
![3](https://github.com/user-attachments/assets/623b94fe-2f03-4b4b-bdb2-b21dadf08741)
![1](https://github.com/user-attachments/assets/30c98a05-4bbc-4bd8-8b19-7afaa4c65be8)
---
---

## 💡 Future Improvements
- Incorporate more emotions for better music recommendations.
- Add a feedback loop to improve the recommendation algorithm based on user preferences.
- Include a playlist generation feature from music streaming services like Spotify.

---

## 🎉 Conclusion

Now you can easily discover music that matches your mood! 

---
