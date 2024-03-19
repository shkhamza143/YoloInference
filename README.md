# Yolo Inference
This Project Includes MFC C++ based inference for Yolov5.

# Prerequiests
Visual Studio 2022 | Python3.8 | Anaconda

1. Install VS2022 with MFC C++ build tools
2. Download and install [Python3.8](https://www.python.org/downloads/)
3. Download and install [Anaconda](https://www.anaconda.com/download) (Optional)
4. Download all required wheel packages from [drive]() and paste them in YoloInference/dependencies/wheels
5. Download and extract [boost 1.83.0](https://www.boost.org/users/history/version_1_83_0.html) in YoloInference/dependencies/libs/boost_1_83_0

# Installation
1. **Python Installation:**
   - create anaconda virtual envirenmont and activate it using:
   ```
   conda create --name yolo python=3.8
   conda activate yolo
   ```
   - Install required packages using:
   ```
   cd YoloInference/dependencies/wheels
   pip install "Cython-3.0.9-cp38-cp38-win_amd64.whl"
   pip install "matplotlib-3.2.2-cp38-cp38-win_amd64.whl"
   pip install "numpy-1.22.4-cp38-cp38-win_amd64.whl"
   pip install "opencv_python-4.5.1.48-cp38-cp38-win_amd64.whl"
   pip install "pandas-1.3.5-cp38-cp38-win_amd64.whl"
   pip install "Pillow-9.1.1-cp38-cp38-win_amd64.whl"
   pip install "psutil-5.9.0-cp38-cp38-win_amd64.whl"
   pip install "PyYAML-6.0-cp38-cp38-win_amd64.whl"

   # For CPU
   pip install "torch-1.8.0+cpu-cp38-cp38-win_amd64.whl"
   pip install "torchaudio-0.8.0-cp38-none-win_amd64.whl"
   pip install "torchvision-0.9.0+cpu-cp38-cp38-win_amd64.whl"

   # For GPU

   pip install -r requirements.txt
   ```

2. **Boost Installation**
   - Open cmd.
   ```
   cd YoloInference/dependencies/libs/boost_1_83_0
   bootstrap.bat
   b2 --toolset=msvc address-model=64
   ```

   
