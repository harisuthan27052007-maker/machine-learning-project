# Computer Vision & Deep Learning Roadmap

A structured collection of Computer Vision and Deep Learning projects, ranging from foundational Convolutional Neural Networks (CNNs) to real-time object detection and Generative Adversarial Networks (GANs)[cite: 2, 7].

---

## 📂 Repository Contents

* **`cats_vs_dogs_challenge.py`**: A binary image classification Convolutional Neural Network built with Keras (`Sequential`, `Conv2D`, `MaxPooling2D`) using `ImageDataGenerator` for data augmentation (shearing, zooming, horizontal flipping) to classify images of cats and dogs[cite: 3].
* **`MNIST_Convnet.py`**: A multi-class image classification CNN built with Keras trained on the MNIST handwritten digits dataset (`28x28` grayscale images across 10 classes)[cite: 5].
* **`Face Recognition/`**: Real-time face and eye detection using OpenCV and Haar Cascade classifiers (`haarcascade_frontalface_default.xml`, `haarcascade_eye.xml`)[cite: 2, 7].
* **`Object Detection/`**: Real-time object detection in video streams utilizing Single Shot MultiBox Detector (SSD)[cite: 2, 7].
* **`GANs/`**: Generative Adversarial Network implementation trained on the CIFAR dataset to generate synthetic images[cite: 2, 6, 7].

---

## 🛠️ Environment Setup (Anaconda)

1. Download and install [Anaconda](https://anaconda.org)[cite: 7].
2. Download the environment configuration files from the `Face Recognition/Installations` folder[cite: 7].
3. Open your Terminal (macOS/Linux) or Anaconda Prompt (Windows), navigate to the folder containing the `.yml` files, and create the Conda environment[cite: 7]:
   * **macOS:**
     ```bash
     conda env create -f virtual_platform_mac.yml
     ```
   * **Windows:**
     ```bash
     conda env create -f virtual_platform_windows.yml
     ```
   * **Linux:**
     ```bash
     conda env create -f virtual_platform_linux.yml
     ```
4. Activate the `Virtual_Platform` environment via Anaconda Navigator or terminal[cite: 7].

---

## 🚀 Usage Instructions

### 1. Cats vs. Dogs Classifier (`cats_vs_dogs_challenge.py`)
* Organize your dataset into `training_set` and `test_set` directories[cite: 3].
* Update `training_data_path`, `test_data_path`, and the single prediction image path (`cat_or_dog_1.jpg`) in the script[cite: 3].
* Run the script to train the 2-layer CNN (`64x64x3` input) over 25 epochs and run inference[cite: 3].

### 2. MNIST Digit Recognition (`MNIST_Convnet.py`)
* Run the script directly; Keras automatically downloads the MNIST dataset, normalizes pixel values, and trains a 3-layer CNN (`28x28x1` input) for 5 epochs[cite: 5].

### 3. Face & Eye Detection (`Face Recognition/`)
* Download `haarcascade_eye.xml` and `haarcascade_frontalface_default.xml`[cite: 7].
* Update the XML file paths inside `face_detection.py` and run the script[cite: 7].

### 4. Object Detection (`Object Detection/`)
* Upload the files from the `Object Detection` directory to Jupyter Notebook and run all cells sequentially to generate the annotated output video[cite: 7].

### 5. Generative Adversarial Networks (`GANs/`)
* Download the CIFAR dataset from the [official source](http://www.cs.toronto.edu/~kriz/cifar.html)[cite: 6, 7].
* Save the extracted dataset into a folder named `data_for_gan` in your Jupyter working directory before running the notebook[cite: 7].

---

## 📊 Sample Results

| Task | Preview / Output |
| :--- | :--- |
| **Face & Eye Detection** | ![Face Detection](https://github.com/manvimadan12/Computer_Vision_Roadmap/blob/main/Face%20Recognition/Results/Screen%20Shot%201.png) ![Face and Eyes Detection](https://github.com/manvimadan12/Computer_Vision_Roadmap/blob/main/Face%20Recognition/Results/Screen%20Shot%202.png)[cite: 7] |
| **Real-Time Object Detection** | ![Object Detection](https://github.com/manvimadan12/Computer_Vision_Roadmap/blob/main/Object%20Detection/Output/Object_detection_output_snip.png) • [Watch Output Video](https://github.com/manvimadan12/Computer_Vision_Roadmap/blob/main/Object%20Detection/Output/output.mp4)[cite: 7] |
| **GAN Image Generation** | ![GAN Output](https://github.com/manvimadan12/Computer_Vision_Roadmap/blob/main/GANs/results/fake_samples_epoch_024.png)[cite: 7] |

---

## 📚 References & Further Reading

* **Books:** [Deep Learning with Python](https://www.manning.com/books/deep-learning-with-python) • [Deep Learning (Goodfellow, Bengio, Courville)](https://www.deeplearningbook.org)[cite: 7]
* **Courses:** [Deep Learning and Computer Vision A-Z](https://www.udemy.com/course/computer-vision-a-z/)[cite: 7]
* **Papers:** [Viola-Jones Face Detection](https://github.com/manvimadan12/ML-Research-Papers-/blob/master/Computer%20Vision/Rapid%20Object%20Detection.pdf) • [Single Shot MultiBox Detector (SSD)](https://github.com/manvimadan12/ML-Research-Papers-/blob/master/Computer%20Vision/1512.02325.pdf) • [Generative Adversarial Networks (GANs)](
