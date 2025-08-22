# SECTION: INSTALLATION


## ITEM:
1. Launch ComfyUI
Make sure you’ve followed the installation guide to start ComfyUI and can
successfully enter the ComfyUI interface.


## ITEM:
If you have not installed ComfyUI, please choose a suitable version to install based
on your device.
ComfyUI Desktop
ComfyUI Desktop currently supports standalone installation for Windows and
MacOS (ARM), currently in Beta
•   Code is open source on Github
Because Desktop is always built based on the stable release, so the latest updates
may take some time to experience for Desktop, if you want to always experience the
latest version, please use the portable version or manual installation
You can choose the appropriate installation for your system and hardware below
•   Windows
•   MacOS(Apple Silicon)
•   Linux


## ITEM:
ComfyUI Desktop (Windows) Installation Guide
Suitable for Windows version with Nvidia GPU
ComfyUI Portable (Windows)
Portable version is a ComfyUI version that integrates an independent embedded
Python environment, using the portable version you can experience the latest
features, currently only supports Windows system
ComfyUI Portable (Windows) Installation Guide
Supports Windows ComfyUI version running on Nvidia GPUs or CPU-only, always
use the latest commits and completely portable.
Manual Installation
ComfyUI Manual Installation Guide
Supports all system types and GPU types (Nvidia, AMD, Intel, Apple Silicon, Ascend
NPU, Cambricon MLU)


## ITEM:
3. Model Installation
Most ComfyUI installations don’t include base models by default. After loading the
workflow, if you don’t have the v1-5-pruned-emaonly-fp16.safetensors model
installed, you’ll see this prompt:


## ITEM:
All models are stored in <your ComfyUI installation>/ComfyUI/models/ with
subfolders like checkpoints, embeddings, vae, lora, upscale_model, etc.
ComfyUI detects models in these folders and paths configured in
extra_model_paths.yaml at startup.


## ITEM:
If everything goes smoothly, the model should be able to download locally. If the
download fails for a long time, please try other installation methods.


## ITEM:
4. Load Model and Generate Your First Image
After installing the model:


## ITEM:
1. In the Load Checkpoint node, ensure v1-5-pruned-emaonly-fp16.safetensors is
selected
2. Click Queue or press Ctrl + Enter to generate
The result will appear in the Save Image node. Right-click to save locally.


## ITEM:
Model Loading Issues
If the Load Checkpoint node shows no models or displays “null”, verify your model
installation location and try refreshing or restarting ComfyUI.
_____________________________________
_____________________________________
_____________________________________
Get Started


## ITEM:
• 	Memory Management: Optimized installation size and memory eﬃciency


## ITEM:
Frontend Changes


## ITEM:
• 	Subgraph Support: Subgraph functionality support


## ITEM:
• 	Shortcut Panel: Added bottom shortcut panel


## ITEM:
• 	UI Layout Modifications: Modified terminal entry layout, added template, log
panel and other entries


## ITEM:
• 	CUDA Memory Management: Fixed CUDA malloc to only activate on CUDA-
enabled PyTorch installations


## ITEM:
Sampling Algorithm Improvements


## ITEM:
• 	Euler CFG++ Enhancement: Separated denoised and noise estimation
processes in Euler CFG++ sampler


## ITEM:
• 	Python Version Warnings: Added alerts for outdated Python installations


## ITEM:
• 	WebcamCapture Fixes: Corrected IS_CHANGED signature


## ITEM:
• 	Manual installation


## ITEM:
• 	Manual Installation


## ITEM:
So next we need to use ComfyUI’s independent Python runtime environment to
complete the dependency installation.


## ITEM:
• 	ComfyUI Portable


## ITEM:
• 	ComfyUI Desktop


## ITEM:
• 	Custom Python Environment Users


## ITEM:
For ComfyUI Portable version, it uses an embedded Python located in the
\ComfyUI_windows_portable\python_embeded directory. We need to use this Python
to complete the dependency installation.


