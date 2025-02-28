# **Focus Line App**
![image](https://github.com/user-attachments/assets/3ee42e9b-f009-4018-987f-2b1acfd0cb67)

This app is designed to help manage stress while working on a computer by reminding users to take breaks when necessary. The app is built with a neural network that analyzes users' stress levels based on facial expressions.

## **Key Features:**
- **Automatic Stress Detection**: The app captures a photo every 30 seconds through the webcam and sends it to the server, where a machine learning model processes the image to predict whether the user is stressed or not.
- **Real-Time Predictions**: The model, trained on a dataset of 8,000 images of human faces categorized as "stress" or "no stress," predicts the user's stress level in real-time.
- **Background Operation**: The app works in the background while you're using your computer, making it unobtrusive and easy to integrate into your workflow.
- **Concentration Score**: Based on the predictions, the app maintains a concentration score. If this score drops too low, the app suggests taking a break to improve focus and reduce stress.

## **How It Works:**
1. The app runs in the browser and communicates with the server through a RESTful API.
2. Every 30 seconds, the app automatically takes a photo using your webcam, which is sent to the server for analysis.
3. The server processes the image using the neural network model and returns a stress prediction.
4. The app then updates the concentration score, which influences suggestions for breaks.
