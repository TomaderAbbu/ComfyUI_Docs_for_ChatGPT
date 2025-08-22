# SECTION: FULL_TEXT_APPENDIX (Raw Extract)


```
Get Started
Getting Started with AI Image Generation
This tutorial will guide you through your first image generation with ComfyUI,
covering basic interface operations like workflow loading, model installation, and
image generation
This guide aims to help you understand ComfyUI’s basic operations and complete
your first image generation. We’ll cover:
1. Loading example workflows
• Loading from ComfyUI’s workflow templates
• Loading from images with workflow metadata
2. Model installation guidance
• Automatic model installation
• Manual model installation
• Using ComfyUI Manager for model installation
3. Completing your first text-to-image generation

About Text-to-Image
Text-to-Image is a fundamental AI drawing feature that generates images from text
descriptions. It’s one of the most commonly used functions in AI art generation. You
can think of the process as telling your requirements (positive and negative prompts)
to an artist (the drawing model), who will then create what you want. Detailed
explanations about text-to-image will be covered in the Text to Image chapter.

ComfyUI Text-to-Image Workflow Tutorial

1. Launch ComfyUI
Make sure you’ve followed the installation guide to start ComfyUI and can
successfully enter the ComfyUI interface.

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

2. Load Default Text-to-Image Workflow
ComfyUI usually loads the default text-to-image workflow automatically when
launched. However, you can try different methods to load workflows to familiarize
yourself with ComfyUI’s basic operations:
•   Load from Workflow Template
•   Load from Images with Metadata
•   Load from workflow.json

Follow the numbered steps in the image:
1. Click the Fit View button in the bottom right to ensure any loaded workflow
isn’t hidden
2. Click the folder icon (workflows) in the sidebar
3. Click the Browse example workflows button at the top of the Workflows panel
Continue with:

4. Select the first default workflow Image Generation to load it
Alternatively, you can select Browse workflow templates from the workflow menu

3. Model Installation
Most ComfyUI installations don’t include base models by default. After loading the
workflow, if you don’t have the v1-5-pruned-emaonly-fp16.safetensors model
installed, you’ll see this prompt:


All models are stored in <your ComfyUI installation>/ComfyUI/models/ with
subfolders like checkpoints, embeddings, vae, lora, upscale_model, etc.
ComfyUI detects models in these folders and paths configured in
extra_model_paths.yaml at startup.

You can install models through:
•   Automatic Download
•   ComfyUI Manager
•   Manual Installation
After you click the Download button, ComfyUI will execute the download, and
different behaviors will be performed depending on the version you are using.
•   ComfyUI Desktop
•   ComfyUI Portable
The desktop version will automatically complete the model download and save it to
the <your ComfyUI installation location>/ComfyUI/models/checkpoints directory.
You can wait for the installation to complete or view the installation progress in the
model panel on the sidebar.

If everything goes smoothly, the model should be able to download locally. If the
download fails for a long time, please try other installation methods.

4. Load Model and Generate Your First Image
After installing the model:

1. In the Load Checkpoint node, ensure v1-5-pruned-emaonly-fp16.safetensors is
selected
2. Click Queue or press Ctrl + Enter to generate
The result will appear in the Save Image node. Right-click to save locally.

For detailed text-to-image instructions, see our comprehensive guide:
ComfyUI Text-to-Image Workflow Guide

Click here for detailed text-to-image workflow instructions

Troubleshooting

Model Loading Issues
If the Load Checkpoint node shows no models or displays “null”, verify your model
installation location and try refreshing or restarting ComfyUI.
_____________________________________
_____________________________________
_____________________________________
Get Started

Changelog

Track ComfyUI’s latest features, improvements, and bug fixes

v0.3.51

August 20, 2025

Model Support

• 	Qwen-Image-Edit Model: Native support for Qwen-Image-Edit

• 	FluxKontextMultiReferenceLatentMethod Node: Multi-reference input node for
Flux workflows

• 	WAN 2.2 Fun Camera Model Support: Support for video generation through
camera control

• 	Template Updates: Upgraded to version 0.1.62, added Wan2.2 Fun Camera and
Qwen Image Edit templates

Core Function Improvements

• 	Context Windows Support: Enhanced sampling code to support longer
sequence generation tasks

• 	SDPA Backend Optimization: Improved Scaled Dot Product Attention backend
settings for better performance

Multimedia Node Support

• 	Audio Recording Node: New native audio recording node, now you can record
audio directly in ComfyUI

• 	Audio Video Integration: Complete audio-video dependency integration

API Node Support Updates

• 	GPT-5 Series Models: Support for the latest GPT-5 models

• 	Kling V2-1 and V2-1-Master: Updated video generation model functionality

• 	Minimax Hailuo Video Node: New video generation node

• 	Vidu Video Node: Vidu API node support

• 	Google Model Updates: Added new Google Gemini models

• 	OpenAI API Fix: Fixed MIME type errors in OpenAI API node input images

Performance Optimization

• 	Intel GPU Compatibility: Fixed Intel integrated GPU compatibility issues

• 	PyTorch Compatibility: Enhanced compatibility with older PyTorch versions

• 	Torch Compile Optimization: Improved torch compile behavior

• 	Memory Management: Optimized installation size and memory eﬃciency

Frontend Changes

• 	Subgraph Support: Subgraph functionality support

• 	Shortcut Panel: Added bottom shortcut panel

• 	UI Layout Modifications: Modified terminal entry layout, added template, log
panel and other entries

• 	Standard Canvas Mode: Added standard canvas mode, can be switched in Lite
Graph > Canvas > Canvas Navigation Mode

• 	Mini Map: Added workflow mini map

• 	Tab Preview: Added workflow tab preview

• 	Top Tab Menu Layout Adjustments

v0.3.50

August 13, 2025

Model Integration & Performance Enhancements

This release expands ComfyUI’s model ecosystem with enhanced Qwen support,
async API capabilities, and stability improvements for complex workflows:

Qwen Model Ecosystem

• 	Qwen Image Model Support: Improved integration including proper LoRA
loading and model merging capabilities for sophisticated vision workflows

• 	Qwen Model Merging Node: New dedicated node for merging Qwen image
models, allowing creators to combine diﬀerent model strengths

• 	SimpleTuner Lycoris LoRA Support: Extended compatibility with SimpleTuner-
trained Lycoris LoRAs for Qwen-Image models

API & Performance Infrastructure

• 	Async API Nodes: Introduction of asynchronous API nodes, enabling non-
blocking workflow execution for better performance

• 	Memory Handling: Enhanced RepeatLatentBatch node now properly handles
multi-dimensional latents, fixing workflow interruptions

• 	WAN 2.2 Fun Control Support: Added support for WAN 2.2 fun control features,
expanding creative control for video workflows

Hardware Optimization & Compatibility

• 	AMD GPU Improvements: Enhanced AMD Radeon support with improved FP16
accuracy handling and performance optimization

• 	RDNA3 Architecture Fixes: Resolved issues with gfx1201 GPUs when using Flux
models with PyTorch attention

• 	Updated PyTorch Support: Bumped CUDA and ROCM PyTorch versions with
testing on Python 3.13 and CUDA 12.9

Developer Experience Enhancements

• 	Cleaner Logging: Feature flags now only display in verbose mode, reducing
console noise

• 	Audio Processing Safety: Enhanced torchaudio import safety checks prevent
crashes when audio dependencies are unavailable

• 	Kling API Improvements: Fixed image type parameter handling in Kling Image
API nodes

Workflow Benefits

• 	Async Workflow Execution: New async API capabilities enable more responsive
workflows when integrating external services

• 	Model Flexibility: Expanded Qwen support allows for more diverse vision-
language workflows with improved LoRA compatibility

• 	Hardware Utilization: AMD GPU optimizations and updated PyTorch support
improve performance across hardware configurations

• 	Batch Processing: Fixed RepeatLatentBatch ensures reliable operation with
complex multi-dimensional data structures

• 	Video Control: WAN 2.2 fun control features provide advanced creative control
for video generation workflows

v0.3.49

August 5, 2025

UI Experience & Model Support

This release brings user experience improvements and model support that enhance
workflow creation and performance:

User Interface Enhancements

• 	Recently Used Items API: New API for tracking recently used items in the
interface, streamlining workflow creation

• 	Workflow Navigation: Enhanced user experience with better organization of
commonly accessed elements

Model Integration

• 	Qwen Vision Model Support: Initial support for Qwen image models with
configuration options

• 	Image Processing: Enhanced Qwen model integration allows for more versatile
image analysis and generation workflows

Video Generation

• 	Veo3 Video Generation: Added Veo3 video generation node with integrated
audio support

• 	Audio-Visual Synthesis: Capability combining video and audio generation in a
single node

Performance & Stability Improvements

• 	Memory Management: Optimized conditional VRAM usage through improved
casting and device transfer operations

• 	Device Consistency: Fixes ensuring all conditioning data and context remain on
correct devices

• 	ControlNet Stability: Resolved ControlNet compatibility issues, restoring
functionality for image control workflows

Developer & System Enhancements

• 	Error Handling: Added warnings and crash prevention when conditioning
devices don’t match

• 	Template Updates: Multiple template version updates (0.1.47, 0.1.48, 0.1.51)
maintaining compatibility

Workflow Benefits

• 	Faster Iteration: Recently used items API enables quicker workflow assembly
and modification

• 	Enhanced Creativity: Qwen vision models open new possibilities for image
understanding and manipulation workflows

• 	Video Production: Veo3 integration transforms ComfyUI into a comprehensive
multimedia creation platform

• 	Reliability: Memory optimizations and device management fixes ensure stable
operation with complex workflows

• 	Performance: Optimized VRAM usage allows for more ambitious projects on
systems with limited resources

v0.3.48

August 2, 2025

API Enhancement & Performance Optimizations

This release introduces backend improvements and performance optimizations that
enhance workflow execution and node development:

ComfyAPI Core Framework

• 	ComfyAPI Core v0.0.2: Update to the core API framework, providing improved
stability and extensibility

• 	Partial Execution Support: New backend support for partial workflow execution,
enabling eﬃcient processing of multi-stage workflows

Video Processing Improvements

• 	WAN Camera Memory Optimization: Enhanced memory management for WAN-
based camera workflows, reducing VRAM usage

• 	WanFirstLastFrameToVideo Fix: Resolved issue preventing proper video
generation when clip vision components are not available

Performance & Model Optimizations

• 	VAE Nonlinearity Enhancement: Replaced manual activation functions with
optimized torch.silu in VAE operations

• 	WAN VAE Optimizations: Fine-tuning optimizations for WAN VAE operations,
improving processing speed and memory eﬃciency

Node Schema Evolution

• 	V3 Node Schema Definition: Implementation of next-generation node schema
system

• 	Template Updates: Multiple template version updates (0.1.44, 0.1.45) ensuring
compatibility

Workflow Development Benefits

• 	Video Workflows: Improved stability and performance for video generation
pipelines

• 	Memory Management: Optimized memory usage patterns enable more complex
workflows on systems with limited VRAM

• 	API Reliability: Core API enhancements provide more stable foundation for
custom node development

• 	Execution Flexibility: New partial execution capabilities allow for more eﬃcient
debugging and development

v0.3.47

July 30, 2025

Memory Optimization & Large Model Performance

This release focuses on memory optimizations for large model workflows, improving
performance with WAN 2.2 models and VRAM management:

WAN 2.2 Model Optimizations

• 	Reduced Memory Footprint: Eliminated unnecessary memory clones in WAN 2.2
VAE operations, reducing memory usage

• 	5B I2V Model Support: Memory optimization for WAN 2.2 5B image-to-video
models, making these models more accessible

Enhanced VRAM Management

• 	Windows Large Card Support: Added reserved VRAM allocation for high-end
graphics cards on Windows

• 	Memory Allocation: Improved memory management for users working with
multiple large models simultaneously

Workflow Performance Benefits

• 	VAE Processing: WAN 2.2 VAE operations now run more eﬃciently with reduced
memory overhead

• 	Large Model Inference: Enhanced stability when working with billion-parameter
models

• 	Batch Processing: Memory optimizations enable better handling of batch
operations with large models

v0.3.46

July 28, 2025

Hardware Acceleration & Audio Processing

This release expands hardware support and enhances audio processing capabilities:

Audio Processing Enhancements

• 	PyAV Audio Backend: Replaced torchaudio.load with PyAV for more reliable
audio processing in video workflows

• 	Audio Integration: Enhanced audio handling for multimedia generation
workflows

Hardware Support

• 	Iluvatar CoreX Support: Added native support for Iluvatar CoreX accelerators

• 	Intel XPU Optimization: XPU support improvements including async oﬄoad
capabilities

• 	AMD ROCm Enhancements: Enabled PyTorch attention by default for gfx1201
on Torch 2.8

• 	CUDA Memory Management: Fixed CUDA malloc to only activate on CUDA-
enabled PyTorch installations

Sampling Algorithm Improvements

• 	Euler CFG++ Enhancement: Separated denoised and noise estimation
processes in Euler CFG++ sampler

• 	WAN Model Support: Added support for WAN (Wavelet-based Attention
Network) models

Training Features

• 	Training Nodes: Added algorithm support, gradient accumulation, and optional
gradient checkpointing

• 	Training Flexibility: Better memory management and performance optimization
for custom model training

Node & Workflow Enhancements

• 	Moonvalley V2V Node: Added Moonvalley Marey V2V node with enhanced input
validation

• 	Negative Prompt Updates: Improved negative prompt handling for Moonvalley
nodes

• 	History API Enhancement: Added map_function parameter to get_history API

API & System Improvements

• 	Frontend Version Tracking: Added required_frontend_version parameter in /
system_stats API response

• 	Device Information: Enhanced XPU device name printing for better hardware
identification

• 	Template Updates: Multiple template updates (0.1.40, 0.1.41) ensuring
compatibility

Developer Experience

• 	Documentation Updates: Enhanced README with examples and updated
model integration guides

• 	Line Ending Fixes: Improved cross-platform compatibility by standardizing line
endings

• 	Code Cleanup: Removed deprecated code and optimized components

v0.3.45

July 21, 2025

Sampling & Training Improvements

This release introduces enhancements to sampling algorithms, training capabilities,
and node functionality:

Sampling & Generation Features

• 	SA-Solver Sampler: New reconstructed SA-Solver sampling algorithm providing
enhanced numerical stability

• 	Experimental CFGNorm Node: Classifier-free guidance normalization for
improved control over generation quality

• 	Nested Dual CFG Support: Added nested style configuration to DualCFGGuider
node

• 	SamplingPercentToSigma Node: New utility node for precise sigma calculation
from sampling percentages

Training Capabilities

• 	Multi Image-Caption Dataset Support: LoRA training node now handles multiple
image-caption datasets simultaneously

• 	Training Loop Implementation: Optimized training algorithms for improved
convergence and stability

• 	Error Detection: Added model detection error hints for LoRA operations

Platform & Performance Improvements

• 	Async Node Support: Full support for asynchronous node functions with earlier
execution optimization

• 	Chroma Flexibility: Un-hardcoded patch_size parameter in Chroma

• 	LTXV VAE Decoder: Switched to improved default padding mode for better
image quality

• 	Safetensors Memory Management: Added workaround for mmap issues

API & Integration Enhancements

• 	Custom Prompt IDs: API now allows specifying prompt IDs for better workflow
tracking

• 	Kling API Optimization: Increased polling timeout to prevent user timeouts

• 	History Token Cleanup: Removed sensitive tokens from history items

• 	Python 3.9 Compatibility: Fixed compatibility issues ensuring broader platform
support

Bug Fixes & Stability

• 	MaskComposite Fixes: Resolved errors when destination masks have 2
dimensions

• 	Fresca Input/Output: Corrected input and output handling for Fresca model
workflows

• 	Reference Bug Fixes: Resolved incorrect reference bugs in Gemini node
implementations

• 	Line Ending Standardization: Automated detection and removal of Windows line
endings

Developer Experience

• 	Warning Systems: Added torch import mistake warnings to catch common
configuration issues

• 	Template Updates: Multiple template version updates (0.1.36, 0.1.37, 0.1.39) for
improved custom node development

• 	Documentation: Enhanced fast_fp16_accumulation documentation

v0.3.44

July 8, 2025

Sampling & Model Control Enhancements

This release delivers improvements to sampling algorithms and model control systems:

Sampling Capabilities

• 	TCFG Node: Enhanced classifier-free guidance control for more nuanced
generation control

• 	ER-SDE Sampler: Migrated from VE to VP algorithm with new sampler node

• 	Skip Layer Guidance (SLG): Implementation for precise layer-level control during
inference

Development Tools

• 	Custom Node Management: New --whitelist-custom-nodes argument pairs with
--disable-all-custom-nodes

• 	Performance Optimizations: Dual CFG node now optimizes automatically when
CFG is 1.0

• 	GitHub Actions Integration: Automated release webhook notifications

Image Processing Improvements

• 	Transform Nodes: Added ImageRotate and ImageFlip nodes for enhanced
image manipulation

• 	ImageColorToMask Fix: Corrected mask value returns for more accurate color-
based masking

• 	3D Model Support: Upload 3D models to custom subfolders for better
organization

Guidance & Conditioning Enhancements

• 	PerpNeg Guider: Updated with improved pre and post-CFG handling

• 	Latent Conditioning Fix: Resolved issues with conditioning at index > 0 for multi-
step workflows

• 	Denoising Steps: Added denoising step support to several samplers

Platform Stability

• 	PyTorch Compatibility: Fixed contiguous memory issues with PyTorch nightly
builds

• 	FP8 Fallback: Automatic fallback to regular operations when FP8 operations
encounter exceptions

• 	Audio Processing: Removed deprecated torchaudio.save function dependencies

Model Integration

• 	Moonvalley Nodes: Added native support for Moonvalley model workflows

• 	Scheduler Reordering: Simple scheduler now defaults first

• 	Template Updates: Multiple template version updates (0.1.31-0.1.35)

Security & Safety

• 	Safe Loading: Added warnings when loading files unsafely

• 	File Validation: Enhanced checkpoint loading safety measures

v0.3.43

June 30, 2025

Model Support & Workflow Reliability

This release brings improvements to model compatibility and workflow stability:

Expanded Model Documentation: Added support documentation for Flux Kontext and
Omnigen 2 models VAE Encoding Improvements: Removed unnecessary random noise
injection during VAE encoding Memory Management Fix: Resolved a memory
estimation bug aﬀecting Kontext model usage

v0.3.41

June 17, 2025

Model Support Additions

• 	Cosmos Predict2 Support: Implementation for text-to-image (2B and 14B
models) and image-to-video generation workflows

• 	Flux Compatibility: Chroma Text Encoder now works with regular Flux models

• 	LoRA Training Integration: New native LoRA training node using weight adapter
scheme

Performance & Hardware Optimizations

• 	AMD GPU Enhancements: Enabled FP8 operations and PyTorch attention on
AMD GPUs

• 	Apple Silicon Fixes: Addressed FP16 attention issues on Apple devices

• 	Flux Model Stability: Resolved black image generation issues with certain Flux
models

Sampling Improvements

• 	Rectified Flow Samplers: Added SEEDS and multistep DPM++ SDE samplers
with RF support

• 	ModelSamplingContinuousEDM: New cosmos_rflow option for enhanced
sampling control

• 	Memory Optimization: Improved memory estimation for Cosmos models

Developer & Integration Features

• 	SQLite Database Support: Enhanced data management capabilities for custom
nodes

• 	PyProject.toml Integration: Automatic web folder registration from pyproject files

• 	Frontend Flexibility: Support for semver suﬃxes and prerelease frontend
versions

• 	Tokenizer Enhancements: Configurable min_length settings with tokenizer_data

Quality of Life Improvements

• 	Kontext Aspect Ratio Fix: Resolved widget-only limitation

• 	SaveLora Consistency: Standardized filename format across all save nodes

• 	Python Version Warnings: Added alerts for outdated Python installations

• 	WebcamCapture Fixes: Corrected IS_CHANGED signature

v0.3.40

June 5, 2025

Workflow Tools & Performance Optimizations

This release brings new workflow utilities and performance optimizations:

Workflow Tools

• 	ImageStitch Node: Concatenate multiple images seamlessly in your workflows

• 	GetImageSize Node: Extract image dimensions with batch processing support

• 	Regex Replace Node: Advanced text manipulation capabilities for workflows

Model Compatibility

• 	Tensor Handling: Streamlined list processing makes multi-model workflows
more reliable

• 	BFL API Optimization: Refined support for Kontext models with cleaner node
interfaces

• 	Performance Boost: Fused multiply-add operations in chroma processing for
faster generation

Developer Experience

• 	Custom Node Support: Added pyproject.toml support for better dependency
management

• 	Help Menu Integration: New help system in the Node Library sidebar

• 	API Documentation: Enhanced API nodes documentation

Frontend & UI Enhancements

• 	Frontend Updated to v1.21.7: Stability fixes and performance improvements

• 	Custom API Base Support: Better subpath handling for custom deployment
configurations

• 	Security Hardening: XSS vulnerability fixes

Bug Fixes & Stability

• 	Pillow Compatibility: Updated deprecated API calls

• 	ROCm Support: Improved version detection for AMD GPU users

• 	Template Updates: Enhanced project templates for custom node development

_____________________________________
_____________________________________
_____________________________________
Basic Concepts

Workflow

A graph of nodes

ComfyUI is an environment for building and running generative content workflows. In
this context, a workflow is defined as a collection of program objects called nodes that
are connected to each other, forming a network. This network is also known as a
graph.

A ComfyUI workflow can generate any type of media: image, video, audio, AI model, AI
agent, and so on.

Sample workflows

To get started, try out some of the oﬃcial workflows. These use only the Core nodes
included in the ComfyUI installation. A thriving community of developers has created a
rich ecosystem of custom nodes to extend the functionality of ComfyUI.

Simple Example

Visual programming

A node-based computer program like ComfyUI provides a level of power and flexibility
that can’t be achieved with traditional menu- and button-driven applications. The
ComfyUI node graph is not limited by the tools provided in a traditional computer
application. It’s a high-level visual programming environment allowing users to design
complex systems without needing to write program code or understand advanced
mathematics.

Many other computer applications use this same node graph paradigm. Examples
include the compositing application called Nuke, the 3D programs Maya and Blender,
the Unreal real-time graphics engine, and the interactive media authoring program
called Max.

More Complex Example

Procedural framework

Another term used to describe a node-based application is procedural framework.
Procedural means generative: some procedure or algorithm is employed to generate
content such as a 3D model or a musical composition.

ComfyUI is all of these things: a node graph, a visual programming environment, and a
procedural framework. What makes ComfyUI diﬀerent (and amazing!) is that its
radically open structure allows us to generate any type of media asset such as picture,
movie, sound, 3D model, AI model, etc.

In the context of ComfyUI, the term workflow is a synonym for the node network or
graph. It corresponds to the scene graph in a 3D or multimedia program: the network
of all of the nodes within a particular disk file. 3D programs call this a scene file. Video
editing, compositing, and multimedia programs usually call it a project file.

Saving workflows

The ComfyUI workflow is automatically saved in the metadata of any generated image,
allowing users to open and use the graph that generated the image. A workflow can
also be stored in a human-readable text file that follows the JSON data format. This is
necessary for media formats that don’t support metadata. ComfyUI workflows stored
as JSON files are very small, allowing convenient versioning, archiving, and sharing of
graphs, independently of any generated media.

_____________________________________
_____________________________________
_____________________________________
Basic Concepts

Nodes

Understand the concept of a node in ComfyUI.

In ComfyUI, nodes are the fundamental building blocks for executing tasks. Each node
is an independently built module, whether it’s a Comfy Core node or a Custom Node,
with its own unique functionality. Nodes connect to each other through links, allowing
us to build complex functionality like assembling LEGO blocks. The combinations of
diﬀerent nodes create the unlimited possibilities of ComfyUI.

For example, in the K-Sampler node, you can see it has multiple inputs and outputs,
and also includes multiple parameter settings. These parameters determine the logic of
node execution. Behind each node is well-written Python logic, allowing you to achieve
corresponding functionality without having to write code yourself.

As ComfyUI is still in rapid iteration and development, we are continuously improving it
every day. Therefore, some operations mentioned in this article may change or be
omitted. Please refer to the actual interface. If you find changes in actual operations, it
may be due to our iterative updates. You can also fork this repo and help us improve
this documentation.

Nodes perform operations

In computer science, a node is a container for information, usually including
programmed instructions to perform some task. Nodes almost never exist in isolation,

they’re almost always connected to other nodes in a networked graph. In ComfyUI,
nodes take the visual form of boxes that are connected to each other.

ComfyUI nodes are usually function operators. This means that they operate on some
data to perform a function. A function is a process that accepts input data, performs
some operation on it, and produces output data. In other words, nodes do some work,
contributing to the completion of a task such as generating an image. So ComfyUI
nodes almost always have at least one input or output, and usually have multiple inputs
and outputs.

Diﬀerent Node States

In ComfyUI, nodes have multiple states. Here are some common node states:

1. 	Normal State: The default state

2. 	Running State: The running state, typically displayed when a node is executing
after you start running the workflow

3. 	Error State: Node error, typically displayed after running the workflow if there’s a
problem with the node’s input, indicated by red marking of the erroneous input
node. You need to fix the problematic input to ensure the workflow runs
correctly

4. 	Missing State: This state usually appears after importing workflows, with two
possibilities:

• 	Comfy Core native node missing: This usually happens because ComfyUI
has been updated, but you’re using an older version of ComfyUI. You
need to update ComfyUI to resolve this issue

• 	Custom node missing: The workflow uses custom nodes developed by
third-party authors, but your local ComfyUI version doesn’t have these
custom nodes installed. You can use ComfyUI-Manager to find and install
the missing custom nodes

Connections Between Nodes

In ComfyUI, nodes are connected through links, allowing data of the same type to flow
between diﬀerent processing units to achieve the final result.

Each node receives some input, processes it through its module, and converts it to
corresponding output. Connections between diﬀerent nodes must conform to the data
type requirements. In ComfyUI, we use diﬀerent colors to distinguish node data types.
Below are some basic data types:

Data type Color

diﬀusion model lavender
CLIP model yellow
VAE model rose
conditioning orange
latent image pink
pixel image blue
mask green
number (integer or float) light green
mesh bright green
As ComfyUI evolves, we may expand to more data types to meet the needs of more
scenarios.

Connecting and Disconnecting Nodes

Connecting: Drag from the output point of one node to the input of the same color on
another node to connect them Disconnecting: Click on the input endpoint and drag the
mouse left button to disconnect, or cancel the connection through the midpoint menu
of the link

Node Appearance

We provide various style settings for you to customize the appearance of nodes:

• Modify styles

• Double-click the node title to modify the node name

• Switch node inputs between input sockets and widgets through the context
menu

• Resize the node using the bottom right corner

Node Badges

We provide multiple node badge display features, such as:

• Node ID

• Node source

Currently, Comfy Core nodes use a fox icon for display, while custom nodes use their
names. This way you can quickly understand which node package a node comes from.

You can set the corresponding display in the menu:

Node Context Menus

Node context menus are mainly divided into two types:

• Context menu for the node itself

• Context menu for inputs/outputs

Node Context Menu

By right-clicking on a node, you can expand the corresponding node context menu:

In the node’s right-click context menu, you can:

• Adjust the node’s color style

• Modify the title

• Clone, copy, or delete the node

• Set the node’s mode

In this menu, besides appearance-related settings, the following menu operations are
important:

• 	Mode: Set the node’s mode: Always, Never, Bypass

• 	Toggle between Widget and Input mode for node inputs: Switch between widget
and input mode for node inputs

Mode

For modes, you may notice that we currently provide: Always, Never, On Event, On
Trigger - four modes, but actually only Always and Never are eﬀective. On Event and
On Trigger are currently ineﬀective as we haven’t fully implemented this feature.
Additionally, you can understand Bypass as a mode. Below is an explanation of the
available modes:

• 	Always: The default node mode. The node will execute whenever it runs for the
first time or when any of its inputs change since the last execution

• 	Never: The node will never execute under any circumstances, as if it’s been
deleted. Subsequent nodes cannot read or receive any data from it

• 	Bypass: The node will never execute under any circumstances, but subsequent
nodes can still try to obtain data that hasn’t been processed by this node

Below is a comparison of the Never and Bypass modes:

In this comparison example, you can see that both workflows apply two LoRA models
simultaneously, with the diﬀerence being that one Load LoRA node is set to Never
mode while the other is set to Bypass mode.

• 	The node set to Never mode causes subsequent nodes to show errors because
they don’t receive any input data

• 	The node set to Bypass mode still allows subsequent nodes to receive
unprocessed data, so they load the output data from the first Load LoRA node,
allowing the subsequent workflow to continue running normally

Switching Between Widget and Input Mode for Node Inputs

In some cases, we need to use output results from other nodes as input. In this case,
we can switch between widget and input mode for node inputs.

Here’s a very simple example:

By switching the K-Sampler’s Seed from widget to input mode, multiple nodes can
share the same seed, achieving variable uniformity across multiple samplers.
Comparing the first node with the subsequent two nodes, you can see that the seed in
the latter two nodes is in input mode. You can also convert it back to widget mode:

After frontend version v1.16.0, we improved this feature. Now you only need to directly
connect the input line to the corresponding widget to complete this process

Chenlei Hu

@HclHno3

·

Follow

Say goodbye to annoying widget <> socket conversion starting from frontend version
v1.16.0! Now each widget just always have an associated input socket by default
#ComfyUI

9:42 PM · Apr 6, 2025

235

Reply

Copy link

Input/Output Context Menu

This context menu is mainly related to the data type of the corresponding input/output:

When dragging the input/output of a node, if a connection appears but you haven’t
connected to another node’s input or output, releasing the mouse will pop up a context
menu for the input/output, used to quickly add related types of nodes. You can adjust
the number of node suggestions in the settings:

Node Selection Toolbox

The Node Selection Toolbox is a floating tool that provides quick operations for nodes.
When you select a node, it hovers above the selected node. Through this toolbox, you
can:

• Change the node’s color

• Quickly set the node to Bypass mode (not execute during runtime)

• Lock the node

• Delete the node

Of course, these functions can also be found in the right-click menu of the
corresponding node. The node selection toolbox just provides a shortcut operation. If
you want to disable this feature, you can turn it oﬀ in the settings.

Node Groups

In ComfyUI, you can select multiple parts of a workflow simultaneously, then use the
right-click menu to merge them into a node group, making that part a reusable module
that can be repeatedly called in your ComfyUI.

Custom Nodes

ComfyUI includes many powerful nodes in the base installation package. These are
known as Comfy Core nodes. Additionally, the ComfyUI community has created an
amazing array of custom nodes to perform a wide variety of functions.

ComfyUI Manager

The ComfyUI Manager window makes it easy to perform custom node management
tasks such as search, install, update, disable, and uninstall. The Manager is included in
the ComfyUI desktop application, but not in the ComfyUI server application.

Installing the ComfyUI Manager

If you’re running the ComfyUI server application, you need to install the Manager. If
ComfyUI is running, shut it down before proceeding.

The first step is to install Git, a command-line application for software version control.
Git will download the ComfyUI Manager from github.com. Download Git from git-
scm.com and install it.

Once Git is installed, navigate to the ComfyUI server program directory, to the folder
labeled custom_nodes. Open up a command window or terminal. Make sure that the
command line displays the current directory path as custom_nodes. Enter the following
command. This will download the Manager. Technically, this is known as cloning a Git
repository.

Copy

Ask AI

git clone https://github.com/ltdrdata/ComfyUI-Manager.git

For details or special cases, see ComfyUI Manager Install.

_____________________________________
_____________________________________
_____________________________________
Basic Concepts

Custom Nodes

Learn about installing, enabling dependencies, updating, disabling, and uninstalling
custom nodes in ComfyUI

About Custom Nodes

After installing ComfyUI, you’ll discover that it includes many built-in nodes. These
native nodes are called Comfy Core nodes, which are oﬃcially maintained by ComfyUI.

Additionally, there are numerous custom nodes created by various authors from the
ComfyUI community. These custom nodes bring extensive functionality to ComfyUI,
greatly expanding its capabilities and feature boundaries.

In this guide, we’ll cover various operations related to custom nodes, including
installation, updates, disabling, uninstalling, and dependency installation.

Anyone can develop their own custom extensions for ComfyUI and share them with
others. You can find many community custom nodes here. If you want to develop your
own custom nodes, visit the section below to get started:

Start Developing Custom Nodes

Learn how to start developing a custom node

Custom Node Management

In this section we will cover:

• Installing custom nodes

• Installing node dependencies

• Custom node version control

• Uninstalling custom nodes

• Temporarily disabling custom nodes

• Handling custom node dependency conflicts

1. Installing Custom Nodes

Currently, ComfyUI supports installing custom nodes through multiple methods,
including:

• 	Install via ComfyUI Manager (Recommended)

• 	Install via Git

• 	Manual installation

We recommend installing custom nodes through ComfyUI Manager, which is a highly
significant tool in the ComfyUI custom node ecosystem. It makes custom node
management (such as searching, installing, updating, disabling, and uninstalling)
simple - you just need to search for the node you want to install in ComfyUI Manager
and click install.

However, since all custom nodes are currently stored on GitHub, for regions that
cannot access GitHub normally, we have written detailed instructions for diﬀerent
custom node installation methods in this guide.

Additionally, since we recommend using ComfyUI Manager for plugin management, we
recommend using this tool for plugin management. You can find its source code here.
Therefore, in this documentation, we will use installing ComfyUI Manager as a custom
node installation example, and supplement how to use it for node management in the
relevant introduction sections.

• 	Install via ComfyUI Manager

• 	Install via Git

• 	Manual Installation

Since ComfyUI Manager has very rich functionality, we will use a separate document to
introduce the ComfyUI Manager installation chapter. Please visit the link below to learn
how to use ComfyUI Manager to install custom nodes.

Install Custom Nodes with ComfyUI Manager

Learn how to use ComfyUI Manager to install custom nodes

2. Installing Node Dependencies

Custom nodes all require the installation of related dependencies. For example, for
ComfyUI-Manager, you can visit the requirements.txt file to view the dependency
package requirements.

In the previous steps, we only cloned the custom node code locally and did not install
the corresponding dependencies, so next we need to install the corresponding
dependencies.

Actually, if you use ComfyUI-Manager to install plugins, ComfyUI Manager will
automatically help you complete the dependency installation. You just need to restart
ComfyUI after installing the plugin. This is why we strongly recommend using ComfyUI
Manager to install custom nodes.

But perhaps you may not be able to use ComfyUI Manager to install custom nodes
smoothly in some situations, so we provide this more detailed dependency installation
guide.

In the Dependencies chapter, we introduced the relevant content about dependencies
in ComfyUI. ComfyUI is a Python-based project, and we built an independent Python
runtime environment for running ComfyUI. All related dependencies need to be
installed in this independent Python runtime environment.

If you run pip install -r requirements.txt directly in the system-level terminal, the
corresponding dependencies may be installed in the system-level Python environment,
which will cause the dependencies to still be missing in ComfyUI’s environment,
preventing the corresponding custom nodes from running normally.

So next we need to use ComfyUI’s independent Python runtime environment to
complete the dependency installation.

Depending on diﬀerent ComfyUI versions, we will use diﬀerent methods to install the
corresponding dependencies:

• 	ComfyUI Portable

• 	ComfyUI Desktop

• 	Custom Python Environment Users

For ComfyUI Portable version, it uses an embedded Python located in the
\ComfyUI_windows_portable\python_embeded directory. We need to use this Python
to complete the dependency installation.

First, start the terminal in the portable version directory, or use the cd command to
navigate to the \ComfyUI_windows_portable\ directory after starting the terminal.

Ensure that the terminal directory is \ComfyUI_windows_portable\, as shown below for
D:\ComfyUI_windows_portable\

Then use python_embeded\python.exe to complete the dependency installation:

Copy

Ask AI

python_embeded\python.exe -m pip install -r ComfyUI\custom_nodes\ComfyUI-
Manager\requirements.txt

Of course, you can replace ComfyUI-Manager with the name of the custom node you
actually installed, but make sure that a requirements.txt file exists in the corresponding
node directory.

Custom Node Version Control

Custom node version control is actually based on Git version control. You can manage
node versions through Git, but ComfyUI Manager has already integrated this version
management functionality very well. Many thanks to @Dr.Lt.Data for bringing us such a
convenient tool.

In this section, we will still explain these two diﬀerent plugin version management
methods for you, but if you use ZIP packages for manual installation, the
corresponding git version history information will be lost, making it impossible to
perform version management.

• 	Version Management with ComfyUI Manager

• 	Version Management with Git

Since we are iterating on ComfyUI Manager, the actual latest interface and steps may
change significantly

1

Enter Node Management Interface

Perform the corresponding operations as shown to enter the ComfyUI Manager
interface

2

Find the Corresponding Custom Node Package

You can use the corresponding filters to filter out installed node packages and then
perform the corresponding node management

3

Perform Version Switching

Switch to the corresponding version. Manager will help you complete the
corresponding dependency updates and installation. Usually, you need to restart
ComfyUI after switching versions for the changes to take eﬀect.

Uninstalling Custom Nodes

To be updated

Temporarily Disabling Custom Nodes

To be updated

Custom Node Dependency Conflicts

To be updated

ComfyUI Manager

This tool is currently included by default in the Desktop version, while in the Portable
version, you need to refer to the installation instructions in the Install Manager section
of this document.

As ComfyUI continues to develop, ComfyUI Manager plays an increasingly important
role in ComfyUI. Currently, ComfyUI-Manager has oﬃcially joined the Comfy Org
organization, oﬃcially becoming part of ComfyUI’s core dependencies, and continues
to be maintained by the original author Dr.Lt.Data. You can read this blog post for more
information. In future iterations, we will greatly optimize the use of ComfyUI Manager,
so the interface shown in this documentation may diﬀer from the latest version of
ComfyUI Manager.

Installing the Manager

If you are running the ComfyUI server application, you need to install the manager. If
ComfyUI is running, please close it before continuing.

The first step is to install Git, which is a command-line application for software version
control. Git will download the ComfyUI manager from github.com. Download and install
Git from git-scm.com.

After installing Git, navigate to the ComfyUI server program directory and enter the
folder labeled custom_nodes. Open a command window or terminal. Make sure the
command line shows the current directory path as custom_nodes. Enter the following
command. This will download the manager. Technically, this is called cloning a Git
repository.

Detecting Missing Nodes

After installing the manager, you can detect missing nodes in the manager.

Developing a Custom Node

If you have some development capabilities, please start with the documentation below
to learn how to begin developing a custom node.

Start Developing Custom Nodes

Learn how to start developing a custom node

_____________________________________
_____________________________________
_____________________________________
Basic Concepts

Properties

Nodes are containers for properties

Nodes usually have properties. Also known as parameters or attributes, node
properties are variables that can be changed. Some properties can be adjusted
manually by the user, using a data entry field called a widget. Other properties can be
driven automatically by other nodes connected to the property input slot or port.
Usually, a property can be converted from widget to input and vice versa, allowing
users to control property values manually or automatically.

Properties can take many forms and hold many diﬀerent types of information. For
example, a Load Checkpoint node has a single property:  the file path to the generative
model checkpoint file. A KSampler node has multiple properties such as the number of
sampling steps, CFG scale, sampler_name, etc.

Data types

Information can come in many diﬀerent forms, called data types. For example,
alphanumeric text is known as a string, a whole number is an integer, and a number
with a decimal point is known as a floating point number or float. New data types are
always being added to ComfyUI.

ComfyUI is written in the Python scripting language, which is very forgiving about data
types. By contrast, the ComfyUI environment is very strongly typed. This means that
diﬀerent data types can’t be mixed up. For example, we can’t connect an image output
to an integer input. This is a huge benefit to users, guiding them to proper workflow
construction and preventing program errors.

_____________________________________
_____________________________________
_____________________________________
Basic Concepts

Links

Understand connection links in ComfyUI

As ComfyUI is still in rapid iteration and development, we are continuously improving it
every day. Therefore, some operations mentioned in this article may change or be
omitted. Please refer to the actual interface. If you find changes in actual operations, it
may be due to our iterative updates. You can also fork this repo and help us improve
this documentation.

Links connect nodes

In the terminology of ComfyUI, the lines or curves between nodes are called links.
They’re also known as connections or wires. Links can be displayed in several ways,
such as curves, right angles, straight lines, or completely hidden.

You can modify the link style in Setup Menu —> Display (Lite Graph) —> Graph —>
Link Render Mode.

You can also temporarily hide links in the Canvas Menu.

Link display is crucial. Depending on the situation, it may be necessary to see all links.
Especially when learning, sharing, or even just understanding workflows, the visibility
of links enables users to follow the flow of data through the graph. For packaged
workflows that aren’t intended to be altered, it might make sense to hide the links to
reduce clutter.

Reroute node

If legibility of the graph structure is important, then link wires can be manually routed in
the 2D space of the graph with a tiny node called Reroute. Its purpose is to position the
beginning and/or end points of link wires to ensure visibility. We can design a workflow
so that link wires don’t pass behind nodes, don’t cross other link wires, and so on.

We are also continuously improving the native reroute functionality in litegraph. We
recommend using this feature in the future to reorganize connections.

Color-coding

The data type of node properties is indicated by color coding of input/output ports and
link connection wires. We can always tell which inputs and outputs can be connected
to one another by their color. Ports can only be connected to other ports of the same
color to ensure matching data types.

Common data types:

Data type Color
diﬀusion model lavender
CLIP model yellow
VAE model rose
conditioning orange
latent image pink
pixel image blue
mask green
number (integer or float) light green
mesh bright green

_____________________________________
_____________________________________
_____________________________________
Basic Concepts

Models

Models are essential

Models are essential building blocks for media generation
workflows. They can be combined and mixed to achieve diﬀerent
creative eﬀects.

The word model has many diﬀerent meanings. Here, it means a
data file carrying information that is required for a node graph to
do its work. Specifically, it’s a data structure that models some
function. As a verb, to model something means to represent it or
provide an example.

The primary example of a model data file in ComfyUI is an AI
diﬀusion model. This is a large set of data that represents the
complex relationships among text strings and images, making it
possible to translate words into pictures or vice versa. Other
examples of common models used for image generation are
multimodal vision and language models such as CLIP, and
upscaling models such as RealESRGAN.

Model files

Model files are indispensable for generative media production.
Without them, workflows cannot proceed eﬀectively. Models are
not included in the ComfyUI installation, but ComfyUI can often
automatically download and install missing model files. Many
models can be downloaded and installed from the ComfyUI
Manager window. Models can also be found at websites such as
huggingface.co, civitai.green, and github.com.

Using Models in ComfyUI

1. Download and place them in the ComfyUI program directory

1. Within the models folder, you’ll find subfolders for
various types of models, such as checkpoints

2. The ComfyUI Manager helps to automate the process
of searching, downloading, and installing

3. Restart ComfyUI if it’s running

2. In your workflow, create the node appropriate to the model
type, e.g. Load Checkpoint, Load LoRA, Load VAE

3. In the loader node, choose the model you wish to use

4. Connect the loader node to other nodes in your workflow

Adding Extra Model Paths

If you want to manage your model files outside of ComfyUI/
models, you may have the following reasons:

• You have multiple ComfyUI instances and want them to
share model files to save disk space

• You have diﬀerent types of GUI programs (such as WebUI)
and want them to use the same model files

• Model files cannot be recognized or found

We provide a way to add extra model search paths via the
extra_model_paths.yaml configuration file

Open Config File

• 	 Portable/Manual Install

• 	 ComfyUI Desktop

For the ComfyUI version such as portable and manual, you can
find an example file named extra_model_paths.yaml.example in
the root directory of ComfyUI:

Copy

Ask AI

ComfyUI/extra_model_paths.yaml.example

Copy and rename it to extra_model_paths.yaml for use. Keep it in
ComfyUI’s root directory at ComfyUI/extra_model_paths.yaml.
You can also find the config example file here

If the file does not exist, you can create it yourself with any text
editor.

Example Structure

Suppose you want to add the following model paths to ComfyUI:

Copy

Ask AI

📁  YOUR_PATH/

  ├── 📁 models/

  |   ├── 📁  lora/

  |   │   └── xxxxx.safetensors

  |   ├── 📁  checkpoints/

  |   │   └── xxxxx.safetensors

  |   ├── 📁  vae/

  |   │   └── xxxxx.safetensors

  |   └── 📁  controlnet/

  |       └── xxxxx.safetensors

Then you can configure the extra_model_paths.yaml file like
below to let ComfyUI recognize the model paths on your device:

Copy

Ask AI

my_custom_config:

    base_path: YOUR_PATH

    loras: models/loras/

    checkpoints: models/checkpoints/

    vae: models/vae/

    controlnet: models/controlnet/

or

Copy

Ask AI

my_custom_config:

    base_path: YOUR_PATH/models/

    loras: loras

    checkpoints: checkpoints

    vae: vae

    controlnet: controlnet

For the desktop version, please add the configuration to the existing
configuration path without overwriting the path configuration generated
during installation. Please back up the corresponding file before
modification, so that you can restore it when you make a mistake.

Or you can refer to the default extra_model_paths.yaml.example
for more configuration options. After saving, you need to restart
ComfyUI for the changes to take eﬀect.

Below is the original config example:

Copy

Ask AI

#Rename this to extra_model_paths.yaml and ComfyUI will load it

#config for a1111 ui

#all you have to do is change the base_path to where yours is installed

a111:

    base_path: path/to/stable-diﬀusion-webui/

    checkpoints: models/Stable-diﬀusion

    configs: models/Stable-diﬀusion

    vae: models/VAE

    loras: |

         models/Lora

         models/LyCORIS

    upscale_models: |

                  models/ESRGAN

                  models/RealESRGAN

                  models/SwinIR

    embeddings: embeddings

    hypernetworks: models/hypernetworks

    controlnet: models/ControlNet

#config for comfyui

#your base path should be either an existing comfy install or a central
folder where you store all of your models, loras, etc.

#comfyui:

#     base_path: path/to/comfyui/

#     # You can use is_default to mark that these folders should be listed
first, and used as the default dirs for eg downloads

#     #is_default: true

#     checkpoints: models/checkpoints/

#     clip: models/clip/

#     clip_vision: models/clip_vision/

#     configs: models/configs/

#     controlnet: models/controlnet/

#     diﬀusion_models: |

#                  models/diﬀusion_models

#                  models/unet

#     embeddings: models/embeddings/

#     loras: models/loras/

#     upscale_models: models/upscale_models/

#     vae: models/vae/

#other_ui:

#    base_path: path/to/ui

#    checkpoints: models/checkpoints

#    gligen: models/gligen

#    custom_nodes: path/custom_nodes

For example, if your WebUI is located at D:\stable-diﬀusion-
webui\, you can modify the corresponding configuration to

Copy

Ask AI

a111:

    base_path: D:\stable-diﬀusion-webui\

    checkpoints: models/Stable-diﬀusion

    configs: models/Stable-diﬀusion

    vae: models/VAE

    loras: |

         models/Lora

         models/LyCORIS

    upscale_models: |

                  models/ESRGAN

                  models/RealESRGAN

                  models/SwinIR

    embeddings: embeddings

    hypernetworks: models/hypernetworks

    controlnet: models/ControlNet

Add Extra Custom Nodes Path

Besides adding external models, you can also add custom nodes
paths that are not in the default path of ComfyUI

Please note that this will not change the default installation path of custom
nodes, but will add an extra path search when starting ComfyUI. You still
need to complete the installation of custom node dependencies in the
corresponding environment to ensure the integrity of the running
environment.

Below is a simple configuration example (MacOS), please modify
it according to your actual situation and add it to the
corresponding configuration file, save it and restart ComfyUI for
the changes to take eﬀect:

Copy

Ask AI

my_custom_nodes:

  custom_nodes: /Users/your_username/Documents/extra_custom_nodes

File size

Models can be extremely large files relative to image files. A
typical uncompressed image may require a few megabytes of
disk storage. Generative AI models can be tens of thousands of
times larger, up to tens of gigabytes per model. They take up a
great deal of disk space and take a long time to transfer over a
network.

Model training and refinement

A generative AI model is created by training a machine learning
program on a very large set of data, such as pairs of images and
text descriptions. An AI model doesn’t store the training data

explicitly, but rather it stores the correlations that are implicit
within the data.

Organizations and companies such as Stability AI and Black
Forest Labs release “base” models that carry large amounts of
generic information. These are general purpose generative AI
models. Commonly, the base models need to be refined in order
to get high quality generative outputs. A dedicated community of
people work to refine the base models. The new, refined models
produce better output, provide new or diﬀerent functionality, and/
or use fewer resources. Refined models can usually be run on
systems with less computing power and/or memory.

Auxiliary models

Model functionality can be extended with auxiliary models. For
example, art directing a text-to-image workflow to achieve a
specific result may be diﬃcult or impossible using a diﬀusion
model alone. Additional models can refine a diﬀusion model
within the workflow graph to produce desired results. Examples
include LoRA (Low Rank Adaptation), a small model that is
trained on a specific subject; ControlNet, a model that helps
control composition using a guide image; and Inpainting, a model
that allows certain diﬀusion models to generate new content
within an existing image.

_____________________________________
_____________________________________
_____________________________________
Basic Concepts

Dependencies

Understand dependencies in ComfyUI

A workflow file depends on other files

We often obtain various workflow files from the community, but frequently find that the
workflow cannot run directly after loading. This is because a workflow file depends on
other files besides the workflow itself, such as media asset inputs, models, custom

nodes, related Python dependencies, etc. ComfyUI workflows can only run normally
when all relevant dependencies are satisfied.

ComfyUI workflow dependencies mainly fall into the following categories:

• Assets (media files including audio, video, images, and other inputs)

• Custom nodes

• Python dependencies

• Models (such as Stable Diﬀusion models, etc.)

Assets

An AI model is an example of an asset. In media production, an asset is some media
file that supplies input data. For example, a video editing program operates on movie
files stored on disk. The editing program’s project file holds links to these movie file
assets, allowing non-destructive editing that doesn’t alter the original movie files.

ComfyUI works the same way. A workflow can only run if all of the required assets are
found and loaded. Generative AI models, images, movies, and sounds are some
examples of assets that a workflow might depend upon. These are therefore known as
dependent assets or asset dependencies.

Custom Nodes

Custom nodes are an important component of ComfyUI that extend its functionality.
They are created by the community and can be installed to add new capabilities to
your workflows.

Python Dependencies

ComfyUI is a Python-based project. We build a standalone Python environment to run
ComfyUI, and all related dependencies are installed in this isolated Python
environment.

ComfyUI Dependencies

You can view ComfyUI’s current dependencies in the requirements.txt file:

Copy

Ask AI

comfyui-frontend-package==1.14.5

torch

torchsde

torchvision

torchaudio

numpy>=1.25.0

einops

transformers>=4.28.1

tokenizers>=0.13.3

sentencepiece

safetensors>=0.4.2

aiohttp>=3.11.8

yarl>=1.18.0

pyyaml

Pillow

scipy

tqdm

psutil

#non essential dependencies:

kornia>=0.7.1

spandrel

soundfile

av

As ComfyUI evolves, we may adjust dependencies accordingly, such as adding new
dependencies or removing ones that are no longer needed. So if you use Git to update
ComfyUI, you need to run the following command in the corresponding environment
after pulling the latest updates:

Copy

Ask AI

pip install -r requirements.txt

This ensures that ComfyUI’s dependencies are up to date for proper operation. You can
also modify specific package dependency versions to upgrade or downgrade certain
dependencies.

Additionally, ComfyUI’s frontend ComfyUI_frontend is currently maintained as a
separate project. We update the comfyui-frontend-package dependency version after
the corresponding version stabilizes. If you need to switch to a diﬀerent frontend
version, you can check the version information here.

Custom Node Dependencies

Thanks to the eﬀorts of many authors in the ComfyUI community, we can extend
ComfyUI’s functionality by using diﬀerent custom nodes, enabling impressive creativity.

Typically, each custom node has its own dependencies and a separate
requirements.txt file. If you use ComfyUI Manager to install custom nodes, ComfyUI
Manager will usually automatically install the corresponding dependencies.

There are also cases where you need to install dependencies manually. Currently, all
custom nodes are installed in the ComfyUI/custom_nodes directory.

You need to navigate to the corresponding plugin directory in your ComfyUI Python
environment and run pip install -r requirements.txt to install the dependencies.

If you’re using the Windows Portable version, you can use the following command in
the ComfyUI_windows_portable directory:

Copy

Ask AI

python_embeded\python.exe -m pip install -r
ComfyUI\custom_nodes\<custom_node_name>\requirements.txt

to install the dependencies for the corresponding node.

Dependency Conflicts

Dependency conflicts are a common issue when using ComfyUI. You might find that
after installing or updating a custom node, previously installed custom nodes can no
longer be found in ComfyUI’s node library, or error pop-ups appear. One possible
reason is dependency conflicts.

There can be many reasons for dependency conflicts, such as:

1. Custom node version locking

Some plugins may fix the exact version of a dependency library (e.g.,
open_clip_torch==2.26.1), while other plugins may require a higher version (e.g.,
open_clip_torch>=2.29.0), making it impossible to satisfy both version requirements
simultaneously.

Solution: You can try changing the fixed version dependency to a range constraint,
such as open_clip_torch>=2.26.1, and then reinstall the dependencies to resolve these
issues.

2. Environment pollution

During the installation of custom node dependencies, it may overwrite versions of
libraries already installed by other plugins. For example, multiple plugins may depend
on PyTorch but require diﬀerent CUDA versions, and the later installed plugin will break
the existing environment.

Solutions:

• You can try manually installing specific versions of dependencies in the Python
virtual environment to resolve such issues.

• Or create diﬀerent Python virtual environments for diﬀerent plugins to resolve
these issues.

• Try installing plugins one by one, restarting ComfyUI after each installation to
observe if dependency conflicts occur.

3. Custom node dependency versions incompatible with ComfyUI dependency
versions

These types of dependency conflicts may be more diﬃcult to resolve, and you may
need to upgrade/downgrade ComfyUI or change the dependency versions of custom
nodes to resolve these issues.

Solution: These types of dependency conflicts may be more diﬃcult to resolve, and
you may need to upgrade/downgrade ComfyUI or change the dependency versions of
custom nodes to resolve these issues.

Models

Models are a significant asset dependency for ComfyUI. Various custom nodes and
workflows are built around specific models, such as the Stable Diﬀusion series, Flux
series, Ltxv, and others. These models are an essential foundation for creation with
ComfyUI, so we need to ensure that the models we use are properly available.
Typically, our models are saved in the corresponding directory under ComfyUI/models/.
Of course, you can also create an extra_model_paths.yaml by modifying the template
to make additional model paths recognized by ComfyUI. This allows multiple ComfyUI
instances to share the same model library, reducing disk usage.

Software

An advanced application like ComfyUI also has software dependencies. These are
libraries of programming code and data that are required for the application to run.
Custom nodes are examples of software dependencies. On an even more fundamental
level, the Python programming environment is the ultimate dependency for ComfyUI.
The correct version of Python is required to run a particular version of ComfyUI.
Updates to Python, ComfyUI, and custom nodes can all be handled from the ComfyUI
Manager window.

_____________________________________
_____________________________________
_____________________________________
Interface Guide

Mask Editor - Create and Edit Masks in ComfyUI

Learn how to use the Mask Editor in ComfyUI, including settings and usage
instructions

The Mask Editor is a very useful feature in ComfyUI that allows users to create and edit
masks within images without needing to use other applications.

The Mask Editor is currently triggered through the Load Image node. After uploading
an image, you can right-click on the node and select Open in MaskEditor from the
menu to open the Mask Editor.

You can then click with your mouse on the image to create and edit masks.

Video Tutorial

Your browser does not support the video tag.

_____________________________________
_____________________________________
_____________________________________

Interface Guide

Templates - ComfyUI Built-in Workflow Templates

Templates provide model workflows natively supported by ComfyUI and example
workflows from custom nodes. You can find and use workflows for currently supported
models here.

Workflow Templates is the browser for ComfyUI’s natively supported model workflows
and also some example workflows from custom nodes.

In ComfyUI’s Workflow Templates, you can find:

• Natively supported model workflows

• Example workflows from custom nodes

How to open Templates in ComfyUI

Open via the menu Workflow —> Browse Workflow Templates.

How to use templates

1. Load a template: Click any template you want to load its workflow.

2. Download models: When loading a template, ComfyUI automatically checks
whether all required model files exist. If anything is missing, it will prompt you to
download the models.

3. Run the workflow: Once all requirements—such as models, input images, and
prompts—are ready, click the Run button to start using the workflow.

Model storage location

Each workflow template embeds links to the required models. On first use, if the
corresponding model files are not detected, you will see a download prompt.

1. For desktop version, when you click the Download button, the desktop program
will automatically download the model files for you.

2. For other versions, the browser will be used to download the corresponding
model. You need to download the model and save it to the corresponding folder
under ComfyUI/models. For example, the model in the screenshot should be
saved in the following location:

Copy

Ask AI

📂  ComfyUI/

├── 📂  models/

│   ├── 📂  diﬀusion_models/

│   │   └── qwen_image_fp8_e4m3fn.safetensors

│   ├── 📂  vae/

│   │   └── qwen_image_vae.safetensors

│   └── 📂  text_encoders/

│       └── qwen_2.5_vl_7b_fp8_scaled.safetensors

In the current version, missing-file detection only checks whether there is a file with the
same name in the corresponding top-level directory. For example, the file must exist
directly under ComfyUI/models/diﬀusion_models. If you have already downloaded the
model into a subfolder such as ComfyUI/models/diﬀusion_models/wan_video, you can
ignore the popup and simply ensure the correct model is selected in the corresponding
model loader node.

If you’re curious how model links are embedded, we add a models field under the
node’s properties. Below is a complete snippet of a DualCLIPLoader node with
embedded model information:

Copy

Ask AI

    {

      "id": 40,

      "type": "DualCLIPLoader",

      "pos": [

        -320,

        290

      ],

      "size": [

        270,

        130

      ],

      "flags": {},

      "order": 0,

      "mode": 0,

      "inputs": [],

      "outputs": [

        {

          "name": "CLIP",

          "type": "CLIP",

          "links": [

            64

          ]

        }

      ],

      "properties": {

        "Node name for S&R": "DualCLIPLoader",

        "cnr_id": "comfy-core",

        "ver": "0.3.40",

        "models": [

          {

            "name": "clip_l.safetensors",

            "url": "https://huggingface.co/comfyanonymous/flux_text_encoders/resolve/
main/clip_l.safetensors",

            "directory": "text_encoders"

          },

          {

            "name": "t5xxl_fp16.safetensors",

            "url": "https://huggingface.co/comfyanonymous/flux_text_encoders/resolve/
main/t5xxl_fp16.safetensors",

            "directory": "text_encoders"

          }

        ]

      },

      "widgets_values": [

        "clip_l.safetensors",

        "t5xxl_fp16.safetensors",

        "flux",

        "default"

      ]

    }

The models field inside properties includes name, url, and directory.

• 	 name: the model file name

• 	 url: a direct download link to the file (not a repository page)

• 	 directory: which subfolder under ComfyUI/models to store the file, e.g.
vae means ComfyUI/models/vae

Currently, only links from Hugging Face and Civitai are supported. The model format
must be a safe format such as .safetensors or .sft. Formats like .gguf are considered
unsafe; when embedded they will be flagged as unsafe and the link will not be shown.

You can use this tool to edit the model information in workflow templates. At the
moment, @ComfyUI-Wiki only adds support for native nodes.

How to update templates?

Templates are managed and updated as a separate dependency: comfyui-workflow-
templates.

If, after updating ComfyUI, you don’t see the documentation or newly announced
templates, you may need to update the corresponding dependency. You can check
versions in ComfyUI/requirements.txt.

Typically, the following three dependencies may be upgraded together when ComfyUI
is updated:

Copy

Ask AI

comfyui-frontend-package==1.24.4

comfyui-workflow-templates==0.1.52

comfyui-embedded-docs==0.2.4

If you’re not sure how to update correctly, see Update ComfyUI for how to update
ComfyUI and its dependencies.

How to contribute templates to the ComfyUI repository?

All templates are hosted in the workflow_templates repository. You can contribute
templates by submitting a PR. For oﬃcial templates, we require the following:

1. Do not use any third-party nodes (to avoid extra installations for users who lack
those nodes).

2. The template must not duplicate existing ones and should target supported
model capabilities.

3. You may open an issue in the repository to ask questions.

Custom node templates

If a custom node author provides templates and example workflows, you can also find
them in the Templates browser. Usually, you can locate all templates by finding the
category named after the node.

If you are a custom node author, note that we currently only support a single directory
level under the templates folder (no nested subdirectories), and only JSON-format
templates are supported.

How to add templates for custom nodes?

See Custom Node Templates for how to add workflow templates for your custom
nodes.

_____________________________________
_____________________________________
_____________________________________
Interface Guide

Subgraph - Simplify your workflow

An introduction to the Subgraph feature in ComfyUI, including how to create, navigate,
and manage subgraphs.

The subgraph feature requires ComfyUI frontend version 1.24.3 or later. If you don’t see
this feature, please refer to: How to Update ComfyUI

• 	Images in this document are made with nightly version frontend, please refer to
the actual interface

• 	Some features like converting subgraph back to nodes will be supported in the
future

Comfy Org

5.7K subscribers

Subgraph Oﬃcial Release! Making Complex Workflows Clean and Eﬃcient

Share

Watch on

A subgraph is a powerful ComfyUI feature that lets you package complex workflows
into a single reusable subgraph node, making them easier to manage and share.

Think of a subgraph as a “folder” for your workflow – you can group related nodes
together and use the entire collection as one unified subgraph node.

Use subgraphs to:

• Simplify complex workflows

• Reuse common node combinations

• Build more eﬃcient workflows with modular components

Creating a Subgraph

1

Select nodes

Select the nodes you want to group in ComfyUI

2

Click the subgraph icon

Find the subgraph icon in the toolbar

3

Subgraph created

ComfyUI automatically creates a subgraph based on your selected nodes’ inputs and
outputs

4

Customize your subgraph

Refer to Editing Subgraphs, you can edit and organize the subgraph to create a fully
functional node

Working with Subgraphs

Basic Operations

Subgraphs work just like regular nodes. You can:

• Change colors and names

• Use bypass to disable

• Apply all standard node operations

Editing Subgraphs

To enter edit mode:

• Double-click the empty area inside the subgraph (not on widgets), or

• Click the subgraph edit button

In edit mode you’ll see:

1. 	Navigation bar: Exit the current subgraph and return to the parent level

2. 	Input slots: Internal node inputs exposed to the outside

• 	Connect outputs to slots like normal nodes

• 	Right-click connection points to rename/delete exposed slots

3. 	Output slots: Outputs exposed to the outside (same functionality as input slots)

Working with slots:

1. Default slot (labeled 1): Use this to add new input/output connections

2. Right-click existing slots to rename, delete, or disconnect from original nodes

Note: Slot connections follow standard data type validation rules

Nested Subgraphs

Create even more complex workflows by nesting subgraphs within subgraphs.

The navigation bar shows your current level and lets you easily move between nested
subgraphs.

_____________________________________
_____________________________________
_____________________________________
Interface Guide

Partial Execution - Run Only Part
of Your workflow in ComfyUI

How to use and the requirements for the Partial Execution
feature in ComfyUI

The Partial Execution feature is located in the ComfyUI node
selection toolbox. It allows you to run only a part of your
workflow instead of executing all nodes. This feature is only
available when the selected node is an output node, and when
available, it appears as a green triangle icon.

What is Partial Execution?

Partial Execution, as the name suggests, lets you run only a part
of your workflow instead of executing all nodes in the workflow.

The diagram above compares Partial Execution and running the
entire workflow:

1. Partial Execution (left): Only runs the branch of the workflow
from the starting node to the output node.

2. Run Workflow (right): Runs all nodes in the workflow.

This feature allows you to flexibly execute specific parts of your
workflow, rather than running the entire workflow every time.

How to Use the Partial Execution Feature?

To use the Partial Execution feature, the currently selected node
must be an output node, such as preview or save nodes. When
the corresponding node meets the criteria, after selecting the
node, the button in the toolbox will display as a green triangle
icon. Click this icon to run the partial workflow.

Common Issues

Q: Why do all nodes run when I use this feature? A: Please
ensure your ComfyUI frontend version is after v1.23.4, or
possibly requires v1.24.x version. The corresponding bug was
fixed around version 1.24.x, so please update your ComfyUI to
the latest version to ensure the frontend version meets the
requirements.

_____________________________________
_____________________________________
_____________________________________
ComfyUI Settings

ComfyUI Settings Overview

Detailed description of ComfyUI settings overview

This section covers detailed setting descriptions in the ComfyUI
frontend settings menu. All user settings are automatically saved
to the ComfyUI/user/default/comfy.settings.json file.

You can use the Ctrl + , keyboard shortcut to open the settings
panel, then click on the corresponding setting options to
configure them.

Since custom nodes can also register corresponding setting
categories in the menu, our oﬃcial documentation currently only
includes native setting content. Additionally, some setting options
are only eﬀective for ComfyUI Desktop, which we have noted on
the corresponding pages.

ComfyUI Settings Menu

# Table of Contents



1. User - User settings related to ComfyUI account, mainly used
for logging into ComfyUI account to use API nodes

2. Credits - Entry for purchasing credits and credit balance
history, only visible after logging into ComfyUI account

3. Comfy - Detailed description of ComfyUI core setting options

4. Lite Graph - Detailed description of Canvas (Lite Graph) setting
options in ComfyUI

5. Appearance - Modify ComfyUI appearance options such as
themes, background colors, sidebar position, etc.

6. Extension - Manage the enable/disable status of frontend
extension plugins in ComfyUI

7. 3D - Some setting options for 3D node initialization

8. Comfy Desktop - Desktop update settings, mirror settings, etc.
(only eﬀective for ComfyUI Desktop)

9. Mask Editor - Adjust mask editor usage preferences

10. Keybinding - Modify ComfyUI keyboard shortcut settings

12. About - Learn about current ComfyUI version information,
device runtime information, etc., which is very useful for daily
feedback

13. Server Config

Modify ComfyUI configuration file, this setting is only eﬀective for ComfyUI
Desktop

# Section: User

ComfyUI Settings

Account Management

In this document, we will introduce the account management features of ComfyUI,
including account login, registration, and logout operations.

The account system was added to support API Nodes, which enable calls to closed-
source model APIs, greatly expanding the possibilities of ComfyUI. Since these API
calls consume tokens, we have added a corresponding user system.

Currently, we support the following login methods:

• Email login

• Google login

• Github login

• API Key login (for non-whitelisted site authorization)

We will provide relevant login requirements and explanations in this document.

ComfyUI Version Requirements

You may need to use at least ComfyUI v0.3.0 to use the account system. Ensure that
the corresponding frontend version is at least 1.17.11. Sometimes the frontend may fail
to install and revert to an older version, so please check if the frontend version is
greater than 1.17.11 in Settings -> About.

In some regions, network restrictions may prevent normal access to the login API,
causing timeouts or failures. Before logging in, please ensure that your network
environment does not restrict access to the corresponding API, and make sure you can
access sites like Google or Github.

Since we are still in rapid iterative updates, related functions may change. If there are
no special circumstances, please try to update to the latest version to get support for
relevant functions.

Network Requirements

To login to ComfyUI account, you must be in a secure network environment:

• 	Only allow access from 127.0.0.1 or localhost.

• 	Do not support using the --listen parameter to access the API node through a
local network.

• 	If you are using a non-SSL certificate or a site that does not start with https, you
may not be able to successfully log in.

• 	You may not be able to log in on a site that is not in our whitelist (but you can log
in using an API Key now).

• 	Ensure you can connect to our service normally (some regions may require a
proxy).

How to Log In

Log in via Settings -> User:

Login Methods

If this is your first login, please create an account first.

Logging in with an API Key

Since not all ComfyUI deployments are on our domain authorization whitelist, we have
provided API Key login in a recent update (2025-05-10) for logging in through non-
whitelisted sites. Below are the steps for logging in with an API Key:

• 	Have an API Key

• 	No API Key, Apply for an API Key First

1

Select Comfy API Key Login on the Login Screen

Select Comfy API Key login in the login popup

2

Enter Your API Key

1. Enter your API Key and save it

2. If you don’t have an API Key, click the Get one here link to go to https://
platform.comfy.org/login and log in to obtain it.

3

Login Successful

After a successful login, you can see the corresponding API Key login information in
the settings menu

Post-Login Status

After logging in, a login button is displayed in the top menu bar of the ComfyUI
interface. You can open the corresponding login interface through this button and log
out of the corresponding account in the settings menu.

##Frequently Asked Questions (FAQs)

Q: Are there any login device restrictions?

A: We do not restrict login devices. You can log in to your account on any device, but
please note that your account information may be accessed by other devices, so do
not log in to your account on public devices.

Q: How to log in in a LAN environment?

A: Currently, only API Key login is supported in a LAN environment. If you are
accessing ComfyUI services through a LAN, please use API Key to log in.

Q: Why can't I log in on some websites?

A: Our login service has a whitelist, so you may not be able to log in to ComfyUI
deployed on some servers, for this case, you can use API Key login to solve it.

# Section: Credits

ComfyUI Settings

Credits Management

In this article, we will introduce ComfyUI’s credit management features, including how
to obtain, use, and view credits.

The credit system was added to support the API Nodes, as calling closed-source AI
models requires token consumption, so proper credit management is necessary. By
default, the credits interface is not displayed. Please first log in to your ComfyUI
account in Settings -> User, and then you can view your associated account’s credit
information in Settings -> Credits.

ComfyUI will always remain fully open-source and free for local users.

How to Purchase Credits?

Below is a demonstration video for purchasing credits:

Detailed steps are as follows:

1

Log in to your ComfyUI account

Log in to your ComfyUI account in Settings -> User

2

Go to `Settings` -> `Credits` to purchase credits

After logging in, you should see the Credits option added to the menu

Go to Settings -> Credits to purchase credits

3

Set the amount of credits to purchase

In the popup, set the purchase amount and click the Buy button

4

Make payment through Stripe

On the payment page, please follow these steps:

1. Select the currency for payment

2. Confirm that the email is the same as your ComfyUI registration email

3. Choose your payment method

• Credit Card

• WeChat (only supported when paying in USD)

• Alipay (only supported when paying in USD)

4. Click the Pay button or the Generate QR Code button to complete the payment
process

5

Complete payment and check your credit balance

After completing the payment, please return to Menu -> Credits to check if your
balance has been updated. Try refreshing the interface or restarting if necessary

## Frequently Asked Questions (FAQs)

Q: Can credits go negative?

A: No, when your credit balance is negative, you will not be able to run API Nodes

Q: Can I get a refund for unused credits?

A: Currently, we do not support refunds

Q: How do I check my current balance and usage?

A: Click on Settings -> Credits to see your current balance and access the Credit
History entry

Q: Can I share my credits with other users?

A: You can log into the same account on multiple devices, but we do not support
sharing credits with other users

Q: How do I know how many credits I've consumed each time?

A: Due to diﬀerent image sizes and generation quantities, the Tokens and Credits
consumed each time vary. In Settings -> Credits, you can see the credits consumed
each time and the corresponding credit history

Q: Why don't I see WeChat or Alipay payment options?

A: Please ensure you are paying in USD, as WeChat and Alipay are only supported
when paying in USD

# Section: Comfy

ComfyUI Settings

Comfy Settings

Detailed description of ComfyUI core setting options

API Nodes

Show API node pricing badge

• 	Default Value: Enabled

• 	Function: Controls whether to display pricing badges on API nodes, helping
users identify the usage cost of API nodes

For more information about API nodes, please refer to API Nodes

Dev Mode

Enable dev mode options (API save, etc.)

• 	Default Value: Disabled

• 	Function: Enables development mode options (such as API save, etc.)

Edit Token Weight

Ctrl+up/down precision

• 	Default Value: 0.01

• 	Function: When using CLIPTextEncode type nodes or text input node widgets,
use Ctrl+up/down to quickly adjust weights. This option changes the weight
value for each adjustment

Locale

Language

• 	Options: English, 中⽂ (Chinese),⽇本語 (Japanese), 한국어 (Korean), Русский
(Russian), Español (Spanish), Français (French)

• 	Default Value: Auto-detect browser language

• 	Function: Modify the display language of ComfyUI interface

Menu

Use new menu

• 	Default Value: Top

• 	Function: Select menu interface and position, currently only supports Top,
Bottom, Disabled

• 	Top

• 	Bottom

• 	Disabled

The menu interface will be displayed at the top of the workspace

Model Library

Model Library refers to the model management function in the ComfyUI sidebar menu.
You can use this function to view models in your ComfyUI/models and additionally
configured model folders.

What name to display in the model library tree view

• 	Default Value: title

• 	Function: Select the name format to display in the model library tree view,
currently only supports filename and title

Automatically load all model folders

• 	Default Value: Disabled

• 	Function: Whether to automatically detect model files in all folders when clicking
the model library. Enabling may cause loading delays (requires traversing all
folders). When disabled, files in the corresponding folder will only be loaded
when clicking the folder name.

Node

During the iteration process of ComfyUI, we will adjust some nodes and enable some
nodes. These nodes may undergo major changes or be removed in future versions.
However, to ensure compatibility, deprecated nodes have not been removed. You can
use the settings below to enable whether to display experimental nodes and
deprecated nodes.

Show deprecated nodes in search

• 	Default Value: Disabled

• 	Function: Controls whether to display deprecated nodes in search. Deprecated
nodes are hidden by default in the UI, but remain eﬀective in existing workflows.

Show experimental nodes in search

• 	Default Value: Enabled

• 	Function: Controls whether to display experimental nodes in search.
Experimental nodes are some new feature support, but are not fully stable and
may change or be removed in future versions.

Node Search Box

Number of nodes suggestions

• 	Default Value: 5

• 	Function: Used to modify the number of recommended nodes in the related
node context menu. The larger the value, the more related recommended nodes
are displayed.

Show node frequency in search results

• 	Default Value: Disabled

• 	Function: Controls whether to display node usage frequency in search results

Show node id name in search results

• 	Default Value: Disabled

• 	Function: Controls whether to display node ID names in search results

Show node category in search results

• 	Default Value: Enabled

• 	Function: Controls whether to display node categories in search results, helping
users understand node classification information

Node preview

• 	Default Value: Enabled

• 	Function: Controls whether to display node previews in search results, making it
convenient for you to quickly preview nodes

Node search box implementation

• 	Default Value: default

• 	Function: Select the implementation method of the node search box
(experimental feature). If you select litegraph (legacy), it will switch to the early
ComfyUI search box

Node Widget

Widget control mode

• 	Options: before, after

• 	Function: Controls whether the timing of node widget value updates is before or
after workflow execution, such as updating seed values

Textarea widget spellcheck

• 	Default Value: Disabled

• 	Function: Controls whether text area widgets enable spellcheck, providing
spellcheck functionality during text input. This functionality is implemented
through the browser’s spellcheck attribute

Queue

Queue history size

• 	Default Value: 100

• 	Function: Controls the queue history size recorded in the sidebar queue history
panel. The larger the value, the more queue history is recorded. When the
number is large, loading the page will also consume more memory

Queue Button

Batch count limit

• 	Default Value: 100

• 	Function: Sets the maximum number of tasks added to the queue in a single
click, preventing accidentally adding too many tasks to the queue

Validation

Validate node definitions (slow)

• 	Default Value: Disabled

• 	Function: Controls whether to validate all node definitions at startup (slow). Only
recommended for node developers. When enabled, the system will use Zod
schemas to strictly validate each node definition. This functionality will consume
more memory and time

• 	Error Handling: Failed node definitions will be skipped and warning information
will be output to the console

Since detailed schema validation needs to be performed on all node definitions, this
feature will significantly increase startup time, so it is disabled by default and only
recommended for node developers

Validate workflows

• 	Default Value: Enabled

• 	Function: Ensures the structural and connection correctness of workflows. If
enabled, the system will call useWorkflowValidation().validateWorkflow() to
validate workflow data

• 	Validation Process: The validation process includes two steps:

• 	Schema validation: Use Zod schemas to validate workflow structure

• 	Link repair: Check and repair connection issues between nodes

• 	Error Handling: When validation fails, error prompts will be displayed, but
workflow loading will not be blocked

Window

Show confirmation when closing window

• 	Default Value: Enabled

• 	Function: When there are modified but unsaved workflows, controls whether to
display confirmation when closing the browser window or tab, preventing
accidental window closure that leads to loss of unsaved workflows

Workflow

Persist workflow state and restore on page (re)load

• 	Default Value: Enabled

• 	Function: Controls whether to restore workflow state on page (re)load,
maintaining workflow content after page refresh

Auto Save

• 	Default Value: oﬀ

• 	Function: Controls the auto-save behavior of workflows, automatically saving
workflow changes to avoid data loss

Auto Save Delay (ms)

• 	Default Value: 1000

• 	Function: Sets the delay time for auto-save, only eﬀective when auto-save is set
to “after delay”

Show confirmation when deleting workflows

• 	Default Value: Enabled

• 	Function: Controls whether to display a confirmation dialog when deleting
workflows in the sidebar, preventing accidental deletion of important workflows

Save and restore canvas position and zoom level in workflows

• 	Default Value: Enabled

• 	Function: Controls whether to save and restore canvas position and zoom level
in workflows, restoring the previous view state when reopening workflows

Opened workflows position

• 	Options: Sidebar, Topbar, Topbar (Second Row)

• 	Default Value: Topbar

• 	Function: Controls the display position of opened workflow tabs, currently only
supports Sidebar, Topbar, Topbar (Second Row)

Prompt for filename when saving workflow

• 	Default Value: Enabled

• 	Function: Controls whether to prompt for filename input when saving workflows,
allowing users to customize workflow filenames

Sort node IDs when saving workflow

• 	Default Value: Disabled

• 	Function: Determines whether to sort node IDs when saving workflows, making
workflow file format more standardized and convenient for version control

Show missing nodes warning

• 	Default Value: Enabled

• 	Function: Controls whether to display warnings for missing nodes in workflows,
helping users identify unavailable nodes in workflows

Show missing models warning

• 	Default Value: Enabled

• 	Function: We support adding model link information to widget values in
workflow files for prompts when loading model files. When enabled, if you don’t
have the corresponding model files locally, warnings for missing models in
workflows will be displayed

Require confirmation when clearing workflow

• 	Default Value: Enabled

• 	Function: Controls whether to display a confirmation dialog when clearing
workflows, preventing accidental clearing of workflow content

Save node IDs to workflow

• 	Default Value: Enabled

• 	Function: Controls whether to save node IDs when saving workflows, making
workflow file format more standardized and convenient for version control

# Section: Lite Graph

ComfyUI Settings

ComfyUI LiteGraph (Canvas) Settings

Detailed description of ComfyUI graphics rendering engine LiteGraph setting options

LiteGraph is the underlying graphics rendering engine of ComfyUI. The settings in this
category mainly control the behavior and appearance of graphical interfaces such as
canvas, nodes, and links.

Canvas

Show selection toolbox

• 	Default Value: Enabled

• 	Function: The selection toolbox is a floating quick action toolbar that appears on
nodes after they are selected, providing common quick operations such as
partial execution, pinning, deletion, color modification, etc.

Low quality rendering zoom threshold

• 	Default Value: 0.6

• 	Range: 0.1 - 1.0

• 	Function: When rendering the interface, especially when the workflow is
particularly complex and the entire canvas is particularly large, the frontend
rendering of corresponding elements will consume a lot of memory and cause
lag. By lowering this threshold, you can control elements to enter low quality
rendering mode when scaled to a specific percentage, thereby reducing memory
consumption. The corresponding diﬀerent rendering modes are shown below

Maximum FPS

• 	Default Value: 0 (use screen refresh rate)

• 	Range: 0 - 120

• 	Function: Limits the rendering frame rate of the canvas. 0 means using the
screen refresh rate. Higher FPS will make the canvas rendering smoother, but
will also consume more performance. Too low values will cause more obvious
stuttering.

Always snap to grid

• 	Default Value: Disabled

• 	Function: When this option is not enabled, you can hold the Shift key to align
node edges with the grid. When enabled, node edges will automatically align
with the grid without holding the Shift key.

Snap to grid size

• 	Range: 1 - 500

• 	Function: When auto-snap is enabled or when moving nodes while holding the
Shift key, this parameter determines the grid size for snapping. The default value
is 10, and you can adjust it according to your needs.

Enable fast-zoom shortcut (Ctrl + Shift + Drag)

• 	Default Value: Enabled

• 	Function: Enables the Ctrl + Shift + Left Mouse Button Drag fast zoom function,
providing a faster zoom operation method

Show graph canvas menu

• 	Default Value: Enabled

• 	Function: Controls whether to display the canvas menu in the bottom right
corner

The canvas menu is located in the bottom right corner of the entire ComfyUI interface,
containing operations such as canvas zooming, temporarily hiding all connections,
quickly scaling the workflow to fit the canvas, etc., as shown in the image below

Canvas zoom speed

• 	Default Value: 1.1

• 	Range: 1.01 - 2.5

• 	Function: Controls the speed of canvas zooming, adjusts the sensitivity of
mouse wheel zooming

Show canvas info on bottom left corner (fps, etc.)

• 	Default Value: Enabled

• 	Function: Controls whether to display canvas information in the bottom left
corner, showing performance metrics like FPS

Context Menu

Scale node combo widget menus (lists) when zoomed in

• 	Default Value: Enabled

• 	Function: Controls whether to scale node combo widget menus (lists) when
zoomed in, allowing users to select node combo widgets

Graph

Link Render Mode

• 	Default Value: 2 (Spline)

• 	Options: Straight, Linear, Spline, Hidden

• 	Function: Sets the rendering style of connections, controlling the visual style of
links between nodes

Group

This section of settings is mainly related to node group functionality

Double click group title to edit

• 	Default Value: Enabled

• 	Function: Controls whether you can double-click the node title to edit it, allowing
users to rename nodes, marked as part 1 in the image

Group selected nodes padding

• 	Default Value: 10

• 	Range: 0 - 100

• 	Function: Sets the inner padding when grouping selected nodes, controlling the
spacing between the group frame and nodes, marked as the arrow annotation
part 2 in the image

Link

Link midpoint markers

• 	Default Value: Circle

• 	Options: None, Circle, Arrow

• 	Function: Sets the marker style at link midpoints, displaying direction indicators
at link midpoints

Link Release

This menu section currently mainly controls related operations when link connections
are released. The current two related operations are:

A node recommendation list related to the current input/output will appear after release

A search box will be launched after release

Action on link release (Shift)

• 	Default Value: search box

• 	Options: context menu, search box, no action

• 	Function: Sets the action when releasing links while holding the Shift key,
special behavior when releasing links while holding Shift

Action on link release (No modifier)

• 	Default Value: context menu

• 	Options: context menu, search box, no action

• 	Function: Sets the default action when releasing links, controls the behavior
after dragging and releasing links

Node

Always shrink new nodes

• 	Default Value: Enabled

• 	Function: Controls whether to automatically shrink when creating new nodes, so
nodes can always display the minimum size, but may cause some text display to
be truncated when adding, requiring manual adjustment of node size

Enable DOM element clipping (enabling may reduce performance)

• 	Default Value: Enabled

• 	Function: Enables DOM element clipping (may aﬀect performance), optimizes
rendering but may reduce performance

Middle-click creates a new Reroute node

• 	Default Value: Enabled

• 	Function: Creates a new reroute node when middle-clicking, quickly creates
reroute nodes for organizing connections

Keep all links when deleting nodes

• 	Default Value: Enabled

• 	Function: Automatically bypasses connections when deleting intermediate
nodes, attempts to reconnect input and output links when deleting nodes

Snap highlights node

• 	Default Value: Enabled

• 	Function: Highlights nodes when dragging links to them, provides visual
feedback, shows connectable nodes. When enabled, the eﬀect is as shown in
the image below, the corresponding side of the link will display highlighted style

Auto snap link to node slot

• 	Default Value: Enabled

• 	Function: Automatically snaps to available slots when dragging links to nodes,
simplifies connection operations, automatically finds suitable input slots

Enable Tooltips

• 	Default Value: Enabled

• 	Function: Some node information will contain tooltips, including parameter
descriptions, etc. When enabled, these tooltips will be displayed when hovering
the mouse, as shown in the image below

Tooltip Delay

• 	Default Value: 500

• 	Function: Controls the delay time for tooltips, in milliseconds. Setting to 0 means
displaying tooltips immediately

Node life cycle badge mode

• 	Default Value: Show all

• 	Function: Controls the display of node lifecycle markers, showing node status
information

Node ID badge mode

• 	Default Value: Show all

• 	Function: Controls the display of node ID markers, showing node unique
identifiers

Node source badge mode

• 	Options:

• 	None

• 	Hide built-in

• 	Show all

• 	Function: Controls the display mode of node source markers, showing node
source information. The corresponding display eﬀect is shown in the image
below. If show all is selected, it will display labels for both custom nodes and
built-in nodes, making it convenient for you to determine the corresponding
node source. The corresponding fox logo represents ComfyUI built-in nodes

Double click node title to edit

• 	Default Value: Enabled

• 	Function: Controls whether you can double-click the node title to edit it, allowing
users to rename nodes

Node Widget

Float widget rounding decimal places [0 = auto]

• 	Default Value: 0 (auto)

• 	Range: 0 - 6

• 	Function: Sets the decimal places for float widget rounding, 0 means auto,
requires page reload

Disable default float widget rounding

• 	Default Value: Disabled

• 	Function: Controls whether to disable default float widget rounding, requires
page reload, cannot be disabled when the node backend has set rounding

Disable node widget sliders

• 	Default Value: Disabled

• 	Function: Controls whether to disable slider controls in node widgets, forcing
text input instead of sliders

Preview image format

• 	Default Value: Empty string (use original format)

• 	Function: Sets the format for preview images in image widgets, converts to
lightweight formats like webp, jpeg, etc.

Show width × height below the image preview

• 	Default Value: Enabled

• 	Function: Displays width × height information below image previews, showing
image dimension information

Pointer

Enable trackpad gestures

• 	Default Value: Enabled

• 	Function: This setting enables trackpad mode for the canvas, allowing two-
finger pinch zoom and drag.

Double click interval (maximum)

• 	Default Value: 300

• 	Function: Maximum time (milliseconds) between two clicks of a double-click.
Increasing this value helps solve issues where double-clicks are sometimes not
recognized.

Pointer click drift delay

• 	Default Value: 150

• 	Function: Maximum time (milliseconds) to ignore pointer movement after
pressing the pointer button. Helps prevent accidental mouse movement when
clicking.

Pointer click drift (maximum distance)

• 	Default Value: 6

• 	Function: If the pointer moves more than this distance while holding the button,
it is considered a drag (rather than a click). Helps prevent accidental mouse
movement when clicking.

Reroute

Reroute spline oﬀset

• 	Default Value: 20

• 	Function: Used to determine the smoothness of curves on both sides of reroute
nodes. Larger values make curves smoother, smaller values make curves
sharper.

# Section: Appearance

ComfyUI Settings

Customizing ComfyUI Appearance

Learn how to customize the appearance of ComfyUI using color palettes and
advanced CSS options

ComfyUI oﬀers flexible appearance customization options that allow you to personalize
the interface to your preferences.

Color Palette System

The primary way to customize ComfyUI’s appearance is through the built-in color
palette system.

This allows you to:

1. Switch ComfyUI themes

2. Export the currently selected theme as JSON format

3. Load custom theme configuration from JSON file

4. Delete custom theme configuration

For appearance needs that cannot be satisfied by the color palette, you can perform
advanced appearance customization through the user.css file

How to Customize Color Themes

The color palette allows you to modify many specific properties. Here are some of the
most commonly customized elements, with colors represented in hexadecimal format:

1. The JSON comments below are for illustration only. Do not copy the content
below for modification as it will cause the theme to malfunction.

2. Since we are still iterating frequently, the content below may change with
ComfyUI frontend updates. If you need to modify, please export the theme
configuration from settings and then modify it.

Copy

Ask AI

{

  "id": "dark",                     // Must be unique, cannot be the same as other theme IDs

  "name": "Dark (Default)",         // Theme name, displayed in theme selector

  "colors": {

    "node_slot": {                  // Node connection slot color configuration

      "CLIP": "#FFD500",            // CLIP model connection slot color

      "CLIP_VISION": "#A8DADC",     // CLIP Vision model connection slot color

      "CLIP_VISION_OUTPUT": "#ad7452", // CLIP Vision output connection slot color

      "CONDITIONING": "#FFA931",     // Conditioning control connection slot color

      "CONTROL_NET": "#6EE7B7",     // ControlNet model connection slot color

      "IMAGE": "#64B5F6",           // Image data connection slot color

      "LATENT": "#FF9CF9",          // Latent space connection slot color

      "MASK": "#81C784",            // Mask data connection slot color

      "MODEL": "#B39DDB",           // Model connection slot color

      "STYLE_MODEL": "#C2FFAE",     // Style model connection slot color

      "VAE": "#FF6E6E",             // VAE model connection slot color

      "NOISE": "#B0B0B0",           // Noise data connection slot color

      "GUIDER": "#66FFFF",          // Guider connection slot color

      "SAMPLER": "#ECB4B4",         // Sampler connection slot color

      "SIGMAS": "#CDFFCD",          // Sigmas data connection slot color

      "TAESD": "#DCC274"            // TAESD model connection slot color

    },

    "litegraph_base": {             // LiteGraph base interface configuration

      "BACKGROUND_IMAGE": "",        // Background image, default is empty

      "CLEAR_BACKGROUND_COLOR": "#222", // Main canvas background color

      "NODE_TITLE_COLOR": "#999",    // Node title text color

      "NODE_SELECTED_TITLE_COLOR": "#FFF", // Selected node title color

      "NODE_TEXT_SIZE": 14,          // Node text size

      "NODE_TEXT_COLOR": "#AAA",     // Node text color

      "NODE_TEXT_HIGHLIGHT_COLOR": "#FFF", // Node text highlight color

      "NODE_SUBTEXT_SIZE": 12,       // Node subtext size

      "NODE_DEFAULT_COLOR": "#333",   // Node default color

      "NODE_DEFAULT_BGCOLOR": "#353535", // Node default background color

      "NODE_DEFAULT_BOXCOLOR": "#666", // Node default border color

      "NODE_DEFAULT_SHAPE": 2,        // Node default shape

      "NODE_BOX_OUTLINE_COLOR": "#FFF", // Node border outline color

      "NODE_BYPASS_BGCOLOR": "#FF00FF", // Node bypass background color

      "NODE_ERROR_COLOUR": "#E00",    // Node error state color

      "DEFAULT_SHADOW_COLOR": "rgba(0,0,0,0.5)", // Default shadow color

      "DEFAULT_GROUP_FONT": 24,       // Group default font size

      "WIDGET_BGCOLOR": "#222",       // Widget background color

      "WIDGET_OUTLINE_COLOR": "#666", // Widget outline color

      "WIDGET_TEXT_COLOR": "#DDD",    // Widget text color

      "WIDGET_SECONDARY_TEXT_COLOR": "#999", // Widget secondary text color

      "WIDGET_DISABLED_TEXT_COLOR": "#666", // Widget disabled state text color

      "LINK_COLOR": "#9A9",          // Connection line color

      "EVENT_LINK_COLOR": "#A86",    // Event connection line color

      "CONNECTING_LINK_COLOR": "#AFA", // Connecting line color

      "BADGE_FG_COLOR": "#FFF",      // Badge foreground color

      "BADGE_BG_COLOR": "#0F1F0F"    // Badge background color

    },

    "comfy_base": {                  // ComfyUI base interface configuration

      "fg-color": "#ﬀf",            // Foreground color

      "bg-color": "#202020",         // Background color

      "comfy-menu-bg": "#353535",    // Menu background color

      "comfy-menu-secondary-bg": "#303030", // Secondary menu background color

      "comfy-input-bg": "#222",      // Input field background color

      "input-text": "#ddd",          // Input text color

      "descrip-text": "#999",        // Description text color

      "drag-text": "#ccc",           // Drag text color

      "error-text": "#ﬀ4444",       // Error text color

      "border-color": "#4e4e4e",     // Border color

      "tr-even-bg-color": "#222",    // Table even row background color

      "tr-odd-bg-color": "#353535",  // Table odd row background color

      "content-bg": "#4e4e4e",       // Content area background color

      "content-fg": "#ﬀf",          // Content area foreground color

      "content-hover-bg": "#222",    // Content area hover background color

      "content-hover-fg": "#ﬀf",    // Content area hover foreground color

      "bar-shadow": "rgba(16, 16, 16, 0.5) 0 0 0.5rem" // Bar shadow eﬀect

    }

  }

}

Canvas

Background Image

• 	Requirements: ComfyUI frontend version 1.20.5 or newer

• 	Function: Set a custom background image for the canvas to provide a more
personalized workspace. You can upload images or use web images to set the
background for the canvas.

Node

Node Opacity

• 	Function: Set the opacity of nodes, where 0 represents completely transparent
and 1 represents completely opaque.

Node Widget

Textarea Widget Font Size

• 	Range: 8 - 24

• 	Function: Set the font size in textarea widgets. Adjusts the text display size in
text input boxes to improve readability.

Sidebar

Unified Sidebar Width

• 	Function: When enabled, the sidebar width will be unified to a consistent width
when switching between diﬀerent sidebars. If disabled, diﬀerent sidebars can
maintain their custom widths when switching.

Sidebar Size

• 	Function: Control the size of the sidebar, can be set to normal or small.

Sidebar Location

• 	Function: Control whether the sidebar is displayed on the left or right side of the
interface, allowing users to adjust the sidebar position according to their usage
habits.

Tree Explorer

Tree Explorer Item Padding

• 	Function: Set the padding of items in the tree explorer (sidebar panel), adjusting
the spacing between items in the tree structure.

Advanced Customization with user.css

For cases where the color palette doesn’t provide enough control, you can use custom
CSS via a user.css file. This method is recommended for advanced users who need to
customize elements that aren’t available in the color palette system.

Requirements

• ComfyUI frontend version 1.20.5 or newer

Setting Up user.css

1. Create a file named user.css in your ComfyUI user directory (same location as
your workflows and settings - see location details below)

2. Add your custom CSS rules to this file

3. Restart ComfyUI or refresh the page to apply changes

User Directory Location

The ComfyUI user directory is where your personal settings, workflows, and
customizations are stored. The location depends on your installation type:

• 	Desktop - Windows

• 	Desktop - macOS

• 	Desktop - Linux

• 	Manual Install

• 	Portable

Copy

Ask AI

C:\Users\<your username>\AppData\Roaming\ComfyUI\user

This location contains your workflows, settings, and other user-specific files.

After finding the above folder location, please copy the corresponding CSS file to the
corresponding user directory, such as the default user folder being ComfyUI/user/
default, then restart ComfyUI or refresh the page to apply changes.

user.css Examples and Related Instructions

The user.css file is loaded early in the application startup process. So you may need to
use !important in your CSS rules to ensure they override the default styles.

user.css Customization Examples

Copy

Ask AI

/* Increase font size in inputs and menus for better readability */

.comfy-multiline-input, .litecontextmenu .litemenu-entry {

    font-size: 20px !important;

}

/* Make context menu entries larger for easier selection */

.litegraph .litemenu-entry,

.litemenu-title {

  font-size: 24px !important;

}

/* Custom styling for specific elements not available in the color palette */

.comfy-menu {

    border: 1px solid rgb(126, 179, 189) !important;

    border-radius: 0px 0px 0px 10px !important;

    backdrop-filter: blur(2px);

}

Best Practices

1. Start with the color palette for most customizations

2. Use user.css only when necessary for elements not covered by the color palette

3. Export your theme before making significant changes so you can revert if
needed

4. Share your themes with the community to inspire others

## Troubleshooting

Problem: If your color palette changes don’t appear.

Solution: Try refreshing the page

Problem: If CSS customizations didn’t work

Solution: Check that you’re using frontend version 1.20.5+

Problem:

Solution: Try adding !important to user.css rules that aren’t being applied

Problem:

Solution: Keep Backups of your Customizations to easily restore them.

# Section: 3D

ComfyUI Settings

ComfyUI 3D Settings

Detailed description of ComfyUI 3D setting options

This section of settings is mainly used to control the initialization settings of 3D-related
components in ComfyUI, including camera, lighting, scene, etc. When creating new 3D
components, they will be initialized according to these settings. After creation, these
settings can still be adjusted individually.

Camera

Initial Camera Type

• 	Options:

• 	perspective

• 	orthographic

• 	Function: Controls whether the default camera is perspective or orthographic
when creating new 3D components. This default setting can still be switched
individually for each component after creation

Light

The light settings in this section are used to set the default lighting settings for 3D
components. The corresponding settings in the 3D settings in ComfyUI can also be
modified.

Light Adjustment Increment

• 	Default Value: 0.5

• 	Function: Controls the step size when adjusting light intensity in 3D scenes.
Smaller step values allow for finer light adjustments, while larger values make
each adjustment more noticeable

Light Intensity Minimum

• 	Default Value: 1

• 	Function: Sets the minimum light intensity value allowed in 3D scenes. This
defines the lowest brightness that can be set when adjusting the lighting of any
3D control

Light Intensity Maximum

• 	Default Value: 10

• 	Function: Sets the maximum light intensity value allowed in 3D scenes. This
defines the upper limit of brightness that can be set when adjusting the lighting
of any 3D control

Initial Light Intensity

• 	Default Value: 3

• 	Function: Sets the default brightness level of lights in 3D scenes. This value
determines the intensity with which lights illuminate objects when creating new
3D controls, but each control can be adjusted individually after creation

Scene

Initial Background Color

• 	Function: Controls the default background color of 3D scenes. This setting
determines the background appearance when creating new 3D components, but
each component can be adjusted individually after creation

• 	Default Value: 282828 (dark gray)

Change the background color, which can also be adjusted in the canvas.

Initial Preview Visibility

• 	Function: Controls whether the preview screen is displayed by default when
creating new 3D components. This default setting can still be toggled
individually for each component after creation

• 	Default Value: true (enabled)

Initial Grid Visibility

• 	Function: Controls whether the grid is displayed by default when creating new
3D components. This default setting can still be toggled individually for each
component after creation

• 	Default Value: true (enabled)

Hide or show the grid on initialization

# Section: Comfy Desktop

ComfyUI Settings

Comfy Desktop General Settings

Detailed description of ComfyUI Desktop general setting options

General

Window Style

Function: Controls the title bar style of the application window

Automatically check for updates

Function: Automatically checks for ComfyUI Desktop updates and will remind you to
update when updates are available

Send anonymous usage metrics

Function: Sends anonymous usage statistics to help improve the software. Changes to
this setting require a restart to take eﬀect

UV

This section is mainly for users in China, because many of the original mirrors used by
Desktop are outside of China, so access may not be friendly for domestic users. You
can set your own mirror sources here to improve access speed and ensure that
corresponding packages can be accessed and downloaded normally.

Python Install Mirror

Function:

• 	Managed Python installation packages are downloaded from the Astral python-
build-standalone project

• 	Can set mirror URL to use diﬀerent Python installation sources

• 	The provided URL will replace the default GitHub download address

• 	Supports using file:// protocol to read distribution packages from local
directories

Validation: Automatically checks mirror reachability

Pypi Install Mirror

Function: Default pip package installation mirror source

Torch Install Mirror

Function: PyTorch-specific pip installation mirror source

# Section: Mask Editor

ComfyUI Settings

ComfyUI Mask Editor Settings

Detailed description of ComfyUI mask editor setting options

Brush Adjustment

Brush adjustment speed multiplier

• 	Function: Controls the speed of brush size and hardness changes during
adjustment

• 	Description: Higher values mean faster changes

Lock brush adjustment to dominant axis

• 	Function: When enabled, brush adjustment will only aﬀect size or hardness
based on the direction you move

• 	Description: This feature allows users to more precisely control brush property
adjustments

New Editor

Use new mask editor

• 	Function: Switch to the new brush editor interface

• 	Description: Allows users to switch between new and old editor interfaces

• 	New Editor

• 	Old Editor

The new version has a better UI interface and interaction, with more complete
functionality

# Section: Keybinding

ComfyUI Settings

ComfyUI Keyboard Shortcuts and Custom Settings

Keyboard and mouse shortcuts for ComfyUI and related settings

Currently, ComfyUI supports custom keyboard shortcuts. You can set the shortcuts by
clicking on Settings (gear icon) —> Keybinding.

In the corresponding menu, you can see all the current shortcut settings for ComfyUI.
Click the edit icon before the corresponding command to customize the shortcut.

Below is the current list of shortcuts for ComfyUI, which you can customize as needed.

• 	Windows/Linux

• 	MacOS

Shortcut Command
Ctrl + Enter Queue prompt
Ctrl + Shift  Queue prompt (Front)
+ Enter
Ctrl + Alt +  Interrupt
Enter

Ctrl + Z /  Undo/Redo
Ctrl + Y
Ctrl + S Save workflow
Ctrl + O Load workflow
Ctrl + A Select all nodes
Alt + C Collapse/uncollapse selected nodes
Ctrl + M Mute/unmute selected nodes
Ctrl + B Bypass/unbypass selected nodes
Delete
 Delete selected nodes
Backspace
Backspace Clear workflow
Space Move canvas when holding and moving cursor
Ctrl + Click
 Add clicked node to selection
Shift +
Click
Ctrl + C/ Copy and paste selected nodes (without maintaining
Ctrl + V connections to outputs of unselected nodes)
Ctrl + C/ Copy and paste selected nodes (maintaining connections
Ctrl + Shift  from outputs of unselected nodes to inputs of pasted
+ V nodes)
Shift +  Move multiple selected nodes at the same time
Drag
Ctrl + G Add frame to selected nodes
Ctrl + , Show settings dialog
Alt + = Zoom in (canvas)

Alt + - Zoom out (canvas)
. Fit view to selected nodes
P Pin/unpin selected items
Q Toggle queue sidebar
W Toggle workflow sidebar
N Toggle node library sidebar
M Toggle model library sidebar
Ctrl + ` Toggle log bottom panel
F Toggle focus mode (full screen)
R Refresh node definitions
Double- Quick search for nodes to add
Click LMB
# Section: Extension