## ITEM:
First, start the terminal in the portable version directory, or use the cd command to
navigate to the \ComfyUI_windows_portable\ directory after starting the terminal.


## ITEM:
Ensure that the terminal directory is \ComfyUI_windows_portable\, as shown below for
D:\ComfyUI_windows_portable\


## ITEM:
Then use python_embeded\python.exe to complete the dependency installation:


## ITEM:
Copy


## ITEM:
Ask AI


## ITEM:
In this section, we will still explain these two diﬀerent plugin version management
methods for you, but if you use ZIP packages for manual installation, the
corresponding git version history information will be lost, making it impossible to
perform version management.


## ITEM:
Switch to the corresponding version. Manager will help you complete the
corresponding dependency updates and installation. Usually, you need to restart
ComfyUI after switching versions for the changes to take eﬀect.


## ITEM:
This tool is currently included by default in the Desktop version, while in the Portable
version, you need to refer to the installation instructions in the Install Manager section
of this document.


## ITEM:
Model files are indispensable for generative media production.
Without them, workflows cannot proceed eﬀectively. Models are
not included in the ComfyUI installation, but ComfyUI can often
automatically download and install missing model files. Many
models can be downloaded and installed from the ComfyUI
Manager window. Models can also be found at websites such as
huggingface.co, civitai.green, and github.com.


## ITEM:
• 	 Portable/Manual Install


## ITEM:
• 	 ComfyUI Desktop


## ITEM:
For the ComfyUI version such as portable and manual, you can
find an example file named extra_model_paths.yaml.example in
the root directory of ComfyUI:


## ITEM:
Copy


## ITEM:
Ask AI


## ITEM:
ComfyUI/extra_model_paths.yaml.example


## ITEM:
Copy and rename it to extra_model_paths.yaml for use. Keep it in
ComfyUI’s root directory at ComfyUI/extra_model_paths.yaml.
You can also find the config example file here


## ITEM:
If the file does not exist, you can create it yourself with any text
editor.


## ITEM:
Example Structure


## ITEM:
Suppose you want to add the following model paths to ComfyUI:


## ITEM:
Copy


## ITEM:
Ask AI


## ITEM:
📁  YOUR_PATH/


## ITEM:
For the desktop version, please add the configuration to the existing
configuration path without overwriting the path configuration generated
during installation. Please back up the corresponding file before
modification, so that you can restore it when you make a mistake.


## ITEM:
Or you can refer to the default extra_model_paths.yaml.example
for more configuration options. After saving, you need to restart
ComfyUI for the changes to take eﬀect.


## ITEM:
Below is the original config example:


## ITEM:
Copy


## ITEM:
Ask AI


## ITEM:
#Rename this to extra_model_paths.yaml and ComfyUI will load it


## ITEM:
#config for a1111 ui


## ITEM:
#all you have to do is change the base_path to where yours is installed


## ITEM:
a111:


## ITEM:
base_path: path/to/stable-diﬀusion-webui/


## ITEM:
If you’re using the Windows Portable version, you can use the following command in
the ComfyUI_windows_portable directory:


## ITEM:
Copy


## ITEM:
Ask AI


## ITEM:
• Try installing plugins one by one, restarting ComfyUI after each installation to
observe if dependency conflicts occur.


## ITEM:
1. Do not use any third-party nodes (to avoid extra installations for users who lack
those nodes).


## ITEM:
2. The template must not duplicate existing ones and should target supported
model capabilities.


## ITEM:
3. You may open an issue in the repository to ask questions.


## ITEM:
The ComfyUI user directory is where your personal settings, workflows, and
customizations are stored. The location depends on your installation type:


## ITEM:
• 	Desktop - Windows


## ITEM:
• 	Desktop - macOS


## ITEM:
• 	Desktop - Linux


## ITEM:
• 	Manual Install


