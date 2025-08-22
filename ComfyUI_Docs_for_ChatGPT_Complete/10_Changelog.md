# SECTION: CHANGELOG


## ITEM:
Changelog


## ITEM:
Track ComfyUI’s latest features, improvements, and bug fixes


## ITEM:
v0.3.51


## ITEM:
August 20, 2025


## ITEM:
Model Support


## ITEM:
• 	Qwen-Image-Edit Model: Native support for Qwen-Image-Edit


## ITEM:
v0.3.50


## ITEM:
August 13, 2025


## ITEM:
Model Integration & Performance Enhancements


## ITEM:
v0.3.49


## ITEM:
August 5, 2025


## ITEM:
UI Experience & Model Support


## ITEM:
v0.3.48


## ITEM:
August 2, 2025


## ITEM:
API Enhancement & Performance Optimizations


## ITEM:
• 	ComfyAPI Core v0.0.2: Update to the core API framework, providing improved
stability and extensibility


## ITEM:
v0.3.47


## ITEM:
July 30, 2025


## ITEM:
Memory Optimization & Large Model Performance


## ITEM:
v0.3.46


## ITEM:
July 28, 2025


## ITEM:
Hardware Acceleration & Audio Processing


## ITEM:
This release expands hardware support and enhances audio processing capabilities:


## ITEM:
Audio Processing Enhancements


## ITEM:
v0.3.45


## ITEM:
July 21, 2025


## ITEM:
Sampling & Training Improvements


## ITEM:
This release introduces enhancements to sampling algorithms, training capabilities,
and node functionality:


## ITEM:
Sampling & Generation Features


## ITEM:
• 	SA-Solver Sampler: New reconstructed SA-Solver sampling algorithm providing
enhanced numerical stability


## ITEM:
• 	Experimental CFGNorm Node: Classifier-free guidance normalization for
improved control over generation quality


## ITEM:
• 	Nested Dual CFG Support: Added nested style configuration to DualCFGGuider
node


## ITEM:
• 	SamplingPercentToSigma Node: New utility node for precise sigma calculation
from sampling percentages


## ITEM:
Training Capabilities


## ITEM:
• 	Multi Image-Caption Dataset Support: LoRA training node now handles multiple
image-caption datasets simultaneously


## ITEM:
• 	Training Loop Implementation: Optimized training algorithms for improved
convergence and stability


## ITEM:
• 	Error Detection: Added model detection error hints for LoRA operations


## ITEM:
Platform & Performance Improvements


## ITEM:
• 	Async Node Support: Full support for asynchronous node functions with earlier
execution optimization


## ITEM:
• 	Chroma Flexibility: Un-hardcoded patch_size parameter in Chroma


## ITEM:
• 	LTXV VAE Decoder: Switched to improved default padding mode for better
image quality


## ITEM:
• 	Safetensors Memory Management: Added workaround for mmap issues


## ITEM:
API & Integration Enhancements


## ITEM:
v0.3.44


## ITEM:
July 8, 2025


## ITEM:
Sampling & Model Control Enhancements


## ITEM:
This release delivers improvements to sampling algorithms and model control systems:


## ITEM:
Sampling Capabilities


## ITEM:
• 	TCFG Node: Enhanced classifier-free guidance control for more nuanced
generation control


## ITEM:
• 	ER-SDE Sampler: Migrated from VE to VP algorithm with new sampler node


## ITEM:
• 	Skip Layer Guidance (SLG): Implementation for precise layer-level control during
inference


## ITEM:
Development Tools


## ITEM:
v0.3.43


## ITEM:
June 30, 2025


## ITEM:
v0.3.41


## ITEM:
June 17, 2025


## ITEM:
Model Support Additions


## ITEM:
v0.3.40


## ITEM:
June 5, 2025


## ITEM:
• 	Frontend Updated to v1.21.7: Stability fixes and performance improvements


## ITEM:
• 	Custom API Base Support: Better subpath handling for custom deployment
configurations


## ITEM:
• 	Security Hardening: XSS vulnerability fixes