ComfyUI Settings

Extension Settings

Detailed description of ComfyUI extension management and setting options

The Extension settings panel is a special management panel in the ComfyUI frontend
settings system, specifically used to manage the enable/disable status of frontend
extension plugins. Unlike Custom Nodes, this panel is only used to manage frontend
extensions registered by custom nodes, not to disable custom nodes themselves.

These frontend extension plugins are used to enhance the ComfyUI experience, such
as providing shortcuts, settings, UI components, menu items, and other features.

Extension status changes require a page reload to take eﬀect:

Extension Settings Panel Features

1. Extension List Management

Displays all registered extensions, including:

• Extension Name

• Core extension identification (displays “Core” label)

• Enable/disable status

2. Search Functionality

Provides a search box to quickly find specific extensions:

3. Enable/Disable Control

Each extension has an independent toggle switch:

4. Batch Operations

Provides right-click menu for batch operations:

• Enable All extensions

• Disable All extensions

• Disable 3rd Party extensions (keep core extensions)

Notes

• Extension status changes require a page reload to take eﬀect

• Some core extensions cannot be disabled

• The system will automatically disable known problematic extensions

• Extension settings are automatically saved to the user configuration file

This Extension settings panel is essentially a “frontend plugin manager” that allows
users to flexibly control ComfyUI’s functional modules.