## ITEM:
• 	Portable


## ITEM:
Copy


## ITEM:
Ask AI


## ITEM:
C:\Users\<your username>\AppData\Roaming\ComfyUI\user


## ITEM:
• 	Managed Python installation packages are downloaded from the Astral python-
build-standalone project


## ITEM:
• 	Can set mirror URL to use diﬀerent Python installation sources


## ITEM:
• 	The provided URL will replace the default GitHub download address


## ITEM:
• 	Supports using file:// protocol to read distribution packages from local
directories


## ITEM:
Validation: Automatically checks mirror reachability


## ITEM:
Pypi Install Mirror


## ITEM:
Function: Default pip package installation mirror source


## ITEM:
Torch Install Mirror


## ITEM:
Function: PyTorch-specific pip installation mirror source


## ITEM:
Installation-Specific Issues


## ITEM:
Desktop App Issues


## ITEM:
• 	Unsupported device: ComfyUI Desktop Windows only supports NVIDIA GPUs
with CUDA. Use ComfyUI Portable or manual installation for other GPUs


## ITEM:
• 	Installation fails: Run installer as administrator, ensure at least 15GB disk space


## ITEM:
• 	Maintenance page: Check mirror settings if downloads fail


## ITEM:
Manual Installation Issues


## ITEM:
The documentation may be slightly out of date. If an issue occurs, please manually
verify whether a newer stable version of pytorch or any of the listed libraries exists.
Refer to resources like the pytorch installation matrix or the ROCm website.


## ITEM:
Python version conflicts:


## ITEM:
Copy


## ITEM:
Ask AI


## ITEM:
```bash
# Check Python version (3.9+ required, 3.12 recommended)
```


## ITEM:
```bash
python --version
```


## ITEM:
```bash
# Use virtual environment (recommended)
```


## ITEM:
```bash
python -m venv comfyui_env
```


## ITEM:
source comfyui_env/bin/activate  # Linux/Mac


## ITEM:
comfyui_env\Scripts\activate     # Windows


## ITEM:
Package installation failures:


## ITEM:
Copy


## ITEM:
Ask AI


## ITEM:
```bash
# Update pip first
```


## ITEM:
```bash
python -m pip install --upgrade pip
```


## ITEM:
1. Modern PyTorch installations (most common):


## ITEM:
Copy


## ITEM:
Ask AI


## ITEM:
```bash
# For virtual environments with NVIDIA packages
```


## ITEM:
export LD_LIBRARY_PATH=$VIRTUAL_ENV/lib/python3.12/site-packages/nvidia/
nvjitlink/lib:$LD_LIBRARY_PATH


## ITEM:
```bash
# For conda environments
```


## ITEM:
export LD_LIBRARY_PATH=$CONDA_PREFIX/lib/python3.12/site-packages/nvidia/
nvjitlink/lib:$LD_LIBRARY_PATH


## ITEM:
```bash
# Or find your Python site-packages automatically
```


## ITEM:
PYTHON_PATH=$(python -c "import site; print(site.getsitepackages()[0])")


## ITEM:
export LD_LIBRARY_PATH=$PYTHON_PATH/nvidia/nvjitlink/lib:$LD_LIBRARY_PATH


## ITEM:
```bash
# You may also need other NVIDIA libraries
```


## ITEM:
export LD_LIBRARY_PATH=$PYTHON_PATH/nvidia/cuda_runtime/lib:
$LD_LIBRARY_PATH


## ITEM:
export LD_LIBRARY_PATH=$PYTHON_PATH/nvidia/cublas/lib:$LD_LIBRARY_PATH


## ITEM:
2. Find what libraries you have:


## ITEM:
Copy


## ITEM:
Ask AI


## ITEM:
```bash
# Check installed NVIDIA packages
```


