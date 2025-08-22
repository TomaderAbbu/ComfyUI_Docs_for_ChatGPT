# SECTION: GETTING_STARTED


## ITEM:
```bash
# Launch ComfyUI
```


## ITEM:
```bash
python main.py
```


## ITEM:
If MPS causes issues:


## ITEM:
Copy


## ITEM:
Ask AI


## ITEM:
```bash
# Force CPU mode
```


## ITEM:
```bash
python main.py --cpu
```


## ITEM:
```bash
# With memory optimization
```


## ITEM:
```bash
python main.py --force-fp16 --cpu
```


## ITEM:
Intel GPU Issues


## ITEM:
Option 1: Native PyTorch XPU support (Windows/Linux):


## ITEM:
Copy


## ITEM:
Ask AI


## ITEM:
```bash
# Install PyTorch nightly with XPU support
```


## ITEM:
```bash
pip install --pre torch torchvision torchaudio --index-url https://download.pytorch.org/
whl/nightly/xpu
```


## ITEM:
```bash
# Launch ComfyUI
```


## ITEM:
```bash
python main.py
```


## ITEM:
Option 2: Intel Extension for PyTorch (IPEX):


## ITEM:
Copy


## ITEM:
Ask AI


## ITEM:
```bash
# For Intel Arc A-Series Graphics
```


## ITEM:
conda install libuv


## ITEM:
```bash
pip install torch==2.3.1.post0+cxx11.abi torchvision==0.18.1.post0+cxx11.abi
torchaudio==2.3.1.post0+cxx11.abi intel-extension-for-pytorch==2.3.110.post0+xpu --
```
extra-index-url https://pytorch-extension.intel.com/release-whl/stable/xpu/us/


## ITEM:
Getting Help & Reporting Bugs


## ITEM:
Before Reporting a Bug


## ITEM:
1. 	Check if it’s a known issue:


## ITEM:
• 	Search GitHub Issues


## ITEM:
• 	Check ComfyUI Forum


## ITEM:
• 	Review Discord discussions