# Section: About

ComfyUI Settings

About Page

Detailed description of ComfyUI About settings page

The About page is an information display panel in the ComfyUI settings system, used
to show application version information, related links, and system statistics. These
settings can provide us with critical information when you submit feedback or report
issues.

Version Information Badges

The About page displays the following core version information:

• 	ComfyUI Version: Shows the backend ComfyUI version number, linked to the
oﬃcial GitHub repository

• 	ComfyUI_frontend Version: Shows the frontend interface version number, linked
to the frontend GitHub repository

• 	Discord Community: Provides a link to the ComfyOrg Discord server

• 	Oﬃcial Website: Links to the ComfyOrg oﬃcial website

Since the version information here mainly corresponds to stable version information, if
you are using the nightly version, the corresponding commit hash will not be displayed
here. If you are using the nightly version, you can use the git log command in the
corresponding ComfyUI main directory to view the corresponding commit hash and
other information. Another common issue is that diﬀerent dependency packages may
fail and rollback during updates.

Custom Node Badges

If custom nodes are installed, the About page will also display additional badge
information provided by custom nodes. These badges are registered by each custom
node through the aboutPageBadges property.

System Info

The bottom of the page displays detailed system statistics, including:

• Hardware configuration information

• Software environment information

• System performance data

Extension Developer Guide

