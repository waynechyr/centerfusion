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

4. Clone the CenterFusion repository with the `--recursive ` option. We'll call the directory that you cloned CenterFusion into `CF_ROOT`:
    ```bash
    CF_ROOT=/path/to/CenterFusion
    git clone --recursive https://github.com/mrnabati/CenterFusion.git $CF_ROOT
    ```

5. Install the requirements:
   ```bash
   cd $CF_ROOT
   pip install -r requirements.txt
   ```

6. Build the deformable convolution library:
    ```bash
    cd $CF_ROOT/src/lib/model/networks/DCNv2
    ./make.sh
    ```
