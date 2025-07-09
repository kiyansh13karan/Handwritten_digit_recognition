# Handwritten Digit Recognition

A comprehensive machine learning application that recognizes handwritten digits (0-9) using a neural network trained on the MNIST dataset. The project includes both a command-line interface and a modern web-based Streamlit application.

## 📸 Project Screenshots

<!-- Add your screenshots here -->
*Main Application Interface*
![Main Interface]<img width="1920" height="1200" alt="Image" src="https://github.com/user-attachments/assets/e6655979-43d5-4044-87b8-ea8463690630" />

*Prediction Results*
![Prediction Results]<img width="1920" height="1200" alt="Image" src="https://github.com/user-attachments/assets/b102f663-8a08-400d-9a48-16d9068ba68e" />

*Probability Distribution*
![Probability Distribution](screenshots/probability_chart.png)

## 🚀 Features

- **Neural Network Model**: Custom-built neural network with 98% accuracy on MNIST test set
- **Web Interface**: Modern, responsive Streamlit web application
- **Image Upload**: Support for PNG, JPG, and JPEG image formats
- **Real-time Prediction**: Instant digit recognition with confidence scores
- **Visual Analytics**: Interactive probability distribution charts
- **Batch Processing**: Command-line tool for processing multiple images
- **Model Persistence**: Automatic model saving and loading

## 🛠️ Technology Stack

- **Machine Learning**: TensorFlow/Keras
- **Web Framework**: Streamlit
- **Image Processing**: OpenCV, PIL
- **Data Visualization**: Matplotlib
- **Data Handling**: NumPy

## 📋 Requirements

- Python 3.7+
- TensorFlow 2.12.0+
- OpenCV 4.8.0+
- Streamlit 1.30.0+
- NumPy 1.24.0+
- Pillow 10.0.0+
- Matplotlib 3.7.0+

## 🔧 Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/handwritten-digit-recognition.git
   cd handwritten-digit-recognition
   ```

2. **Create a virtual environment** (recommended)
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

## 🎯 Usage

### Web Application (Streamlit)

1. **Launch the web application**
   ```bash
   streamlit run app.py
   ```

2. **Open your browser** to `http://localhost:8501`

3. **Upload an image** of a handwritten digit (0-9)

4. **Click "Predict Digit"** to see the results

### Command Line Interface

1. **Create a digits directory** and add your 28x28 pixel images:
   ```bash
   mkdir digits
   # Add your digit images as digit1.png, digit2.png, etc.
   ```

2. **Run the command-line version**:
   ```bash
   python handwritten_digits_recognition.py
   ```

## 🧠 Model Architecture

The neural network consists of:

- **Input Layer**: 784 neurons (flattened 28×28 pixel image)
- **Hidden Layer 1**: 128 neurons with ReLU activation
- **Hidden Layer 2**: 128 neurons with ReLU activation
- **Output Layer**: 10 neurons with Softmax activation (for digits 0-9)

### Training Details

- **Dataset**: MNIST (60,000 training images, 10,000 test images)
- **Optimizer**: Adam
- **Loss Function**: Sparse Categorical Crossentropy
- **Epochs**: 3
- **Accuracy**: ~98% on test set

## 📁 Project Structure

```
handwritten-digit-recognition/
├── app.py                              # Streamlit web application
├── handwritten_digits_recognition.py   # Command-line interface
├── requirements.txt                    # Python dependencies
├── README.md                          # Project documentation
├── handwritten_digits.keras          # Saved model (generated after training)
├── digits/                           # Directory for test images
│   ├── digit1.png
│   ├── digit2.png
│   └── ...
└── screenshots/                      # Project screenshots
    ├── main_interface.png
    ├── prediction_results.png
    └── probability_chart.png
```

## 🎨 Web Interface Features

### Main Dashboard
- Clean, modern UI with responsive design
- Real-time image upload and preview
- Intuitive navigation with tabs

### Prediction Results
- Large, clear display of predicted digit
- Confidence percentage
- Interactive probability distribution chart
- Visual feedback for all predictions

### About Section
- Technical details about the model
- Information about the MNIST dataset
- Potential applications and use cases

## 🔄 How It Works

1. **Image Preprocessing**:
   - Convert uploaded image to grayscale
   - Resize to 28×28 pixels (MNIST standard)
   - Normalize pixel values (0-1 range)
   - Invert colors if necessary

2. **Model Prediction**:
   - Feed preprocessed image to neural network
   - Get probability distribution for all digits (0-9)
   - Return highest probability as prediction

3. **Result Display**:
   - Show predicted digit with confidence score
   - Display probability chart for all digits
   - Highlight the predicted digit in the chart

## 📊 Performance Metrics

- **Training Accuracy**: ~99%
- **Test Accuracy**: ~98%
- **Inference Time**: <100ms per image
- **Model Size**: ~1.5MB

## 🛡️ Error Handling

- Automatic model training if saved model not found
- Image format validation
- Graceful error messages for invalid inputs
- Fallback mechanisms for processing failures

## 🔮 Future Enhancements

- [ ] Support for multiple digit recognition in single image
- [ ] Real-time drawing canvas for digit input
- [ ] Model performance comparison tools
- [ ] Export predictions to CSV/JSON
- [ ] Custom model training with user data
- [ ] Mobile-responsive design improvements
- [ ] API endpoint for programmatic access

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- **MNIST Dataset**: Yann LeCun, Corinna Cortes, and Christopher J.C. Burges
- **TensorFlow/Keras**: Google Brain Team
- **Streamlit**: Streamlit Inc.
- **OpenCV**: OpenCV Foundation

## 📞 Support

If you encounter any issues or have questions:

1. Check the [Issues](https://github.com/yourusername/handwritten-digit-recognition/issues) page
2. Create a new issue with detailed information
3. Contact the maintainer at your.email@example.com

## 📈 Stats

![GitHub stars](https://img.shields.io/github/stars/yourusername/handwritten-digit-recognition?style=social)
![GitHub forks](https://img.shields.io/github/forks/yourusername/handwritten-digit-recognition?style=social)
![GitHub issues](https://img.shields.io/github/issues/yourusername/handwritten-digit-recognition)
![GitHub license](https://img.shields.io/github/license/yourusername/handwritten-digit-recognition)

---

⭐ **Star this repository if you found it helpful!**