Extension developers can add custom badges to the About page by adding the
aboutPageBadges property to their extension configuration:

Copy

Ask AI

app.registerExtension({

  name: 'MyExtension',

  aboutPageBadges: [

    {

      label: 'My Extension v1.0.0',

      url: 'https://github.com/myuser/myextension',

      icon: 'pi pi-github'

    }

  ]

})

# Section: Server Config

ComfyUI Settings

Server Config

Detailed description of ComfyUI server configuration options

Currently the Server Config settings menu only exists in the Desktop version, and this
settings menu item does not exist in other versions

Network

Host: The IP address to listen on

• 	Function: Sets the IP address the server binds to. Default 127.0.0.1 means only
local access is allowed. If you need LAN access, you can set it to 0.0.0.0

Although we provide LAN listening settings for the Desktop version, as a desktop
application, it is not suitable for use as a server. We recommend that if you need to use
ComfyUI as a public service within the LAN, please refer to the manual deployment
tutorial to deploy the corresponding ComfyUI service.

Port: The port to listen on

Function: The port number the server listens on. Desktop version defaults to port 8000,
Web version typically uses port 8188

TLS Key File: Path to TLS key file for HTTPS

Function: The private key file path required for HTTPS encryption, used to establish
secure connections

TLS Certificate File: Path to TLS certificate file for HTTPS

