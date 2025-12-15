# onnx2hef_hailo8l-8

## Overview

A set of Python scripts to **convert ONNX deep learning models into Hailo HEF format** for deployment on Hailo-8L and Hailo-8 accelerators. This project includes parsing, optimizing, and compiling steps for preparing models **YOLOv8** to Hailo deployable binaries.

Hailo’s HEF format enables efficient inference on Hailo-8L and Hailo-8 hardware. 

---


## Prepare WSL2 (Ubuntu 22.04)

on command promt or powershell
```bash
wsl --install -d Ubuntu-22.04
```
## Get file from Hailo
** Please register then download **

https://hailo.ai/developer-zone/software-downloads/?product=ai_accelerators&device=hailo_8_8l

1. Dataflow Complier

<img width="1280" height="720" alt="image" src="https://github.com/user-attachments/assets/0d9ac7d8-12e6-4baf-8c3f-daa1b421cbf7" />

2. Model Zoo

<img width="1280" height="720" alt="image" src="https://github.com/user-attachments/assets/5bc77190-f8fe-4b93-98ec-a7ad5f5048bc" />

move to wsl user path

## Prepare environment

```bash
sudo apt install -y \
  python3.10 \
  python3.10-venv \
  python3.10-dev
```
check
```bash
python3 --version
```
suppose to be python 3.10.xx

clone this 
```bash
git clone https://github.com/BRatcha-cytronth/onnx2hef_hailo8l-8.git
```

build virtual environment
```bash
python3.10 -m venv ~/venv_hailo
source ~/venv_hailo/bin/activate
```
install essential libraries
```bash
sudo apt-get update
sudo apt-get install build-essential python3-dev graphviz graphviz-dev python3-tk
pip install -r requirements.txt
```
```bash
pip install hailo_dataflow_compiler-3.33.0-py3-none-linux_x86_64.whl
pip install hailo_model_zoo-2.17.1-py3-none-any.whl
```
```bash
git clone https://github.com/hailo-ai/hailo_model_zoo.git
```

