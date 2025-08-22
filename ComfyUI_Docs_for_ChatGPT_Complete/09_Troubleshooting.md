# SECTION: TROUBLESHOOTING


## ITEM:
Troubleshooting


## ITEM:
• 	Intel GPU Compatibility: Fixed Intel integrated GPU compatibility issues


## ITEM:
• 	PyTorch Compatibility: Enhanced compatibility with older PyTorch versions


## ITEM:
• 	Torch Compile Optimization: Improved torch compile behavior


## ITEM:
• 	RDNA3 Architecture Fixes: Resolved issues with gfx1201 GPUs when using Flux
models with PyTorch attention


## ITEM:
• 	Updated PyTorch Support: Bumped CUDA and ROCM PyTorch versions with
testing on Python 3.13 and CUDA 12.9


## ITEM:
Developer Experience Enhancements


## ITEM:
• 	Cleaner Logging: Feature flags now only display in verbose mode, reducing
console noise


## ITEM:
• 	WanFirstLastFrameToVideo Fix: Resolved issue preventing proper video
generation when clip vision components are not available


## ITEM:
Performance & Model Optimizations


## ITEM:
• 	VAE Nonlinearity Enhancement: Replaced manual activation functions with
optimized torch.silu in VAE operations


## ITEM:
• 	WAN VAE Optimizations: Fine-tuning optimizations for WAN VAE operations,
improving processing speed and memory eﬃciency


## ITEM:
Node Schema Evolution


## ITEM:
• 	V3 Node Schema Definition: Implementation of next-generation node schema
system


## ITEM:
• 	Template Updates: Multiple template version updates (0.1.44, 0.1.45) ensuring
compatibility


## ITEM:
• 	Python 3.9 Compatibility: Fixed compatibility issues ensuring broader platform
support


## ITEM:
Bug Fixes & Stability


## ITEM:
• 	MaskComposite Fixes: Resolved errors when destination masks have 2
dimensions


## ITEM:
• 	Latent Conditioning Fix: Resolved issues with conditioning at index > 0 for multi-
step workflows


## ITEM:
• 	Denoising Steps: Added denoising step support to several samplers


## ITEM:
Platform Stability


## ITEM:
• 	PyTorch Compatibility: Fixed contiguous memory issues with PyTorch nightly
builds


## ITEM:
• 	FP8 Fallback: Automatic fallback to regular operations when FP8 operations
encounter exceptions


## ITEM:
• 	Apple Silicon Fixes: Addressed FP16 attention issues on Apple devices


## ITEM:
Solution: You can try changing the fixed version dependency to a range constraint,
such as open_clip_torch>=2.26.1, and then reinstall the dependencies to resolve these
issues.


## ITEM:
2. Environment pollution


## ITEM:
Solution: These types of dependency conflicts may be more diﬃcult to resolve, and
you may need to upgrade/downgrade ComfyUI or change the dependency versions of
custom nodes to resolve these issues.


## ITEM:
## Troubleshooting


## ITEM:
Problem: If your color palette changes don’t appear.


## ITEM:
Solution: Try refreshing the page


## ITEM:
Problem: If CSS customizations didn’t work


## ITEM:
Solution: Check that you’re using frontend version 1.20.5+


## ITEM:
Problem:


## ITEM:
Solution: Try adding !important to user.css rules that aren’t being applied


## ITEM:
Problem:


## ITEM:
Solution: Keep Backups of your Customizations to easily restore them.


## ITEM:
```bash
# Section: 3D
```


## ITEM:
• When debugging or troubleshooting requires using standard implementations


## ITEM:
Default hashing function for model files


## ITEM:
Options:


## ITEM:
• 	 sha256: Uses SHA-256 algorithm for hash verification, high security but
slower computation


## ITEM:
• 	 sha1: Uses SHA-1 algorithm, faster but slightly lower security


## ITEM:
• 	 sha512: Uses SHA-512 algorithm, provides highest security but slowest
computation


## ITEM:
• 	 md5: Uses MD5 algorithm, fastest but lowest security