Function: The certificate file path required for HTTPS encryption, used in conjunction
with the private key

Enable CORS header: Use ”*” for all origins or specify domain

Function: Cross-Origin Resource Sharing settings, allowing web browsers to access
the server from diﬀerent domains

Maximum upload size (MB)

Function: Limits the maximum size of single file uploads, in MB, default 100MB. Aﬀects
upload limits for images, models and other files

CUDA

CUDA device index to use

Function: Specifies which NVIDIA graphics card to use. 0 represents the first graphics
card, 1 represents the second, and so on. Important for multi-GPU systems

Use CUDA malloc for memory allocation

Function: Controls whether to use CUDA’s memory allocator. Can improve memory
management eﬃciency in certain situations

Inference

Global floating point precision

Function: Sets the numerical precision for model calculations. FP16 saves VRAM but
may aﬀect quality, FP32 is more precise but uses more VRAM

UNET precision

Options:

• 	 auto: Automatically selects the most suitable precision

• 	 fp64: 64-bit floating point precision, highest precision but largest VRAM
usage

• 	 fp32: 32-bit floating point precision, standard precision

• 	 fp16: 16-bit floating point precision, can save VRAM

• 	 bf16: 16-bit brain floating point precision, between fp16 and fp32

• 	 fp8_e4m3fn: 8-bit floating point precision (e4m3), minimal VRAM usage

