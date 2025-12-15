# onnx2hef_hailo8l-8

## Overview

A set of Python scripts to **convert ONNX deep learning models into Hailo HEF format** for deployment on Hailo-8L and Hailo-8 accelerators. This project includes parsing, optimizing, and compiling steps for preparing models (e.g., from YOLO/Ultralytics) to Hailo deployable binaries.

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

<img width="1280" height="720" alt="image" src="https://github.com/user-attachments/assets/0d9ac7d8-12e6-4baf-8c3f-daa1b421cbf7" />

and

<img width="1280" height="720" alt="image" src="https://github.com/user-attachments/assets/5bc77190-f8fe-4b93-98ec-a7ad5f5048bc" />

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

build virtual environment
```bash
python3.10 -m venv ~/venv_hailo
source ~/venv_hailo/bin/activate
```