## ITEM:
```bash
python -c "import site; import os; nvidia_path=os.path.join(site.getsitepackages()[0],
'nvidia'); print('NVIDIA libs:', [d for d in os.listdir(nvidia_path) if
```
os.path.isdir(os.path.join(nvidia_path, d))] if os.path.exists(nvidia_path) else 'Not
found')"


## ITEM:
```bash
# Find missing libraries that PyTorch needs
```


## ITEM:
```bash
python -c "import torch; print(torch.__file__)"
```


## ITEM:
ldd $(python -c "import torch; print(torch.__file__.replace('__init__.py', 'lib/
libtorch_cuda.so'))")


## ITEM:
3. Set permanently for your environment:


## ITEM:
Copy


## ITEM:
Ask AI


## ITEM:
```bash
# For virtual environments, add to activation script
```


## ITEM:
echo 'export LD_LIBRARY_PATH=$VIRTUAL_ENV/lib/python*/site-packages/nvidia/
nvjitlink/lib:$LD_LIBRARY_PATH' >> $VIRTUAL_ENV/bin/activate


## ITEM:
```bash
# For conda environments
```


## ITEM:
conda env config vars set LD_LIBRARY_PATH=$CONDA_PREFIX/lib/python*/site-
packages/nvidia/nvjitlink/lib:$LD_LIBRARY_PATH


## ITEM:
```bash
# For global bashrc (adjust Python version as needed)
```


## ITEM:
echo 'export LD_LIBRARY_PATH=$(python -c "import site; print(site.getsitepackages()
[0])")/nvidia/nvjitlink/lib:$LD_LIBRARY_PATH' >> ~/.bashrc


## ITEM:
4. Alternative: Use ldconfig:


## ITEM:
Copy


## ITEM:
Ask AI


## ITEM:
```bash
# Check current library cache
```


## ITEM:
ldconfig -p | grep cuda


## ITEM:
ldconfig -p | grep nccl


## ITEM:
```bash
# If missing, add library paths (requires root)
```


## ITEM:
sudo echo "/usr/local/cuda/lib64" > /etc/ld.so.conf.d/cuda.conf


## ITEM:
sudo ldconfig


## ITEM:
5. Debug library loading:


## ITEM:
Copy


## ITEM:
Ask AI


## ITEM:
```bash
# Verbose library loading to see what's missing
```


## ITEM:
LD_DEBUG=libs python main.py 2>&1 | grep "looking for"


## ITEM:
```bash
# Check PyTorch CUDA availability
```


## ITEM:
```bash
python -c "import torch; print('CUDA available:', torch.cuda.is_available()); print('CUDA
version:', torch.version.cuda)"
```


## ITEM:
Model-Related Issues


## ITEM:
• 	Installation method (Desktop, Portable, Manual, comfy-cli)


## ITEM:
2


## ITEM:
Desktop App issues


## ITEM:
For Desktop App issues, also include:


## ITEM:
• 	Log files from: C:\Users\<username>\AppData\Roaming\ComfyUI\logs
(Windows)


## ITEM:
• 	Config files from: C:\Users\<username>\AppData\Roaming\ComfyUI (Windows)


## ITEM:
3


## ITEM:
Problem Details


## ITEM:
Problem Details:


## ITEM:
• Clear description of the issue


## ITEM:
• Steps to reproduce the problem


## ITEM:
• Expected vs actual behavior


## ITEM:
• Screenshots or videos if applicable


## ITEM:
Error Messages:


## ITEM:
• Full error text from console/terminal


## ITEM:
• Browser console errors (F12 → Console tab)


## ITEM:
• Any crash logs or error dialogs


## ITEM:
4


## ITEM:
Additional Context


## ITEM:
Additional Context:


## ITEM:
• Recent changes (new installations, updates, etc.)


## ITEM:
Community Resources


## ITEM:
• 	Oﬃcial Forum: forum.comfy.org


## ITEM:
• 	Discord: ComfyUI Discord Server


## ITEM:
• 	Reddit: r/comfyui