## ITEM:
Bug Fixes & Stability


## ITEM:
• 	Pillow Compatibility: Updated deprecated API calls


## ITEM:
• 	ROCm Support: Improved version detection for AMD GPU users


## ITEM:
After frontend version v1.16.0, we improved this feature. Now you only need to directly
connect the input line to the corresponding widget to complete this process


## ITEM:
Chenlei Hu


## ITEM:
@HclHno3


## ITEM:
·


## ITEM:
Follow


## ITEM:
Say goodbye to annoying widget <> socket conversion starting from frontend version
v1.16.0! Now each widget just always have an associated input socket by default
#ComfyUI


## ITEM:
9:42 PM · Apr 6, 2025


## ITEM:
235


## ITEM:
Reply


## ITEM:
Copy link


## ITEM:
Input/Output Context Menu


## ITEM:
This context menu is mainly related to the data type of the corresponding input/output:


## ITEM:
Q: Why do all nodes run when I use this feature? A: Please
ensure your ComfyUI frontend version is after v1.23.4, or
possibly requires v1.24.x version. The corresponding bug was
fixed around version 1.24.x, so please update your ComfyUI to
the latest version to ensure the frontend version meets the
requirements.


## ITEM:
You may need to use at least ComfyUI v0.3.0 to use the account system. Ensure that
the corresponding frontend version is at least 1.17.11. Sometimes the frontend may fail
to install and revert to an older version, so please check if the frontend version is
greater than 1.17.11 in Settings -> About.


## ITEM:
In some regions, network restrictions may prevent normal access to the login API,
causing timeouts or failures. Before logging in, please ensure that your network
environment does not restrict access to the corresponding API, and make sure you can
access sites like Google or Github.


## ITEM:
Since we are still in rapid iterative updates, related functions may change. If there are
no special circumstances, please try to update to the latest version to get support for
relevant functions.


## ITEM:
Network Requirements


## ITEM:
To login to ComfyUI account, you must be in a secure network environment:


## ITEM:
• 	Only allow access from 127.0.0.1 or localhost.


## ITEM:
• 	Do not support using the --listen parameter to access the API node through a
local network.


## ITEM:
• 	If you are using a non-SSL certificate or a site that does not start with https, you
may not be able to successfully log in.


## ITEM:
• 	You may not be able to log in on a site that is not in our whitelist (but you can log
in using an API Key now).


## ITEM:
• 	Ensure you can connect to our service normally (some regions may require a
proxy).


## ITEM:
How to Log In


## ITEM:
Log in via Settings -> User:


## ITEM:
Login Methods


## ITEM:
If this is your first login, please create an account first.


## ITEM:
Logging in with an API Key


## ITEM:
Since not all ComfyUI deployments are on our domain authorization whitelist, we have
provided API Key login in a recent update (2025-05-10) for logging in through non-
whitelisted sites. Below are the steps for logging in with an API Key:


## ITEM:
• 	Have an API Key


## ITEM:
• 	No API Key, Apply for an API Key First


## ITEM:
1


## ITEM:
Select Comfy API Key Login on the Login Screen


## ITEM:
Select Comfy API Key login in the login popup


## ITEM:
2


## ITEM:
Enter Your API Key


## ITEM:
1. Enter your API Key and save it


## ITEM:
2. If you don’t have an API Key, click the Get one here link to go to https://
platform.comfy.org/login and log in to obtain it.


## ITEM:
3


## ITEM:
Login Successful


## ITEM:
After a successful login, you can see the corresponding API Key login information in
the settings menu


## ITEM:
Post-Login Status


## ITEM:
After logging in, a login button is displayed in the top menu bar of the ComfyUI
interface. You can open the corresponding login interface through this button and log
out of the corresponding account in the settings menu.


## ITEM:
label: 'My Extension v1.0.0',


## ITEM:
url: 'https://github.com/myuser/myextension',


## ITEM:
icon: 'pi pi-github'


## ITEM:
}


## ITEM:
]


## ITEM:
})


## ITEM:
```bash
# Section: Server Config
```
