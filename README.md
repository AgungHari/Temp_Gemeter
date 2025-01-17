[![banner4](banner4.png)](https://www.agungg.com/)

# Wheelchair Control System Using Invisible Steering Gesture Based on LSTM

![Scikit-learn version](https://img.shields.io/badge/scikitlearn-v1.5.1-black)
![Keras version](https://img.shields.io/badge/Keras-v3.5.0-purple)
![matplotlib version](https://img.shields.io/badge/matplotlib-v3.9.2-red)
![MediaPipe version](https://img.shields.io/badge/MediaPipe-v0.10.14-blue)
![Tensorflow version](https://img.shields.io/badge/Tensorflow-v2.10.1-orange)
![OpenCV version](https://img.shields.io/badge/OpenCV-v4.9.0.80-green)
![IPyKernel version](https://img.shields.io/badge/IPyKernel-v6.29.4-yellow)
![License](https://img.shields.io/badge/License-MIT-darkblue)

<img src="https://user-images.githubusercontent.com/74038190/212284100-561aa473-3905-4a80-b561-0d28506553ee.gif" width="900">

This is an original project by I Putu Krisna Erlangga, but it has been modified to control a wheelchair.

This project is still under development. It involves controlling the wheelchair with an invisible steering wheel, using hand gestures as if steering. The approach utilizes an LSTM model to send output to the wheelchair, corresponding to the five available classes.

## Project Result

[![mantap](https://github.com/user-attachments/assets/dad0701e-425c-4b3d-8604-a94cfa2fa1b4)](https://youtu.be/O69vtuBGGe4)

[![YouTube](https://img.shields.io/badge/YouTube-black?style=flat-square&logo=youtube)](https://youtu.be/O69vtuBGGe4)

## Installation

Please use seperate file for collecting dataset and training also use seperate folder for control. venv setup for training

```bash
  python --version
  python -m venv nama_venv
  nama_venv\Scripts\activate
  pip install opencv-python
  pip install mediapipe
  pip install numpy
  pip install matplotlib
  pip install tensorflow
  pip install seaborn
  pip install scikit-learn
```

Actually, you need an ESP32 and the wheelchair to run it.

```bash
  python --version
  python -m venv nama_venv
  nama_venv\Scripts\activate
  pip install mediapipe
  pip install opencv-python
```

## Collecting Dataset

change the dataset folder name and class for your setup. 

```bash
  DATA_PATH = os.path.join('p_ganti_ini_pake_namaDataset') #Change it with whatever you like

  actions = np.array(["Follow", "Github", "Agung", "Hari", "Bos"])
  no_sequences = 50 #set jumlah sequence
  sequence_length = 6 #Lama ngambil per sequence
```
run all cell on AMBIL_DATASET_AGUNG. it should open camera feed like this.

![ambildataset](https://github.com/user-attachments/assets/08da6c91-c6a7-4ab6-8016-f970053b7a83)

after you normalized the dataset you can start training the model

## Feedback

<img alt="Static Badge" src="https://img.shields.io/badge/krsx-black?style=social&logo=github&link=https%3A%2F%2Fgithub.com%2Fkrsx">
It is better to use a CNN-LSTM approach.


## Authors

<img alt="Static Badge" src="https://img.shields.io/badge/krsx-black?style=social&logo=github&link=https%3A%2F%2Fgithub.com%2Fkrsx">
<img alt="Static Badge" src="https://img.shields.io/badge/Naufal-black?style=social&logo=github&link=https%3A%2F%2Fgithub.com%2FKodokHamil">
<img alt="Static Badge" src="https://img.shields.io/badge/AgungHari-black?style=social&logo=github&link=https%3A%2F%2Fgithub.com%2FAgungHari">

## License

<img alt="GitHub License" src="https://img.shields.io/github/license/AgungHari/Wheelchair-Control-System-Using-Invisible-Steering-Gesture-Based-on-LSTM">