• 	 fp8_e5m2: 8-bit floating point precision (e5m2), minimal VRAM usage

Function: Specifically controls the computational precision of the UNET core
component of diﬀusion models. Higher precision can provide better image generation
quality but uses more VRAM. Lower precision can significantly save VRAM but may
aﬀect the quality of generated results.

VAE precision

Options and Recommendations:

• 	 auto: Automatically selects the most suitable precision, recommended for
users with 8-12GB VRAM

• 	 fp16: 16-bit floating point precision, recommended for users with 6GB or
less VRAM, can save VRAM but may aﬀect quality

• 	 fp32: 32-bit floating point precision, recommended for users with 16GB
or more VRAM who pursue the best quality

• 	 bf16: 16-bit brain floating point precision, recommended for newer
graphics cards that support this format, can achieve better performance
balance

Function: Controls the computational precision of the Variational Autoencoder (VAE),
aﬀecting the quality and speed of image encoding/decoding. Higher precision can
provide better image reconstruction quality but uses more VRAM. Lower precision can
save VRAM but may aﬀect image detail restoration.

Run VAE on CPU

Function: Forces VAE to run on CPU, can save VRAM but will reduce processing speed

Text Encoder precision

Options:

• 	 auto: Automatically selects the most suitable precision

• 	 fp8_e4m3fn: 8-bit floating point precision (e4m3), minimal VRAM usage

