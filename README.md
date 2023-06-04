# Tamil Handwriting Recognition Detection Model

Welcome to the Tamil Handwriting Recognition Detection Model repository! This project aims to detect handwritten letters of the Tamil language using deep learning neural networks powered by TensorFlow and AI. The model utilizes the Inception V3 architecture (`inception_v3`) for accurate and efficient recognition.

## Dataset

The training data for this project is sourced from the [Tamil Handwritten Character Recognition (IWFHR-06)](http://shiftleft.com/mirrors/www.hpl.hp.com/india/research/penhw-resources/tamil-iwfhr06-train.html) dataset. You can download the original images from the [HPL Tamil IWFHR-06 Train Offline Dataset](http://shiftleft.com/mirrors/www.hpl.hp.com/india/research/penhw-resources/hpl-tamil-iwfhr06-train-offline.tar.gz) link.

## Getting Started

To get started with the Tamil Handwriting Recognition Detection Model, ensure you have the necessary prerequisites installed and follow the provided steps.

### Prerequisites

- Anaconda: Install Anaconda for Python 3.5+ from the official website: [Anaconda Download](https://www.anaconda.com/download/)

### Create and Activate TensorFlow Environment

Follow the instructions provided by TensorFlow to create and activate the TensorFlow environment using Anaconda or the Command Prompt.

## Usage

Follow these steps to train and utilize the Tamil Handwriting Recognition Detection Model:

### Step 1: Clone the Project

Clone this project to your local machine and navigate to the project folder.

### Step 2: Extract Images

Unzip the `160x160.zip` file located in the `Training Data/Tamil/160x160/` folder. Remember to remove all the zip files from that folder. If you want to generate more images, you can also use the "Tamil Font to Handwriting Image" project.

### Step 3: Activate TensorFlow

Open the Command Prompt (`Start -> Run -> CMD`) and execute the following command to activate the TensorFlow environment:

```shell
C:> activate tensorflow
```

### Step 4: Training Your Data for 160x160 Image Size

Start training your AI by executing the following command:

```shell
(tensorflow)C:> python -m retrain --how_many_training_steps=6000
```

Increasing the number of training steps (`how_many_training_steps`) generally leads to better accuracy of the results.

### Step 5: Validate Your Own Handwritten Tamil Letter

Validate the model's performance by testing it with your own 160x160 image or by using a sample image from the `Test_Images/160` folder. Run the following command:

```shell
(tensorflow)C

:> python label_image.py --test_data_dir=Test_Images/160
```

## Key Benefits

- Accurate Handwriting Recognition: The model is trained using deep learning techniques, enabling accurate recognition of handwritten Tamil letters.
- Automation and Efficiency: By leveraging machine learning, the model reduces the need for manual input and computation, providing a more efficient way to process handwritten equations.
- Improved Accuracy and Productivity: The automated approach minimizes user errors associated with manual input, resulting in increased accuracy and productivity.
- Open-Source and Extensible: This project is open-source, allowing developers to contribute, enhance, and adapt the model for other languages or applications.

## Presentation

During our 2nd year, we prepared a comprehensive PowerPoint presentation on this project. You can find the presentation slides in the [presentation folder](./Presentation). Feel free to explore the slides to gain a deeper understanding of our Tamil Handwriting Recognition Detection Model.

We hope you find this project valuable and encourage you to contribute, provide feedback, or report any issues. Happy coding!
