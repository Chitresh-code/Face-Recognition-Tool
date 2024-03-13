# Face Recognition Tool
> Powerful tool that offers accurate and efficient face detection and recognition capabilities.

## Table of Contents

- [About](#about)
- [Features](#features)
- [Demo](#demo)
- [Getting Started](#getting-started)
- [Contributing](#contributing)
- [License](#license)

## About

This Face Recognition Tool is a powerful application designed to detect and recognize faces within images. Leveraging state-of-the-art machine learning algorithms, it offers accurate and efficient face detection and recognition capabilities.
Whether you're building a security system, enhancing photo management applications, or exploring the possibilities of computer vision, the Face Recognition Tool offers a robust solution for detecting and recognizing faces in images.

## Features

- **User-Friendly Interface:** The tool provides an intuitive user interface, making it easy for users to upload images, perform face detection and recognition tasks, and visualize the results.

- **Customizable:** Users have the flexibility to customize various parameters and settings according to their specific requirements, allowing for fine-tuning of the face detection and recognition process.

- **Scalable:** The tool is designed to handle large datasets of images efficiently, making it suitable for both small-scale and enterprise-level applications.

- **Open Source:** This project is open source, encouraging collaboration and contribution from the community. Developers can extend the functionality of the tool and adapt it to their own projects and use cases.

## Demo
- Input Image
![Input Image](https://github.com/Chitresh-code/Face-Recognition-Tool/blob/main/eval_img/test_img.jpg)
- Output Image
![Output Image](https://github.com/Chitresh-code/Face-Recognition-Tool/blob/main/output/output_image.jpg)


## Getting Started

To get started with the Face Recognition Tool locally, follow these steps:

1. Clone the repository:

   ```bash
   https://github.com/Chitresh-code/GDSC-GNIOT-Completion-Tracker.git

2. Get your training and testing data or use the data in the [sample_data]() folder
3. Create your project directories
	  ```bash
	PS> mkdir face_recognizer
	PS> cd face_recognizer
	PS> mkdir output
	PS> mkdir training
	PS> mkdir validation
	```
	Your data should look like this:
	```
	face_recognizer/
	│
	├── output/
	│
	├── training/
	│   └── ben_affleck/
	│       ├── img_1.jpg
	│       └── img_2.png
	│
	├── validation/
	│   ├── ben_affleck1.jpg
	│   └── michael_jordan1.jpg
	│
	├── detector.py
	├── requirements.txt
	└── unknown.jpg

4. Create your virtual environment: 
	```bash
	PS> python -m venv venv
	PS> venv\Scripts\activate
	(venv) PS>
	#To deactivate it use
	(venv) PS> deactivate
	PS>
5. Before you start installing this project’s dependencies with `pip`, you’ll need to ensure that you have [CMake](https://cmake.org/) and a C compiler like [gcc](https://gcc.gnu.org/) installed on your system.
6. Now open your favorite text editor to create your `requirements.txt` file:
	 ```bash
	 dlib==19.24.0
	face-recognition==1.3.0
	numpy==1.24.2
	Pillow==9.4.0
7. After creating the requirements file and activating your virtual environment, you can install all of your dependencies at once:
	```bash
	python -m pip install -r requirements.txt
8. Now you can run the code using CLI you can check the commands using:
	```bash
	(venv) PS> python detector.py --help
9. To train the model use:
	 ```bash
	 python detector.py --train -m=hog
	 ```
	 or
	 ```bash
	 python detector.py --train -m=cnn
	 ```
10. To validate the model use:
	```bash
	python detector.py --validate
11. To test the model use: 
	```bash
	python detector.py --test -f image_path

Your readme looks great so far! Here's the continuation with the contributing guidelines and license section:


## Contributing

Contributions are welcome! Please follow these steps to contribute to the Face Recognition Tool:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature/fooBar`).
3. Make your changes.
4. Commit your changes (`git commit -am 'Add some fooBar'`).
5. Push to the branch (`git push origin feature/fooBar`).
6. Create a new Pull Request.

Please ensure that your contributions adhere to the coding standards and practices of the project.

## License

This project is licensed under the MIT License. See the [LICENSE](https://github.com/Chitresh-code/Face-Recognition-Tool/blob/main/LICENSE) file for details.