## ITEM:
Function: Sets the hash algorithm for model file verification, used to verify file integrity.
Diﬀerent hash algorithms have diﬀerent trade-oﬀs between computation speed and
security. Usually recommended to use sha256 as the default option, which achieves a
good balance between security and performance.


## ITEM:
Make pytorch use slower deterministic algorithms when it can


## ITEM:
Function: Forces PyTorch to use deterministic algorithms when possible to improve
result reproducibility.


## ITEM:
Description:


## ITEM:
• When enabled, PyTorch will prioritize deterministic algorithms over faster non-
deterministic algorithms


## ITEM:
• Same inputs will produce same outputs, helpful for debugging and result
verification


## ITEM:
• Deterministic algorithms typically run slower than non-deterministic algorithms


## ITEM:
• Even with this setting enabled, completely identical image results cannot be
guaranteed in all situations


## ITEM:
Use Cases:


## ITEM:
• Scientific research requiring strict result reproducibility


## ITEM:
• Debugging processes requiring stable output results


## ITEM:
• Production environments requiring result consistency


## ITEM:
Enable some untested and potentially quality deteriorating optimizations


## ITEM:
Function: Enables experimental optimizations that may improve speed but could
potentially aﬀect generation quality


## ITEM:
Don’t print server output to console


## ITEM:
Function: Prevents displaying server runtime information in the console, keeping the
interface clean.


## ITEM:
Description:


## ITEM:
• When enabled, ComfyUI server logs and runtime information will not be
displayed


## ITEM:
• Can reduce console information interference, making the interface cleaner


## ITEM:
• May slightly improve system performance when there’s heavy log output


## ITEM:
• Default is disabled (false), meaning server output is displayed by default


## ITEM:
Use Cases:


## ITEM:
• Production environments where debugging information is not needed


## ITEM:
• When wanting to keep the console interface clean


## ITEM:
• When the system runs stably and log monitoring is not required


## ITEM:
Note: It’s recommended to keep this option disabled during development and
debugging to promptly view server runtime status and error information.


## ITEM:
Disable saving prompt metadata in files


## ITEM:
Function: Prevents loading all third-party extension nodes, typically used when
troubleshooting issues to locate whether errors are caused by third-party extension
nodes


## ITEM:
Logging verbosity level


## ITEM:
Function: Controls the verbosity level of log output, used for debugging and monitoring
system runtime status.


## ITEM:
Options:


## ITEM:
• 	 CRITICAL: Only outputs critical error information that may cause the
program to stop running


## ITEM:
• 	 ERROR: Outputs error information indicating some functions cannot work
properly


## ITEM:
• 	 WARNING: Outputs warning information indicating possible issues that
don’t aﬀect main functionality


## ITEM:
• 	 INFO: Outputs general information including system runtime status and
important operation records


## ITEM:
• 	 DEBUG: Outputs the most detailed debugging information including
system internal runtime details


## ITEM:
Description:


## ITEM:
• Log levels increase in verbosity from top to bottom


## ITEM:
• Each level includes all log information from higher levels


## ITEM:
• Recommended to set to INFO level for normal use


## ITEM:
• Can be set to DEBUG level when troubleshooting for more information


## ITEM:
• Can be set to WARNING or ERROR level in production environments to reduce
log volume


## ITEM:
Directories


## ITEM:
Input directory


## ITEM:
Troubleshooting


## ITEM:
```bash
# Table of Contents
```


## ITEM:
1. Overview


## ITEM:
2. Model Issues


## ITEM:
Troubleshooting


## ITEM:
How to Troubleshoot and Solve ComfyUI Issues


## ITEM:
Common ComfyUI issues, solutions, and how to report bugs eﬀectively


## ITEM:
We receive a lot of feedback issues, and we find that most of the issues submitted are
related to custom nodes. So please ensure that you have read the custom node
troubleshooting guide before submitting an error report to ensure that the issue is not
caused by ComfyUI core issues.


## ITEM:
Custom Node Troubleshooting Guide