• 	 fp8_e5m2: 8-bit floating point precision (e5m2), minimal VRAM usage

• 	 fp16: 16-bit floating point precision, can save VRAM

• 	 fp32: 32-bit floating point precision, standard precision

Function: Controls the computational precision of the text prompt encoder, aﬀecting
the accuracy of text understanding and VRAM usage. Higher precision can provide
more accurate text understanding but uses more VRAM. Lower precision can save
VRAM but may aﬀect prompt parsing eﬀectiveness.

Memory

Force channels-last memory format

Function: Changes the data arrangement in memory, may improve performance on
certain hardware

DirectML device index

Function: Specifies the device when using DirectML acceleration on Windows, mainly
for AMD graphics cards

Disable IPEX optimization

Function: Disables Intel CPU optimization, mainly aﬀects Intel processor performance

VRAM management mode

Options:

• 	 auto: Automatically manages VRAM, allocating VRAM based on model
size and requirements

• 	 lowvram: Low VRAM mode, uses minimal VRAM, may aﬀect generation
quality

• 	 normalvram: Standard VRAM mode, balances VRAM usage and
performance

• 	 highvram: High VRAM mode, uses more VRAM for better performance

• 	 novram: No VRAM usage, runs entirely on system memory

• 	 cpu: CPU-only mode, doesn’t use graphics card

Function: Controls VRAM usage strategy, such as automatic management, low VRAM
mode, etc.

Reserved VRAM (GB)

Function: Amount of VRAM reserved for the operating system and other programs,
prevents system freezing

Disable smart memory management

Function: Disables automatic memory optimization, forces models to move to system
memory to free VRAM

Preview

Method used for latent previews

Options:

• 	 none: No preview images displayed, only shows progress bar during
generation

• 	 auto: Automatically selects the most suitable preview method,
dynamically adjusts based on system performance and VRAM

• 	 latent2rgb: Directly converts latent space data to RGB images for
preview, faster but average quality

• 	 taesd: Uses lightweight TAESD model for preview, balances speed and
quality

Function: Controls how to preview intermediate results during generation. Diﬀerent
preview methods aﬀect preview quality and performance consumption. Choosing the
right preview method can find a balance between preview eﬀects and system resource
usage.

Size of preview images

Function: Sets the resolution of preview images, aﬀects preview clarity and
performance. Larger sizes provide higher preview quality but also consume more
VRAM

Cache

Use classic cache system

Function: Uses traditional caching strategy, more conservative but stable

Use LRU caching with a maximum of N node results cached

Function: Uses Least Recently Used (LRU) algorithm caching system, can cache a
specified number of node computation results

Description:

• Set a specific number to control maximum cache count, such as 10, 50, 100,
etc.

• Caching can avoid repeated computation of the same node operations,
improving workflow execution speed

• When cache reaches the limit, automatically clears the least recently used
results

• Cached results occupy system memory (RAM/VRAM), larger values use more
memory

Usage Recommendations:

• Default value is null, meaning LRU caching is not enabled

• Set appropriate cache count based on system memory capacity and usage
requirements

• Recommended for workflows that frequently reuse the same node
configurations

• If system memory is suﬃcient, larger values can be set for better performance
improvement

Attention

Cross attention method

Options:

• 	 auto: Automatically selects the most suitable attention computation
method

• 	 split: Block-wise attention computation, can save VRAM but slower
speed

• 	 quad: Uses quad attention algorithm, balances speed and VRAM usage

• 	 pytorch: Uses PyTorch native attention computation, faster but higher
VRAM usage

Function: Controls the specific algorithm used when the model computes attention.
Diﬀerent algorithms make diﬀerent trade-oﬀs between generation quality, speed, and
VRAM usage. Usually recommended to use auto for automatic selection.

Force attention upcast

Function: Forces high-precision attention computation, improves quality but increases
VRAM usage

Prevent attention upcast

Function: Disables high-precision attention computation, saves VRAM

General

Disable xFormers optimization

Function: Disables the optimization features of the xFormers library. xFormers is a
library specifically designed to optimize the attention mechanisms of Transformer
models, typically improving computational eﬃciency, reducing memory usage, and
accelerating inference speed. Disabling this optimization will:

• Fall back to standard attention computation methods

• May increase memory usage and computation time

• Provide a more stable runtime environment in certain situations

Use Cases:

• When encountering compatibility issues related to xFormers

• When more precise computation results are needed (some optimizations may
aﬀect numerical precision)

• When debugging or troubleshooting requires using standard implementations

Default hashing function for model files

Options:

• 	 sha256: Uses SHA-256 algorithm for hash verification, high security but
slower computation

• 	 sha1: Uses SHA-1 algorithm, faster but slightly lower security

• 	 sha512: Uses SHA-512 algorithm, provides highest security but slowest
computation

• 	 md5: Uses MD5 algorithm, fastest but lowest security

Function: Sets the hash algorithm for model file verification, used to verify file integrity.
Diﬀerent hash algorithms have diﬀerent trade-oﬀs between computation speed and
security. Usually recommended to use sha256 as the default option, which achieves a
good balance between security and performance.

Make pytorch use slower deterministic algorithms when it can

Function: Forces PyTorch to use deterministic algorithms when possible to improve
result reproducibility.

Description:

• When enabled, PyTorch will prioritize deterministic algorithms over faster non-
deterministic algorithms

• Same inputs will produce same outputs, helpful for debugging and result
verification

• Deterministic algorithms typically run slower than non-deterministic algorithms

• Even with this setting enabled, completely identical image results cannot be
guaranteed in all situations

Use Cases:

• Scientific research requiring strict result reproducibility

• Debugging processes requiring stable output results

• Production environments requiring result consistency

Enable some untested and potentially quality deteriorating optimizations

Function: Enables experimental optimizations that may improve speed but could
potentially aﬀect generation quality

Don’t print server output to console

Function: Prevents displaying server runtime information in the console, keeping the
interface clean.

Description:

• When enabled, ComfyUI server logs and runtime information will not be
displayed

• Can reduce console information interference, making the interface cleaner

• May slightly improve system performance when there’s heavy log output

• Default is disabled (false), meaning server output is displayed by default

Use Cases:

• Production environments where debugging information is not needed

• When wanting to keep the console interface clean

• When the system runs stably and log monitoring is not required

Note: It’s recommended to keep this option disabled during development and
debugging to promptly view server runtime status and error information.

Disable saving prompt metadata in files

Function: Does not save workflow information in generated images, reducing file size,
but also means the loss of corresponding workflow information, preventing you from
using workflow output files to reproduce the corresponding generation results

Disable loading all custom nodes

Function: Prevents loading all third-party extension nodes, typically used when
troubleshooting issues to locate whether errors are caused by third-party extension
nodes

Logging verbosity level

Function: Controls the verbosity level of log output, used for debugging and monitoring
system runtime status.

Options:

• 	 CRITICAL: Only outputs critical error information that may cause the
program to stop running

• 	 ERROR: Outputs error information indicating some functions cannot work
properly

• 	 WARNING: Outputs warning information indicating possible issues that
don’t aﬀect main functionality

• 	 INFO: Outputs general information including system runtime status and
important operation records

• 	 DEBUG: Outputs the most detailed debugging information including
system internal runtime details

Description:

• Log levels increase in verbosity from top to bottom

• Each level includes all log information from higher levels

• Recommended to set to INFO level for normal use

• Can be set to DEBUG level when troubleshooting for more information

• Can be set to WARNING or ERROR level in production environments to reduce
log volume

Directories

Input directory

Function: Sets the default storage path for input files (such as images, models)

Output directory

Function: Sets the save path for generation results

Troubleshooting

# Table of Contents

1. Overview

2. Model Issues

3. Custom Node Issues

# Section: Overview

Troubleshooting

How to Troubleshoot and Solve ComfyUI Issues

Common ComfyUI issues, solutions, and how to report bugs eﬀectively

We receive a lot of feedback issues, and we find that most of the issues submitted are
related to custom nodes. So please ensure that you have read the custom node
troubleshooting guide before submitting an error report to ensure that the issue is not
caused by ComfyUI core issues.

Custom Node Troubleshooting Guide

Check how to troubleshoot issues caused by custom nodes.

Common Issues & Quick Fixes

Before diving into detailed troubleshooting, try these common solutions:

ComfyUI Won’t Start

Symptoms: Application crashes on startup, black screen, or fails to load

Quick fixes:

1. Check system requirements - Ensure your system meets the minimum
requirements

2. Update GPU drivers - Download latest drivers from NVIDIA/AMD/Intel

Generation Fails or Produces Errors

Symptoms: “Prompt execution failed” dialog with “Show report” button, workflow
stops executing

Quick fixes:

1. Click “Show report” - Read the detailed error message to identify the specific
issue

2. Check if it’s a custom node issue - Follow our custom node troubleshooting
guide

3. Verify model files - See Models documentation for model setup

4. Check VRAM usage - Close other applications using GPU memory

Slow Performance

Symptoms: Very slow generation times, system freezing, out of memory errors

Quick fixes:

1. Lower resolution/batch size - Reduce image size or number of images

2. Use memory optimization flags - See performance optimization section below

3. Close unnecessary applications - Free up RAM and VRAM

4. Check CPU/GPU usage - Use Task Manager to identify bottlenecks

Performance Optimization Commands:

For low VRAM systems:

Copy

Ask AI

# Low VRAM mode (uses cpu for text encoder)

python main.py --lowvram

# CPU mode (very slow but works with any hardware, only use as absolute last resort)

python main.py --cpu

For better performance:

Copy

Ask AI

# Disable previews (saves VRAM and processing)

python main.py --preview-method none

# Use optimized attention mechanisms

python main.py --use-pytorch-cross-attention

python main.py --use-flash-attention

# Async weight oﬄoading

python main.py --async-oﬄoad

For memory management:

Copy

Ask AI

# Reserve specific VRAM amount for OS (in GB)

python main.py --reserve-vram 2

# Disable smart memory management

python main.py --disable-smart-memory

# Use diﬀerent caching strategies

python main.py --cache-none      # Less RAM usage, but slower

python main.py --cache-lru 10    # Cache 10 results, faster

python main.py --cache-classic   # Use the old style (aggressive) caching.

Installation-Specific Issues

Desktop App Issues

For comprehensive desktop installation troubleshooting, see the Desktop Installation
Guide.

• 	Windows

• 	macOS

• 	Linux

• 	Unsupported device: ComfyUI Desktop Windows only supports NVIDIA GPUs
with CUDA. Use ComfyUI Portable or manual installation for other GPUs

• 	Installation fails: Run installer as administrator, ensure at least 15GB disk space

• 	Maintenance page: Check mirror settings if downloads fail

• 	Missing models: Models are not copied during migration, only linked. Verify
model paths

Manual Installation Issues

The documentation may be slightly out of date. If an issue occurs, please manually
verify whether a newer stable version of pytorch or any of the listed libraries exists.
Refer to resources like the pytorch installation matrix or the ROCm website.

Python version conflicts:

Copy

Ask AI

# Check Python version (3.9+ required, 3.12 recommended)

python --version

# Use virtual environment (recommended)

python -m venv comfyui_env

source comfyui_env/bin/activate  # Linux/Mac

comfyui_env\Scripts\activate     # Windows

Package installation failures:

Copy

Ask AI

# Update pip first

python -m pip install --upgrade pip

# Install dependencies

pip install -r requirements.txt

# For NVIDIA GPUs (CUDA 12.8)

pip install torch torchvision torchaudio --extra-index-url https://download.pytorch.org/
whl/cu128

# For AMD GPUs (Linux only - ROCm 6.3)

pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/
rocm6.3

Linux-Specific Issues

LD_LIBRARY_PATH errors:

Common symptoms:

• “libcuda.so.1: cannot open shared object file”

• “libnccl.so: cannot open shared object file”

• “ImportError: libnvinfer.so.X: cannot open shared object file”

Solutions:

1. Modern PyTorch installations (most common):

Copy

Ask AI

# For virtual environments with NVIDIA packages

export LD_LIBRARY_PATH=$VIRTUAL_ENV/lib/python3.12/site-packages/nvidia/
nvjitlink/lib:$LD_LIBRARY_PATH

# For conda environments

export LD_LIBRARY_PATH=$CONDA_PREFIX/lib/python3.12/site-packages/nvidia/
nvjitlink/lib:$LD_LIBRARY_PATH

# Or find your Python site-packages automatically

PYTHON_PATH=$(python -c "import site; print(site.getsitepackages()[0])")

export LD_LIBRARY_PATH=$PYTHON_PATH/nvidia/nvjitlink/lib:$LD_LIBRARY_PATH

# You may also need other NVIDIA libraries

export LD_LIBRARY_PATH=$PYTHON_PATH/nvidia/cuda_runtime/lib:
$LD_LIBRARY_PATH

export LD_LIBRARY_PATH=$PYTHON_PATH/nvidia/cublas/lib:$LD_LIBRARY_PATH

2. Find what libraries you have:

Copy

Ask AI

# Check installed NVIDIA packages

python -c "import site; import os; nvidia_path=os.path.join(site.getsitepackages()[0],
'nvidia'); print('NVIDIA libs:', [d for d in os.listdir(nvidia_path) if
os.path.isdir(os.path.join(nvidia_path, d))] if os.path.exists(nvidia_path) else 'Not
found')"

# Find missing libraries that PyTorch needs

python -c "import torch; print(torch.__file__)"

ldd $(python -c "import torch; print(torch.__file__.replace('__init__.py', 'lib/
libtorch_cuda.so'))")

3. Set permanently for your environment:

Copy

Ask AI

# For virtual environments, add to activation script

echo 'export LD_LIBRARY_PATH=$VIRTUAL_ENV/lib/python*/site-packages/nvidia/
nvjitlink/lib:$LD_LIBRARY_PATH' >> $VIRTUAL_ENV/bin/activate

# For conda environments

conda env config vars set LD_LIBRARY_PATH=$CONDA_PREFIX/lib/python*/site-
packages/nvidia/nvjitlink/lib:$LD_LIBRARY_PATH

# For global bashrc (adjust Python version as needed)

echo 'export LD_LIBRARY_PATH=$(python -c "import site; print(site.getsitepackages()
[0])")/nvidia/nvjitlink/lib:$LD_LIBRARY_PATH' >> ~/.bashrc

4. Alternative: Use ldconfig:

Copy

Ask AI

# Check current library cache

ldconfig -p | grep cuda

ldconfig -p | grep nccl

# If missing, add library paths (requires root)

sudo echo "/usr/local/cuda/lib64" > /etc/ld.so.conf.d/cuda.conf

sudo ldconfig

5. Debug library loading:

Copy

Ask AI

# Verbose library loading to see what's missing

LD_DEBUG=libs python main.py 2>&1 | grep "looking for"

# Check PyTorch CUDA availability

python -c "import torch; print('CUDA available:', torch.cuda.is_available()); print('CUDA
version:', torch.version.cuda)"

Model-Related Issues

For comprehensive model troubleshooting including architecture mismatches, missing
models, and loading errors, see the dedicated Model Issues page.

Network & API Issues

API Nodes Not Working

Symptoms: API calls fail, timeout errors, quota exceeded

Solutions:

1. Check API key validity - Verify keys in user settings

2. Check account credits - Ensure suﬃcient API credits

3. Verify internet connection - Test with other online services

4. Check service status - Provider may be experiencing downtime

Connection Issues

Symptoms: “Failed to connect to server”, timeout errors

Solutions:

1. Check firewall settings - Allow ComfyUI through firewall

2. Try diﬀerent port - Default is 8188, try 8189 or 8190

3. Disable VPN temporarily - VPN may be blocking connections

4. Check proxy settings - Disable proxy if not required

Frontend Issues

“Frontend or Templates Package Not Updated”:

Copy

Ask AI

# After updating ComfyUI via Git, update frontend dependencies

pip install -r requirements.txt

“Can’t Find Custom Node”:

• Disable node validation in ComfyUI settings

“Error Toast About Workflow Failing Validation”:

• Disable workflow validation in settings temporarily

• Report the issue to the ComfyUI team

Login Issues When Not on Localhost:

• 	Normal login only works when accessing from localhost

• 	For LAN/remote access: Generate API key at platform.comfy.org/login

• 	Use API key in login dialog or with --api-key command line argument

Hardware-Specific Issues

NVIDIA GPU Issues

“Torch not compiled with CUDA enabled” error:

Copy

Ask AI

# First uninstall torch

pip uninstall torch

# Install stable PyTorch with CUDA 12.8

pip install torch torchvision torchaudio --extra-index-url https://download.pytorch.org/
whl/cu128

# For nightly builds (might have performance improvements)

pip install --pre torch torchvision torchaudio --index-url https://download.pytorch.org/
whl/nightly/cu128

# Verify CUDA support

python -c "import torch; print(torch.cuda.is_available())"

GPU not detected:

Copy

Ask AI

# Check if GPU is visible

nvidia-smi

# Check driver version and CUDA compatibility

nvidia-smi --query-gpu=driver_version --format=csv

AMD GPU Issues

ROCm support (Linux only):

Copy

Ask AI

# Install stable ROCm PyTorch (6.3.1 at the time of writing)

pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/
rocm6.3

# For nightly builds (ROCm 6.4 at the time of writing), which might have performance
improvements)

pip install --pre torch torchvision torchaudio --index-url https://download.pytorch.org/
whl/nightly/rocm6.4

Unsupported AMD GPUs:

Copy

Ask AI

# For RDNA2 or older (6700, 6600)

HSA_OVERRIDE_GFX_VERSION=10.3.0 python main.py

# For RDNA3 cards (7600)

HSA_OVERRIDE_GFX_VERSION=11.0.0 python main.py

Performance optimization:

Copy

Ask AI

# Enable experimental memory eﬃcient attention (no longer necessary with PyTorch
2.4)

TORCH_ROCM_AOTRITON_ENABLE_EXPERIMENTAL=1 python main.py --use-
pytorch-cross-attention

# Enable tunable operations (slow first run, but faster subsequent runs)

PYTORCH_TUNABLEOP_ENABLED=1 python main.py

Apple Silicon (M1/M2/M3) Issues

MPS backend setup:

Copy

Ask AI

# Install PyTorch nightly for Apple Silicon

# Follow Apple's guide: https://developer.apple.com/metal/pytorch/

# Check MPS availability

python -c "import torch; print(torch.backends.mps.is_available())"

# Launch ComfyUI

python main.py

If MPS causes issues:

Copy

Ask AI

# Force CPU mode

python main.py --cpu

# With memory optimization

python main.py --force-fp16 --cpu

Intel GPU Issues

Option 1: Native PyTorch XPU support (Windows/Linux):

Copy

Ask AI

# Install PyTorch nightly with XPU support

pip install --pre torch torchvision torchaudio --index-url https://download.pytorch.org/
whl/nightly/xpu

# Launch ComfyUI

python main.py

Option 2: Intel Extension for PyTorch (IPEX):

Copy

Ask AI

# For Intel Arc A-Series Graphics

conda install libuv

pip install torch==2.3.1.post0+cxx11.abi torchvision==0.18.1.post0+cxx11.abi
torchaudio==2.3.1.post0+cxx11.abi intel-extension-for-pytorch==2.3.110.post0+xpu --
extra-index-url https://pytorch-extension.intel.com/release-whl/stable/xpu/us/

Getting Help & Reporting Bugs

Before Reporting a Bug

1. 	Check if it’s a known issue:

• 	Search GitHub Issues

• 	Check ComfyUI Forum

• 	Review Discord discussions

2. 	Try basic troubleshooting:

• 	Test with default workflow

• 	Disable all custom nodes (see custom node troubleshooting)

• 	Check console/terminal for error messages

• 	If using comfy-cli, try updating: comfy node update all

How to Report Bugs Eﬀectively

For ComfyUI Core Issues

Where to report: GitHub Issues

For Desktop App Issues

Where to report: Desktop GitHub Issues

For Frontend Issues

Where to report: Frontend GitHub Issues

For Custom Node Issues

Where to report: Contact the specific custom node developer

Required Information

When reporting any issue, include:

1

System Information

• 	From ComfyUI Interface

• 	From Command Line

System Information (can be found in the About page in settings):

• 	Operating System (Windows 11, macOS 14.1, Ubuntu 22.04, etc.)

• 	ComfyUI version (check About page in settings)

• 	Python version: python --version

• 	PyTorch version: python -c "import torch; print(torch.__version__)"

• 	GPU model and driver version

• 	Installation method (Desktop, Portable, Manual, comfy-cli)

2

Desktop App issues

For Desktop App issues, also include:

• 	Log files from: C:\Users\<username>\AppData\Roaming\ComfyUI\logs
(Windows)

• 	Config files from: C:\Users\<username>\AppData\Roaming\ComfyUI (Windows)

3

Problem Details

Problem Details:

• Clear description of the issue

• Steps to reproduce the problem

• Expected vs actual behavior

• Screenshots or videos if applicable

Error Messages:

• Full error text from console/terminal

• Browser console errors (F12 → Console tab)

• Any crash logs or error dialogs

4

Additional Context

Additional Context:

• List of installed custom nodes

• Workflow file (.json) that reproduces the issue

• Recent changes (new installations, updates, etc.)

Community Resources

• 	Oﬃcial Forum: forum.comfy.org

• 	Discord: ComfyUI Discord Server

• 	Reddit: r/comfyui

• 	YouTube: ComfyUI Tutorials

# Section: Model Issues

Troubleshooting

How to Troubleshoot and Solve ComfyUI Model Issues

Troubleshooting model-related problems including architecture mismatches, missing
models, and loading errors

Model Architecture Mismatch

Symptoms: Tensor dimension errors during generation, especially during VAE decode
stage

Common error messages:

• 	Given groups=1, weight of size [64, 4, 3, 3], expected input[1, 16, 128, 128] to
have 4 channels, but got 16 channels instead

• 	Given groups=1, weight of size [4, 4, 1, 1], expected input[1, 16, 144, 112] to
have 4 channels, but got 16 channels instead

• 	Given groups=1, weight of size [320, 4, 3, 3], expected input[2, 16, 192, 128] to
have 4 channels, but got 16 channels instead

• 	The size of tensor a (49) must match the size of tensor b (16) at non-singleton
dimension 1

• 	Tensors must have same number of dimensions: got 2 and 3

• 	mat1 and mat2 shapes cannot be multiplied (154x2048 and 768x320)

Root cause: Using models from diﬀerent architecture families together

Solutions

1. 	Verify model family compatibility:

• 	Flux models use 16-channel latent space with dual text encoder
conditioning (CLIP-L + T5-XXL)

• 	SD1.5 models use 4-channel latent space with single CLIP ViT-L/14 text
encoder

• 	SDXL models use 4-channel latent space with dual text encoders (CLIP
ViT-L/14 + OpenCLIP ViT-bigG/14)

• 	SD3 models use 16-channel latent space with triple text encoder
conditioning (CLIP-L + OpenCLIP bigG + T5-XXL)

• 	ControlNet models must match the architecture of the base checkpoint
(SD1.5 ControlNets only work with SD1.5 checkpoints, SDXL ControlNets
only work with SDXL checkpoints, etc.)

2. 	Common mismatch scenarios and fixes: Flux + wrong VAE:

Copy





Ask AI




Problem: Using taesd or sdxl_vae.safetensors with Flux checkpoint

3. 	Fix: Use ae.safetensors (Flux VAE) from Hugging Face Flux releases

4.









Flux + incorrect CLIP configuration:

Copy





Ask AI



Problem: Using t5xxl_fp8_e4m3fn.safetensors in both CLIP slots of
DualClipLoader

5. 	Fix: Use t5xxl_fp8_e4m3fn.safetensors in one slot and clip_l.safetensors in the
other

6.









ControlNet architecture mismatch:

Copy





Ask AI



Problem: SD1.5 ControlNet with SDXL checkpoint (or vice versa)

7. 	Error: "mat1 and mat2 shapes cannot be multiplied (154x2048 and 768x320)"

8. 	Fix: Use ControlNet models designed for your checkpoint architecture

9. 	     - SD1.5 checkpoints require SD1.5 ControlNets

10. 	     - SDXL checkpoints require SDXL ControlNets

11.







12. 	Quick diagnostics:

Copy





Ask AI




# Check if error occurs at VAE decode stage

13. 	# Look for "expected input[X, Y, Z] to have N channels, but got M channels"

14. 	# Y value indicates channel count: 4 = SD models, 16 = Flux models

15.







16. 	Prevention strategies:

• 	Keep all workflow models within the same architecture family

• 	Download complete model packages from same source/release (often all
in a Hugging Face repo)

• 	When trying new models, start with the template workflows or oﬃcial
ComfyUI workflow examples before customizing

Missing Models Error

Example error message:

Copy

Ask AI

Prompt execution failed

Prompt outputs failed validation:

CheckpointLoaderSimple:

- Value not in list: ckpt_name: 'model-name.safetensors' not in []

Solutions

1. 	Download required models:

• 	Use ComfyUI Manager to auto-download models

• 	Verify models are in correct subfolders

2. 	Check model paths:

• 	Checkpoints: models/checkpoints/

• 	VAE: models/vae/

• 	LoRA: models/loras/

• 	ControlNet: models/controlnet/

• 	Embeddings: models/embeddings/

3. 	Share models between UIs or use custom paths:

• 	See ComfyUI Model Sharing and Custom Model Directory Configuration
for detailed instructions

• 	Edit extra_model_paths.yaml file to add custom model directories

Model Search Path Configuration

If you have models in custom locations, see the detailed guide for ComfyUI Model
Sharing and Custom Model Directory Configuration to configure ComfyUI to find them.

Model Loading Errors

Error message: “Error while deserializing header”

Solutions

1. Re-download the model - File may be corrupted during download

2. Check available disk space - Ensure enough space for model loading (models
can be 2-15GB+)

3. Check file permissions - Ensure ComfyUI can read the model files

4. Test with diﬀerent model - Verify if issue is model-specific or system-wide

Model Performance Issues

Slow Model Loading

Symptoms: Long delays when switching models or starting generation

Solutions:

1. 	Use faster storage:

• 	Move models to SSD if using HDD

• 	Use NVMe SSD for best performance

2. 	Adjust caching settings:

Copy





Ask AI



python main.py --cache-classic       # Use the old style (aggressive) caching.

3. 	python main.py --cache-lru 10         # Increase size of LRU cache

4.








Memory Issues with Large Models

“RuntimeError: CUDA out of memory”:

Copy

Ask AI

# Progressive memory reduction

python main.py --lowvram          # First try

python main.py --novram           # If lowvram insuﬃcient

python main.py --cpu              # Last resort

Model-specific memory optimization:

Copy

Ask AI

# Force lower precision

python main.py --force-fp16

# Reduce attention memory usage

python main.py --use-pytorch-cross-attention

For additional model configuration and setup information, see the Models
documentation.

# Section: Custom Node Issues

Troubleshooting

How to Troubleshoot and Solve ComfyUI Issues

Troubleshoot and fix problems caused by custom nodes and extensions

Here is the overall approach for troubleshooting custom node issues:

#_r_1s_{font-family:inherit;font-size:16px;fill:#ccc;}#_r_1s_ .error-icon{fill:#a44141;}
#_r_1s_ .error-text{fill:#ddd;stroke:#ddd;}#_r_1s_ .edge-thickness-normal{stroke-
width:1px;}#_r_1s_ .edge-thickness-thick{stroke-width:3.5px;}#_r_1s_ .edge-pattern-
solid{stroke-dasharray:0;}#_r_1s_ .edge-thickness-invisible{stroke-width:0;fill:none;}

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

Iss
ue
cau
sed
by
cus
tom
nod
es

Iss
ue
not
cau
sed
by
cus
tom
nod

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

Restart ComfyUI and  Issue is in enabled
test custom nodes

Issue is in disabled
custom nodes

Enabled custom
nodes > 1?

Disabled custom
nodes > 1?

Continue binary
search on enabled
nodes

Continue binary
search on disabled
nodes

Found problematic
custom node

End

Two
Troubleshoo
ting
Methods

In this document,
we categorize
custom nodes into
two types for
troubleshooting:

• A: Custom
nodes with

En
d
.
```