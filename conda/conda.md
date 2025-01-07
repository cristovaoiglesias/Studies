	
	


this video explain how to install cuda 12.1 and tensorflow and pytorch
https://www.youtube.com/watch?v=1Tr1ifuSh6o&t=432s



     conda create --name tf_gpu python=3.10
     conda activate tf_gpu

    # https://www.tensorflow.org/install/pip
     python3 -m pip install tensorflow[and-cuda]
     python3 -c "import tensorflow as tf; print(tf.config.list_physical_devices('GPU'))"

    # https://pytorch.org/get-started/locally/
     pip3 install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu121



cuda12.1: https://developer.nvidia.com/cuda-12-1-1-download-archive?target_os=Linux&target_arch=x86_64&Distribution=Ubuntu&target_version=22.04&target_type=runfile_local

cuDNN Archive: https://developer.nvidia.com/rdp/cudnn-archive
NVIDIA TensorRT 8.x Download: https://developer.nvidia.com/nvidia-tensorrt-8x-download

https://repo.anaconda.com/miniconda/Miniconda3-py310_24.4.0-0-Linux-x86_64.sh

https://pytorch.org/get-started/locally/
https://www.tensorflow.org/install/pip
https://jupyter.org/install







# Environment Management

# Create a new environment
conda create --name myenv python=3.9

# Activate an environment
conda activate myenv

# Deactivate the current environment
conda deactivate

# List all environments
conda env list

# Clone an environment
conda create --name new_env --clone myenv

# Remove an environment
conda remove --name myenv --all

# Export an environment to a file
conda env export > environment.yml

# Create an environment from a file
conda env create -f environment.yml


# Package Management

# Install a package in the current environment
conda install numpy

# Install a package in a specific environment
conda install --name myenv pandas

# Remove a package from the current environment
conda remove numpy

# Update a specific package
conda update pandas

# Update all packages in the current environment
conda update --all

# List installed packages in the active environment
conda list

# Search for a package in the Conda repository
conda search matplotli