## ITEM:
Common Issues & Quick Fixes


## ITEM:
Before diving into detailed troubleshooting, try these common solutions:


## ITEM:
ComfyUI Won’t Start


## ITEM:
Symptoms: Application crashes on startup, black screen, or fails to load


## ITEM:
Quick fixes:


## ITEM:
1. Check system requirements - Ensure your system meets the minimum
requirements


## ITEM:
2. Update GPU drivers - Download latest drivers from NVIDIA/AMD/Intel


## ITEM:
Generation Fails or Produces Errors


## ITEM:
2. Check if it’s a custom node issue - Follow our custom node troubleshooting
guide


## ITEM:
For comprehensive desktop installation troubleshooting, see the Desktop Installation
Guide.


## ITEM:
• 	Windows


## ITEM:
• 	macOS


## ITEM:
• 	Linux


## ITEM:
For comprehensive model troubleshooting including architecture mismatches, missing
models, and loading errors, see the dedicated Model Issues page.


## ITEM:
Network & API Issues


## ITEM:
2. 	Try basic troubleshooting:


## ITEM:
• 	Disable all custom nodes (see custom node troubleshooting)


## ITEM:
• 	Check console/terminal for error messages


## ITEM:
• 	If using comfy-cli, try updating: comfy node update all


## ITEM:
How to Report Bugs Eﬀectively


## ITEM:
For ComfyUI Core Issues


## ITEM:
Where to report: GitHub Issues


## ITEM:
For Desktop App Issues


## ITEM:
Where to report: Desktop GitHub Issues


## ITEM:
For Frontend Issues


## ITEM:
Where to report: Frontend GitHub Issues


## ITEM:
Troubleshooting


## ITEM:
How to Troubleshoot and Solve ComfyUI Model Issues


## ITEM:
Troubleshooting model-related problems including architecture mismatches, missing
models, and loading errors


## ITEM:
Model Architecture Mismatch


## ITEM:
Symptoms: Tensor dimension errors during generation, especially during VAE decode
stage


## ITEM:
Common error messages:


## ITEM:
• 	Given groups=1, weight of size [64, 4, 3, 3], expected input[1, 16, 128, 128] to
have 4 channels, but got 16 channels instead


## ITEM:
• 	Given groups=1, weight of size [4, 4, 1, 1], expected input[1, 16, 144, 112] to
have 4 channels, but got 16 channels instead


## ITEM:
• 	Given groups=1, weight of size [320, 4, 3, 3], expected input[2, 16, 192, 128] to
have 4 channels, but got 16 channels instead


## ITEM:
• 	The size of tensor a (49) must match the size of tensor b (16) at non-singleton
dimension 1


## ITEM:
• 	Tensors must have same number of dimensions: got 2 and 3


## ITEM:
• 	mat1 and mat2 shapes cannot be multiplied (154x2048 and 768x320)


## ITEM:
Troubleshooting


## ITEM:
How to Troubleshoot and Solve ComfyUI Issues


## ITEM:
Here is the overall approach for troubleshooting custom node issues:


## ITEM:
#_r_1s_{font-family:inherit;font-size:16px;fill:#ccc;}#_r_1s_ .error-icon{fill:#a44141;}
#_r_1s_ .error-text{fill:#ddd;stroke:#ddd;}#_r_1s_ .edge-thickness-normal{stroke-
width:1px;}#_r_1s_ .edge-thickness-thick{stroke-width:3.5px;}#_r_1s_ .edge-pattern-
solid{stroke-dasharray:0;}#_r_1s_ .edge-thickness-invisible{stroke-width:0;fill:none;}


