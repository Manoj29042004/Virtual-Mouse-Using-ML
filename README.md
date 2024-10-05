# Virtual Mouse Using Machine Learning

### Overview
This project explores the development of a **Virtual Mouse** that uses **machine learning** algorithms to interpret hand gestures and translate them into mouse controls. By leveraging **computer vision** through **OpenCV** and **TensorFlow**, this system enables users to control their computer mouse without physical contact, using only hand gestures.

### Features
- Gesture-based mouse control (pointer movement, clicks, scrolling)
- Customizable gestures to perform specific actions
- Real-time hand tracking and gesture recognition
- Seamless integration with graphical user interface (GUI) actions
- Works with standard laptop/desktop cameras
- Supports multiple gestures: scrolling, double click, tab switching, zoom in/out, etc.

### Algorithms Used
The system employs three main machine learning algorithms:
- **K-Nearest Neighbors (KNN)**
- **Support Vector Machine (SVM)**
- **Multilayer Perceptron (MLP) Neural Networks**

These algorithms classify hand gestures based on input data captured from the hand landmarks detected by the camera.

### Technologies Used
- **Python**: Programming language
- **OpenCV**: For computer vision and gesture detection
- **TensorFlow**: For gesture classification using MLP Neural Networks
- **PyAutoGUI**: To map gestures to mouse actions
- **Keras**: For building machine learning models
- **Mediapipe**: For hand landmark detection

### Installation & Setup
1. **Clone the repository**:
    ```bash
    git clone https://github.com/yourusername/virtual-mouse.git
    cd virtual-mouse
    ```
2. **Install required packages**:
    ```bash
    pip install -r requirements.txt
    ```

3. **Run the application**:
    ```bash
    python app.py
    ```

### How It Works
1. The camera captures video in real time.
2. **Mediapipe** detects the hand landmarks.
3. The landmarks are processed and passed through a machine learning model (KNN, SVM, or MLP) to classify the gesture.
4. Based on the recognized gesture, **PyAutoGUI** performs corresponding mouse actions such as:
    - Moving the mouse cursor
    - Clicking (left or right)
    - Scrolling up/down
    - Zoom in/out
    - Switching tabs
5. Users can customize gestures and train the system to recognize new gestures.

### Usage
- **Pointer Gesture**: Move the mouse cursor
- **Two Fingers**: Zoom in
- **Three Fingers**: Zoom out
- **Thumbs Up**: Left click
- **Thumbs Down**: Right click
- **Four Fingers**: Minimize/Maximize windows

### Project Flow
1. **Data Collection**: Hand landmarks data is collected and stored in CSV files.
2. **Model Training**: KNN, SVM, and MLP models are trained on hand landmarks data.
3. **Real-Time Gesture Detection**: The trained model is used to recognize gestures in real-time video.
4. **Mouse Control**: Recognized gestures are mapped to specific mouse actions.

### Future Enhancements
- Add support for more gestures
- Optimize hand tracking for different lighting conditions
- Integrate voice commands for enhanced accessibility
- Explore holographic projections for virtual keyboards

### Contribution
We welcome contributions! Feel free to open issues or submit pull requests.

### Acknowledgements
Special thanks to my friend **Sai Adharsh** and everyone who supported this project. This project won 1st place at the **ML Hackathon: Master the Art of Machine Learning**.

### Contact
For any queries or feedback, contact **G. Manoj** at **gudisevabrothers@gmail.com**.
