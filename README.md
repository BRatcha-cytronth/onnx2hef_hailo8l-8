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

## Prepare environment

```bash
sudo apt install -y \
  python3.10 \
  python3.10-venv \
  python3.10-dev
```