## ITEM:
#_r_1s_ .edge-pattern-dashed{stroke-dasharray:3;}#_r_1s_ .edge-pattern-
dotted{stroke-dasharray:2;}#_r_1s_ .marker{fill:lightgrey;stroke:lightgrey;}
#_r_1s_ .marker.cross{stroke:lightgrey;}#_r_1s_ svg{font-family:inherit;font-size:16px;}
#_r_1s_ p{margin:0;}#_r_1s_ .label{font-family:inherit;color:#ccc;}#_r_1s_ .cluster-label
text{fill:#F9FFFE;}#_r_1s_ .cluster-label span{color:#F9FFFE;}#_r_1s_ .cluster-label
span p{background-color:transparent;}#_r_1s_ .label text,#_r_1s_
span{fill:#ccc;color:#ccc;}#_r_1s_ .node rect,#_r_1s_ .node circle,#_r_1s_ .node
ellipse,#_r_1s_ .node polygon,#_r_1s_ .node path{fill:#1f2020;stroke:#ccc;stroke-
width:1px;}#_r_1s_ .rough-node .label text,#_r_1s_ .node .label text,#_r_1s_ .image-
shape .label,#_r_1s_ .icon-shape .label{text-anchor:middle;}#_r_1s_ .node .katex
path{fill:#000;stroke:#000;stroke-width:1px;}#_r_1s_ .rough-
node .label,#_r_1s_ .node .label,#_r_1s_ .image-shape .label,#_r_1s_ .icon-
shape .label{text-align:center;}#_r_1s_ .node.clickable{cursor:pointer;}
#_r_1s_ .root .anchor path{fill:lightgrey!important;stroke-width:0;stroke:lightgrey;}
#_r_1s_ .arrowheadPath{fill:lightgrey;}#_r_1s_ .edgePath .path{stroke:lightgrey;stroke-
width:2.0px;}#_r_1s_ .flowchart-link{stroke:lightgrey;fill:none;}
#_r_1s_ .edgeLabel{background-color:hsl(0, 0%, 34.4117647059%);text-align:center;}
#_r_1s_ .edgeLabel p{background-color:hsl(0, 0%, 34.4117647059%);}
#_r_1s_ .edgeLabel rect{opacity:0.5;background-color:hsl(0, 0%,
34.4117647059%);fill:hsl(0, 0%, 34.4117647059%);}#_r_1s_ .labelBkg{background-
color:rgba(87.75, 87.75, 87.75, 0.5);}#_r_1s_ .cluster rect{fill:hsl(180, 1.5873015873%,
28.3529411765%);stroke:rgba(255, 255, 255, 0.25);stroke-width:1px;}#_r_1s_ .cluster
text{fill:#F9FFFE;}#_r_1s_ .cluster span{color:#F9FFFE;}#_r_1s_
div.mermaidTooltip{position:absolute;text-align:center;max-
width:200px;padding:2px;font-family:inherit;font-size:12px;background:hsl(20,
1.5873015873%, 12.3529411765%);border:1px solid rgba(255, 255, 255, 0.25);border-
radius:2px;pointer-events:none;z-index:100;}#_r_1s_ .flowchartTitleText{text-
anchor:middle;font-size:18px;fill:#ccc;}#_r_1s_ rect.text{fill:none;stroke-width:0;}
#_r_1s_ .icon-shape,#_r_1s_ .image-shape{background-color:hsl(0, 0%,
34.4117647059%);text-align:center;}#_r_1s_ .icon-shape p,#_r_1s_ .image-shape
p{background-color:hsl(0, 0%, 34.4117647059%);padding:2px;}#_r_1s_ .icon-shape
rect,#_r_1s_ .image-shape rect{opacity:0.5;background-color:hsl(0, 0%,
34.4117647059%);fill:hsl(0, 0%, 34.4117647059%);}#_r_1s_ :root{--mermaid-font-
family:inherit;}


## ITEM:
Do
es
the
issu
e
dis
app
ear
afte
r
dis
abli
ng
all
cus
tom
nod
es?


## ITEM:
Iss
ue
cau
sed
by
cus
tom
nod
es


## ITEM:
Iss
ue
not
cau
sed
by
cus
tom
nod


## ITEM:
S
pl
it
Y Y Y St
N N N al
e e e ar
o o o l
s s s t
c
u
st


## ITEM:
In this document,
we categorize
custom nodes into
two types for
troubleshooting:
