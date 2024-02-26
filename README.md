# centerfusion
## Installation

The code has been tested on Ubuntu 16.04 and CentOS 7 with Python 3.7, CUDA 10.0 and PyTorch 1.2. For installation, follow these steps:

1. Create a new virtual environment (optional):
    ```bash
    mkvirtualenv centerfusion  
    ```

2. Install [PyTorch](https://pytorch.org/get-started/locally/):
    ```bash
    pip install torch torchvision
    ```

3. Install [COCOAPI](https://github.com/cocodataset/coco):
    ```bash
    pip install cython; pip install -U 'git+https://github.com/cocodataset/cocoapi.git#subdirectory=PythonAPI'
    ```

4. Clone the CenterFusion repository with the `--recursive
