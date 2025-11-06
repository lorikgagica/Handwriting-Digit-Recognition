# ✍️ Handwriting Digit Recognition (MNIST CNN)

This project is a complete, easy-to-copy solution for handwritten digit recognition using a Convolutional Neural Network (CNN) in TensorFlow/Keras. Input: MNIST dataset. Output: Super-quick, high-accuracy digit classification — with a visual demonstration!

---

## 🚀 Features

- **Trains a CNN on the MNIST dataset** (28x28 grayscale images of digits 0–9)
- **Normalization for better neural network performance**
- **Model architecture:** 2 Conv2D layers, 2 MaxPooling2D layers, dense hidden layer, and softmax output
- **Prints test accuracy**
- **Predicts and displays a single test-digit with the predicted label**
- **Commented, readable, and easy to extend**

---

## 🛠 Requirements

- Python 3.x
- TensorFlow (`tensorflow`)
- NumPy (`numpy`)
- Matplotlib (`matplotlib`)
`pip install tensorflow numpy matplotlib`

---

## 💾 How to Run

1. Save `write.py` to your project directory.
2. Run:`python write.py`
3. The script will:
 - Download MNIST if not cached
 - Train for 1 epoch (change `epochs=1` for more accuracy)
 - Report test accuracy
 - Display prediction for a test image (index 0 by default)

---

## 🧑‍💻 What the Script Does

1. **Loads MNIST data**
2. **Normalizes images** to [0, 1] range
3. **Reshapes data** for CNN: adds the channel dimension (28,28,1)
4. **Builds a CNN:**  
 - Input layer (28x28x1)
 - Conv2D(32) → MaxPool(2)
 - Conv2D(64) → MaxPool(2)
 - Flatten → Dense(128) → Dense(10, softmax)
5. **Compiles with Adam/categorical crossentropy**
6. **Trains with validation**
7. **Evaluates and prints test accuracy**
8. **Predicts a digit and shows the test image with predicted label**

---

## 📊 Example Output

Train on 60000 samples, validate on 10000 samples
...
Test Accuracy: 98.23%
[matplotlib popup showing a digit and "Predicted Digit: 3"]

---

## ⚡️ Customization & Tips

- Increase `epochs` for better accuracy (>98.5% typical for 5+ epochs)
- Change `index = ...` to visualize other test digits
- Use `model.summary()` (uncommented) for detailed model stats
- Add saving/loading with `model.save("my_model.h5")` if desired
- Support your own data by adjusting the input shape and normalization

---

## 📄 License

MIT — free to use, adapt, and distribute.

---

### 🎯 A perfect starting point for neural net projects, machine learning courses, or AI hackathons.
