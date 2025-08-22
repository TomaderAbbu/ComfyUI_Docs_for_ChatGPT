# SECTION: CORE_CONCEPTS


## ITEM:
Follow the numbered steps in the image:
1. Click the Fit View button in the bottom right to ensure any loaded workflow
isn’t hidden
2. Click the folder icon (workflows) in the sidebar
3. Click the Browse example workflows button at the top of the Workflows panel
Continue with:


## ITEM:
• 	FluxKontextMultiReferenceLatentMethod Node: Multi-reference input node for
Flux workflows


## ITEM:
• 	WAN 2.2 Fun Camera Model Support: Support for video generation through
camera control


## ITEM:
• 	Template Updates: Upgraded to version 0.1.62, added Wan2.2 Fun Camera and
Qwen Image Edit templates


## ITEM:
Core Function Improvements


## ITEM:
• 	Context Windows Support: Enhanced sampling code to support longer
sequence generation tasks


## ITEM:
• 	SDPA Backend Optimization: Improved Scaled Dot Product Attention backend
settings for better performance


## ITEM:
Multimedia Node Support


## ITEM:
• 	Audio Recording Node: New native audio recording node, now you can record
audio directly in ComfyUI


## ITEM:
• 	Audio Video Integration: Complete audio-video dependency integration


## ITEM:
API Node Support Updates


## ITEM:
• 	GPT-5 Series Models: Support for the latest GPT-5 models


## ITEM:
• 	Kling V2-1 and V2-1-Master: Updated video generation model functionality


## ITEM:
• 	Minimax Hailuo Video Node: New video generation node


## ITEM:
• 	Vidu Video Node: Vidu API node support


## ITEM:
• 	Google Model Updates: Added new Google Gemini models


## ITEM:
• 	OpenAI API Fix: Fixed MIME type errors in OpenAI API node input images


## ITEM:
Performance Optimization


## ITEM:
• 	Mini Map: Added workflow mini map


## ITEM:
• 	Tab Preview: Added workflow tab preview


## ITEM:
• 	Top Tab Menu Layout Adjustments


## ITEM:
This release expands ComfyUI’s model ecosystem with enhanced Qwen support,
async API capabilities, and stability improvements for complex workflows:


## ITEM:
Qwen Model Ecosystem


## ITEM:
• 	Qwen Image Model Support: Improved integration including proper LoRA
loading and model merging capabilities for sophisticated vision workflows


## ITEM:
• 	Qwen Model Merging Node: New dedicated node for merging Qwen image
models, allowing creators to combine diﬀerent model strengths


## ITEM:
• 	SimpleTuner Lycoris LoRA Support: Extended compatibility with SimpleTuner-
trained Lycoris LoRAs for Qwen-Image models


## ITEM:
API & Performance Infrastructure


## ITEM:
• 	Async API Nodes: Introduction of asynchronous API nodes, enabling non-
blocking workflow execution for better performance


## ITEM:
• 	Memory Handling: Enhanced RepeatLatentBatch node now properly handles
multi-dimensional latents, fixing workflow interruptions


## ITEM:
• 	WAN 2.2 Fun Control Support: Added support for WAN 2.2 fun control features,
expanding creative control for video workflows


## ITEM:
Hardware Optimization & Compatibility


## ITEM:
• 	AMD GPU Improvements: Enhanced AMD Radeon support with improved FP16
accuracy handling and performance optimization


## ITEM:
• 	Audio Processing Safety: Enhanced torchaudio import safety checks prevent
crashes when audio dependencies are unavailable


## ITEM:
• 	Kling API Improvements: Fixed image type parameter handling in Kling Image
API nodes


## ITEM:
Workflow Benefits


## ITEM:
• 	Async Workflow Execution: New async API capabilities enable more responsive
workflows when integrating external services


## ITEM:
• 	Model Flexibility: Expanded Qwen support allows for more diverse vision-
language workflows with improved LoRA compatibility


## ITEM:
• 	Hardware Utilization: AMD GPU optimizations and updated PyTorch support
improve performance across hardware configurations


## ITEM:
• 	Batch Processing: Fixed RepeatLatentBatch ensures reliable operation with
complex multi-dimensional data structures


## ITEM:
• 	Video Control: WAN 2.2 fun control features provide advanced creative control
for video generation workflows


## ITEM:
This release brings user experience improvements and model support that enhance
workflow creation and performance:


## ITEM:
User Interface Enhancements


## ITEM:
• 	Recently Used Items API: New API for tracking recently used items in the
interface, streamlining workflow creation


## ITEM:
• 	Workflow Navigation: Enhanced user experience with better organization of
commonly accessed elements


## ITEM:
Model Integration


## ITEM:
• 	Qwen Vision Model Support: Initial support for Qwen image models with
configuration options


## ITEM:
• 	Image Processing: Enhanced Qwen model integration allows for more versatile
image analysis and generation workflows


## ITEM:
Video Generation


## ITEM:
• 	Veo3 Video Generation: Added Veo3 video generation node with integrated
audio support


## ITEM:
• 	Audio-Visual Synthesis: Capability combining video and audio generation in a
single node


## ITEM:
Performance & Stability Improvements


## ITEM:
• 	Memory Management: Optimized conditional VRAM usage through improved
casting and device transfer operations


## ITEM:
• 	Device Consistency: Fixes ensuring all conditioning data and context remain on
correct devices


## ITEM:
• 	ControlNet Stability: Resolved ControlNet compatibility issues, restoring
functionality for image control workflows


## ITEM:
Developer & System Enhancements


## ITEM:
• 	Error Handling: Added warnings and crash prevention when conditioning
devices don’t match


## ITEM:
• 	Template Updates: Multiple template version updates (0.1.47, 0.1.48, 0.1.51)
maintaining compatibility


## ITEM:
Workflow Benefits


## ITEM:
• 	Faster Iteration: Recently used items API enables quicker workflow assembly
and modification


## ITEM:
• 	Enhanced Creativity: Qwen vision models open new possibilities for image
understanding and manipulation workflows


## ITEM:
• 	Video Production: Veo3 integration transforms ComfyUI into a comprehensive
multimedia creation platform


## ITEM:
• 	Reliability: Memory optimizations and device management fixes ensure stable
operation with complex workflows


## ITEM:
• 	Performance: Optimized VRAM usage allows for more ambitious projects on
systems with limited resources


## ITEM:
This release introduces backend improvements and performance optimizations that
enhance workflow execution and node development:


## ITEM:
ComfyAPI Core Framework


## ITEM:
• 	Partial Execution Support: New backend support for partial workflow execution,
enabling eﬃcient processing of multi-stage workflows


## ITEM:
Video Processing Improvements


## ITEM:
• 	WAN Camera Memory Optimization: Enhanced memory management for WAN-
based camera workflows, reducing VRAM usage


## ITEM:
Workflow Development Benefits


## ITEM:
• 	Video Workflows: Improved stability and performance for video generation
pipelines


## ITEM:
• 	Memory Management: Optimized memory usage patterns enable more complex
workflows on systems with limited VRAM


## ITEM:
This release focuses on memory optimizations for large model workflows, improving
performance with WAN 2.2 models and VRAM management:


## ITEM:
WAN 2.2 Model Optimizations


## ITEM:
• 	Reduced Memory Footprint: Eliminated unnecessary memory clones in WAN 2.2
VAE operations, reducing memory usage


## ITEM:
• 	5B I2V Model Support: Memory optimization for WAN 2.2 5B image-to-video
models, making these models more accessible


## ITEM:
Enhanced VRAM Management


## ITEM:
• 	Windows Large Card Support: Added reserved VRAM allocation for high-end
graphics cards on Windows


## ITEM:
• 	Memory Allocation: Improved memory management for users working with
multiple large models simultaneously


## ITEM:
Workflow Performance Benefits


## ITEM:
• 	VAE Processing: WAN 2.2 VAE operations now run more eﬃciently with reduced
memory overhead


## ITEM:
• 	Large Model Inference: Enhanced stability when working with billion-parameter
models


## ITEM:
• 	Batch Processing: Memory optimizations enable better handling of batch
operations with large models


## ITEM:
• 	PyAV Audio Backend: Replaced torchaudio.load with PyAV for more reliable
audio processing in video workflows


## ITEM:
• 	Audio Integration: Enhanced audio handling for multimedia generation
workflows


## ITEM:
Hardware Support


## ITEM:
• 	Iluvatar CoreX Support: Added native support for Iluvatar CoreX accelerators


## ITEM:
• 	Intel XPU Optimization: XPU support improvements including async oﬄoad
capabilities


## ITEM:
• 	AMD ROCm Enhancements: Enabled PyTorch attention by default for gfx1201
on Torch 2.8


## ITEM:
• 	WAN Model Support: Added support for WAN (Wavelet-based Attention
Network) models


## ITEM:
Training Features


## ITEM:
• 	Training Nodes: Added algorithm support, gradient accumulation, and optional
gradient checkpointing


## ITEM:
• 	Training Flexibility: Better memory management and performance optimization
for custom model training


## ITEM:
Node & Workflow Enhancements


## ITEM:
• 	Moonvalley V2V Node: Added Moonvalley Marey V2V node with enhanced input
validation


## ITEM:
• 	Negative Prompt Updates: Improved negative prompt handling for Moonvalley
nodes


## ITEM:
• 	History API Enhancement: Added map_function parameter to get_history API


## ITEM:
API & System Improvements


## ITEM:
• 	Frontend Version Tracking: Added required_frontend_version parameter in /
system_stats API response


## ITEM:
• 	Device Information: Enhanced XPU device name printing for better hardware
identification


## ITEM:
• 	Template Updates: Multiple template updates (0.1.40, 0.1.41) ensuring
compatibility


## ITEM:
Developer Experience


## ITEM:
• 	Documentation Updates: Enhanced README with examples and updated
model integration guides


## ITEM:
• 	Line Ending Fixes: Improved cross-platform compatibility by standardizing line
endings


## ITEM:
• 	Code Cleanup: Removed deprecated code and optimized components


## ITEM:
• 	Custom Prompt IDs: API now allows specifying prompt IDs for better workflow
tracking


## ITEM:
• 	Kling API Optimization: Increased polling timeout to prevent user timeouts


## ITEM:
• 	History Token Cleanup: Removed sensitive tokens from history items


## ITEM:
• 	Fresca Input/Output: Corrected input and output handling for Fresca model
workflows


## ITEM:
• 	Reference Bug Fixes: Resolved incorrect reference bugs in Gemini node
implementations


## ITEM:
• 	Line Ending Standardization: Automated detection and removal of Windows line
endings


## ITEM:
Developer Experience


## ITEM:
• 	Warning Systems: Added torch import mistake warnings to catch common
configuration issues


## ITEM:
• 	Transform Nodes: Added ImageRotate and ImageFlip nodes for enhanced
image manipulation


## ITEM:
• 	ImageColorToMask Fix: Corrected mask value returns for more accurate color-
based masking


## ITEM:
• 	3D Model Support: Upload 3D models to custom subfolders for better
organization


## ITEM:
Guidance & Conditioning Enhancements


## ITEM:
• 	PerpNeg Guider: Updated with improved pre and post-CFG handling


## ITEM:
• 	Audio Processing: Removed deprecated torchaudio.save function dependencies


## ITEM:
Model Integration


## ITEM:
• 	Moonvalley Nodes: Added native support for Moonvalley model workflows


## ITEM:
• 	Scheduler Reordering: Simple scheduler now defaults first


## ITEM:
• 	Template Updates: Multiple template version updates (0.1.31-0.1.35)


## ITEM:
Security & Safety


## ITEM:
• 	Safe Loading: Added warnings when loading files unsafely


## ITEM:
• 	File Validation: Enhanced checkpoint loading safety measures


## ITEM:
Model Support & Workflow Reliability


## ITEM:
This release brings improvements to model compatibility and workflow stability:


## ITEM:
Expanded Model Documentation: Added support documentation for Flux Kontext and
Omnigen 2 models VAE Encoding Improvements: Removed unnecessary random noise
injection during VAE encoding Memory Management Fix: Resolved a memory
estimation bug aﬀecting Kontext model usage


## ITEM:
• 	Flux Compatibility: Chroma Text Encoder now works with regular Flux models


## ITEM:
• 	LoRA Training Integration: New native LoRA training node using weight adapter
scheme


## ITEM:
Performance & Hardware Optimizations


## ITEM:
• 	AMD GPU Enhancements: Enabled FP8 operations and PyTorch attention on
AMD GPUs


## ITEM:
• 	Flux Model Stability: Resolved black image generation issues with certain Flux
models


## ITEM:
Sampling Improvements


## ITEM:
• 	Rectified Flow Samplers: Added SEEDS and multistep DPM++ SDE samplers
with RF support


## ITEM:
• 	ModelSamplingContinuousEDM: New cosmos_rflow option for enhanced
sampling control


## ITEM:
• 	Memory Optimization: Improved memory estimation for Cosmos models


## ITEM:
Developer & Integration Features


## ITEM:
• 	SQLite Database Support: Enhanced data management capabilities for custom
nodes


## ITEM:
• 	PyProject.toml Integration: Automatic web folder registration from pyproject files


## ITEM:
• 	Frontend Flexibility: Support for semver suﬃxes and prerelease frontend
versions


## ITEM:
• 	Tokenizer Enhancements: Configurable min_length settings with tokenizer_data


## ITEM:
Quality of Life Improvements


## ITEM:
• 	Kontext Aspect Ratio Fix: Resolved widget-only limitation


## ITEM:
• 	SaveLora Consistency: Standardized filename format across all save nodes


## ITEM:
Workflow Tools & Performance Optimizations


## ITEM:
This release brings new workflow utilities and performance optimizations:


## ITEM:
Workflow Tools


## ITEM:
• 	ImageStitch Node: Concatenate multiple images seamlessly in your workflows


## ITEM:
• 	GetImageSize Node: Extract image dimensions with batch processing support


## ITEM:
• 	Regex Replace Node: Advanced text manipulation capabilities for workflows


## ITEM:
Model Compatibility


## ITEM:
• 	Tensor Handling: Streamlined list processing makes multi-model workflows
more reliable


## ITEM:
• 	BFL API Optimization: Refined support for Kontext models with cleaner node
interfaces


## ITEM:
• 	Performance Boost: Fused multiply-add operations in chroma processing for
faster generation


## ITEM:
Developer Experience


## ITEM:
• 	API Documentation: Enhanced API nodes documentation


## ITEM:
Frontend & UI Enhancements


## ITEM:
_____________________________________
_____________________________________
_____________________________________
Basic Concepts


## ITEM:
Workflow


## ITEM:
A graph of nodes


## ITEM:
ComfyUI is an environment for building and running generative content workflows. In
this context, a workflow is defined as a collection of program objects called nodes that
are connected to each other, forming a network. This network is also known as a
graph.


## ITEM:
A ComfyUI workflow can generate any type of media: image, video, audio, AI model, AI
agent, and so on.


## ITEM:
Sample workflows


## ITEM:
In the context of ComfyUI, the term workflow is a synonym for the node network or
graph. It corresponds to the scene graph in a 3D or multimedia program: the network
of all of the nodes within a particular disk file. 3D programs call this a scene file. Video
editing, compositing, and multimedia programs usually call it a project file.


## ITEM:
Saving workflows


## ITEM:
The ComfyUI workflow is automatically saved in the metadata of any generated image,
allowing users to open and use the graph that generated the image. A workflow can
also be stored in a human-readable text file that follows the JSON data format. This is
necessary for media formats that don’t support metadata. ComfyUI workflows stored
as JSON files are very small, allowing convenient versioning, archiving, and sharing of
graphs, independently of any generated media.


## ITEM:
_____________________________________
_____________________________________
_____________________________________
Basic Concepts


## ITEM:
Nodes


## ITEM:
Understand the concept of a node in ComfyUI.


## ITEM:
Nodes perform operations


## ITEM:
In computer science, a node is a container for information, usually including
programmed instructions to perform some task. Nodes almost never exist in isolation,


## ITEM:
they’re almost always connected to other nodes in a networked graph. In ComfyUI,
nodes take the visual form of boxes that are connected to each other.


## ITEM:
ComfyUI nodes are usually function operators. This means that they operate on some
data to perform a function. A function is a process that accepts input data, performs
some operation on it, and produces output data. In other words, nodes do some work,
contributing to the completion of a task such as generating an image. So ComfyUI
nodes almost always have at least one input or output, and usually have multiple inputs
and outputs.


## ITEM:
Diﬀerent Node States


## ITEM:
In ComfyUI, nodes have multiple states. Here are some common node states:


## ITEM:
1. 	Normal State: The default state


## ITEM:
2. 	Running State: The running state, typically displayed when a node is executing
after you start running the workflow


## ITEM:
3. 	Error State: Node error, typically displayed after running the workflow if there’s a
problem with the node’s input, indicated by red marking of the erroneous input
node. You need to fix the problematic input to ensure the workflow runs
correctly


## ITEM:
4. 	Missing State: This state usually appears after importing workflows, with two
possibilities:


## ITEM:
• 	Comfy Core native node missing: This usually happens because ComfyUI
has been updated, but you’re using an older version of ComfyUI. You
need to update ComfyUI to resolve this issue


## ITEM:
Connections Between Nodes


## ITEM:
In ComfyUI, nodes are connected through links, allowing data of the same type to flow
between diﬀerent processing units to achieve the final result.


## ITEM:
Each node receives some input, processes it through its module, and converts it to
corresponding output. Connections between diﬀerent nodes must conform to the data
type requirements. In ComfyUI, we use diﬀerent colors to distinguish node data types.
Below are some basic data types:


## ITEM:
Data type Color


## ITEM:
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


## ITEM:
Connecting and Disconnecting Nodes


## ITEM:
Connecting: Drag from the output point of one node to the input of the same color on
another node to connect them Disconnecting: Click on the input endpoint and drag the
mouse left button to disconnect, or cancel the connection through the midpoint menu
of the link


## ITEM:
Node Appearance


## ITEM:
We provide various style settings for you to customize the appearance of nodes:


## ITEM:
• Modify styles


## ITEM:
• Double-click the node title to modify the node name


## ITEM:
• Switch node inputs between input sockets and widgets through the context
menu


## ITEM:
• Resize the node using the bottom right corner


## ITEM:
Node Badges


## ITEM:
We provide multiple node badge display features, such as:


## ITEM:
• Node ID


## ITEM:
• Node source


## ITEM:
• 	Never: The node will never execute under any circumstances, as if it’s been
deleted. Subsequent nodes cannot read or receive any data from it


## ITEM:
• 	Bypass: The node will never execute under any circumstances, but subsequent
nodes can still try to obtain data that hasn’t been processed by this node


## ITEM:
Below is a comparison of the Never and Bypass modes:


## ITEM:
In this comparison example, you can see that both workflows apply two LoRA models
simultaneously, with the diﬀerence being that one Load LoRA node is set to Never
mode while the other is set to Bypass mode.


## ITEM:
• 	The node set to Never mode causes subsequent nodes to show errors because
they don’t receive any input data


## ITEM:
• 	The node set to Bypass mode still allows subsequent nodes to receive
unprocessed data, so they load the output data from the first Load LoRA node,
allowing the subsequent workflow to continue running normally


## ITEM:
Switching Between Widget and Input Mode for Node Inputs


## ITEM:
In some cases, we need to use output results from other nodes as input. In this case,
we can switch between widget and input mode for node inputs.


## ITEM:
Here’s a very simple example:


## ITEM:
By switching the K-Sampler’s Seed from widget to input mode, multiple nodes can
share the same seed, achieving variable uniformity across multiple samplers.
Comparing the first node with the subsequent two nodes, you can see that the seed in
the latter two nodes is in input mode. You can also convert it back to widget mode:


## ITEM:
When dragging the input/output of a node, if a connection appears but you haven’t
connected to another node’s input or output, releasing the mouse will pop up a context
menu for the input/output, used to quickly add related types of nodes. You can adjust
the number of node suggestions in the settings:


## ITEM:
Node Selection Toolbox


## ITEM:
The Node Selection Toolbox is a floating tool that provides quick operations for nodes.
When you select a node, it hovers above the selected node. Through this toolbox, you
can:


## ITEM:
• Change the node’s color


## ITEM:
• Quickly set the node to Bypass mode (not execute during runtime)


## ITEM:
• Lock the node


## ITEM:
• Delete the node


## ITEM:
Of course, these functions can also be found in the right-click menu of the
corresponding node. The node selection toolbox just provides a shortcut operation. If
you want to disable this feature, you can turn it oﬀ in the settings.


## ITEM:
Node Groups


## ITEM:
In ComfyUI, you can select multiple parts of a workflow simultaneously, then use the
right-click menu to merge them into a node group, making that part a reusable module
that can be repeatedly called in your ComfyUI.


## ITEM:
Once Git is installed, navigate to the ComfyUI server program directory, to the folder
labeled custom_nodes. Open up a command window or terminal. Make sure that the
command line displays the current directory path as custom_nodes. Enter the following
command. This will download the Manager. Technically, this is known as cloning a Git
repository.


## ITEM:
Copy


## ITEM:
Ask AI


## ITEM:
```bash
git clone https://github.com/ltdrdata/ComfyUI-Manager.git
```


## ITEM:
_____________________________________
_____________________________________
_____________________________________
Basic Concepts


## ITEM:
After installing ComfyUI, you’ll discover that it includes many built-in nodes. These
native nodes are called Comfy Core nodes, which are oﬃcially maintained by ComfyUI.


## ITEM:
• Installing node dependencies


## ITEM:
2. Installing Node Dependencies


## ITEM:
In the Dependencies chapter, we introduced the relevant content about dependencies
in ComfyUI. ComfyUI is a Python-based project, and we built an independent Python
runtime environment for running ComfyUI. All related dependencies need to be
installed in this independent Python runtime environment.


## ITEM:
Depending on diﬀerent ComfyUI versions, we will use diﬀerent methods to install the
corresponding dependencies:


## ITEM:
python_embeded\python.exe -m pip install -r ComfyUI\custom_nodes\ComfyUI-
Manager\requirements.txt


## ITEM:
After installing Git, navigate to the ComfyUI server program directory and enter the
folder labeled custom_nodes. Open a command window or terminal. Make sure the
command line shows the current directory path as custom_nodes. Enter the following
command. This will download the manager. Technically, this is called cloning a Git
repository.


## ITEM:
Detecting Missing Nodes


## ITEM:
After installing the manager, you can detect missing nodes in the manager.


## ITEM:
_____________________________________
_____________________________________
_____________________________________
Basic Concepts


## ITEM:
Properties


## ITEM:
Nodes are containers for properties


## ITEM:
Nodes usually have properties. Also known as parameters or attributes, node
properties are variables that can be changed. Some properties can be adjusted
manually by the user, using a data entry field called a widget. Other properties can be
driven automatically by other nodes connected to the property input slot or port.
Usually, a property can be converted from widget to input and vice versa, allowing
users to control property values manually or automatically.


## ITEM:
Properties can take many forms and hold many diﬀerent types of information. For
example, a Load Checkpoint node has a single property:  the file path to the generative
model checkpoint file. A KSampler node has multiple properties such as the number of
sampling steps, CFG scale, sampler_name, etc.


## ITEM:
Data types


## ITEM:
Information can come in many diﬀerent forms, called data types. For example,
alphanumeric text is known as a string, a whole number is an integer, and a number
with a decimal point is known as a floating point number or float. New data types are
always being added to ComfyUI.


## ITEM:
ComfyUI is written in the Python scripting language, which is very forgiving about data
types. By contrast, the ComfyUI environment is very strongly typed. This means that
diﬀerent data types can’t be mixed up. For example, we can’t connect an image output
to an integer input. This is a huge benefit to users, guiding them to proper workflow
construction and preventing program errors.


## ITEM:
_____________________________________
_____________________________________
_____________________________________
Basic Concepts


## ITEM:
Links


## ITEM:
Understand connection links in ComfyUI


## ITEM:
As ComfyUI is still in rapid iteration and development, we are continuously improving it
every day. Therefore, some operations mentioned in this article may change or be
omitted. Please refer to the actual interface. If you find changes in actual operations, it
may be due to our iterative updates. You can also fork this repo and help us improve
this documentation.


## ITEM:
Links connect nodes


## ITEM:
In the terminology of ComfyUI, the lines or curves between nodes are called links.
They’re also known as connections or wires. Links can be displayed in several ways,
such as curves, right angles, straight lines, or completely hidden.


## ITEM:
You can modify the link style in Setup Menu —> Display (Lite Graph) —> Graph —>
Link Render Mode.


## ITEM:
Link display is crucial. Depending on the situation, it may be necessary to see all links.
Especially when learning, sharing, or even just understanding workflows, the visibility
of links enables users to follow the flow of data through the graph. For packaged
workflows that aren’t intended to be altered, it might make sense to hide the links to
reduce clutter.


## ITEM:
Reroute node


## ITEM:
If legibility of the graph structure is important, then link wires can be manually routed in
the 2D space of the graph with a tiny node called Reroute. Its purpose is to position the
beginning and/or end points of link wires to ensure visibility. We can design a workflow
so that link wires don’t pass behind nodes, don’t cross other link wires, and so on.


## ITEM:
The data type of node properties is indicated by color coding of input/output ports and
link connection wires. We can always tell which inputs and outputs can be connected
to one another by their color. Ports can only be connected to other ports of the same
color to ensure matching data types.


## ITEM:
Common data types:


## ITEM:
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


## ITEM:
_____________________________________
_____________________________________
_____________________________________
Basic Concepts


## ITEM:
Models


## ITEM:
Models are essential


## ITEM:
Models are essential building blocks for media generation
workflows. They can be combined and mixed to achieve diﬀerent
creative eﬀects.


## ITEM:
The word model has many diﬀerent meanings. Here, it means a
data file carrying information that is required for a node graph to
do its work. Specifically, it’s a data structure that models some
function. As a verb, to model something means to represent it or
provide an example.


## ITEM:
The primary example of a model data file in ComfyUI is an AI
diﬀusion model. This is a large set of data that represents the
complex relationships among text strings and images, making it
possible to translate words into pictures or vice versa. Other
examples of common models used for image generation are
multimodal vision and language models such as CLIP, and
upscaling models such as RealESRGAN.


## ITEM:
Model files


## ITEM:
Using Models in ComfyUI


## ITEM:
1. Download and place them in the ComfyUI program directory


## ITEM:
1. Within the models folder, you’ll find subfolders for
various types of models, such as checkpoints


## ITEM:
2. In your workflow, create the node appropriate to the model
type, e.g. Load Checkpoint, Load LoRA, Load VAE


## ITEM:
3. In the loader node, choose the model you wish to use


## ITEM:
4. Connect the loader node to other nodes in your workflow


## ITEM:
Adding Extra Model Paths


## ITEM:
If you want to manage your model files outside of ComfyUI/
models, you may have the following reasons:


## ITEM:
• You have multiple ComfyUI instances and want them to
share model files to save disk space


## ITEM:
• You have diﬀerent types of GUI programs (such as WebUI)
and want them to use the same model files


## ITEM:
• Model files cannot be recognized or found


## ITEM:
We provide a way to add extra model search paths via the
extra_model_paths.yaml configuration file


## ITEM:
Open Config File


## ITEM:
├── 📁 models/


## ITEM:
|   ├── 📁  lora/


## ITEM:
|   │   └── xxxxx.safetensors


## ITEM:
|   ├── 📁  checkpoints/


## ITEM:
|   │   └── xxxxx.safetensors


## ITEM:
|   ├── 📁  vae/


## ITEM:
|   │   └── xxxxx.safetensors


## ITEM:
|   └── 📁  controlnet/


## ITEM:
|       └── xxxxx.safetensors


## ITEM:
Then you can configure the extra_model_paths.yaml file like
below to let ComfyUI recognize the model paths on your device:


## ITEM:
Copy


## ITEM:
Ask AI


## ITEM:
my_custom_config:


## ITEM:
base_path: YOUR_PATH


## ITEM:
loras: models/loras/


## ITEM:
checkpoints: models/checkpoints/


## ITEM:
vae: models/vae/


## ITEM:
controlnet: models/controlnet/


## ITEM:
or


## ITEM:
Copy


## ITEM:
Ask AI


## ITEM:
my_custom_config:


## ITEM:
base_path: YOUR_PATH/models/


## ITEM:
loras: loras


## ITEM:
checkpoints: checkpoints


## ITEM:
vae: vae


## ITEM:
controlnet: controlnet


## ITEM:
checkpoints: models/Stable-diﬀusion


## ITEM:
configs: models/Stable-diﬀusion


## ITEM:
vae: models/VAE


## ITEM:
loras: |


## ITEM:
models/Lora


## ITEM:
models/LyCORIS


## ITEM:
upscale_models: |


## ITEM:
models/ESRGAN


## ITEM:
models/RealESRGAN


## ITEM:
models/SwinIR


## ITEM:
embeddings: embeddings


## ITEM:
hypernetworks: models/hypernetworks


## ITEM:
controlnet: models/ControlNet


## ITEM:
#config for comfyui


## ITEM:
#your base path should be either an existing comfy install or a central
folder where you store all of your models, loras, etc.


## ITEM:
#comfyui:


## ITEM:
```bash
#     base_path: path/to/comfyui/
```


## ITEM:
```bash
#     # You can use is_default to mark that these folders should be listed
first, and used as the default dirs for eg downloads
```


## ITEM:
```bash
#     #is_default: true
```


## ITEM:
```bash
#     checkpoints: models/checkpoints/
```


## ITEM:
```bash
#     clip: models/clip/
```


## ITEM:
```bash
#     clip_vision: models/clip_vision/
```


## ITEM:
```bash
#     configs: models/configs/
```


## ITEM:
```bash
#     controlnet: models/controlnet/
```


## ITEM:
```bash
#     diﬀusion_models: |
```


## ITEM:
```bash
#                  models/diﬀusion_models
```


## ITEM:
```bash
#                  models/unet
```


## ITEM:
```bash
#     embeddings: models/embeddings/
```


## ITEM:
```bash
#     loras: models/loras/
```


## ITEM:
```bash
#     upscale_models: models/upscale_models/
```


## ITEM:
```bash
#     vae: models/vae/
```


## ITEM:
#other_ui:


## ITEM:
```bash
#    base_path: path/to/ui
```


## ITEM:
```bash
#    checkpoints: models/checkpoints
```


## ITEM:
```bash
#    gligen: models/gligen
```


## ITEM:
```bash
#    custom_nodes: path/custom_nodes
```


## ITEM:
For example, if your WebUI is located at D:\stable-diﬀusion-
webui\, you can modify the corresponding configuration to


## ITEM:
Copy


## ITEM:
Ask AI


## ITEM:
a111:


## ITEM:
base_path: D:\stable-diﬀusion-webui\


## ITEM:
checkpoints: models/Stable-diﬀusion


## ITEM:
configs: models/Stable-diﬀusion


## ITEM:
vae: models/VAE


## ITEM:
loras: |


## ITEM:
models/Lora


## ITEM:
models/LyCORIS


## ITEM:
upscale_models: |


## ITEM:
models/ESRGAN


## ITEM:
models/RealESRGAN


## ITEM:
models/SwinIR


## ITEM:
embeddings: embeddings


## ITEM:
hypernetworks: models/hypernetworks


## ITEM:
controlnet: models/ControlNet


## ITEM:
my_custom_nodes:


## ITEM:
custom_nodes: /Users/your_username/Documents/extra_custom_nodes


## ITEM:
File size


## ITEM:
Models can be extremely large files relative to image files. A
typical uncompressed image may require a few megabytes of
disk storage. Generative AI models can be tens of thousands of
times larger, up to tens of gigabytes per model. They take up a
great deal of disk space and take a long time to transfer over a
network.


## ITEM:
Model training and refinement


## ITEM:
A generative AI model is created by training a machine learning
program on a very large set of data, such as pairs of images and
text descriptions. An AI model doesn’t store the training data


## ITEM:
explicitly, but rather it stores the correlations that are implicit
within the data.


## ITEM:
Organizations and companies such as Stability AI and Black
Forest Labs release “base” models that carry large amounts of
generic information. These are general purpose generative AI
models. Commonly, the base models need to be refined in order
to get high quality generative outputs. A dedicated community of
people work to refine the base models. The new, refined models
produce better output, provide new or diﬀerent functionality, and/
or use fewer resources. Refined models can usually be run on
systems with less computing power and/or memory.


## ITEM:
Auxiliary models


## ITEM:
_____________________________________
_____________________________________
_____________________________________
Basic Concepts


## ITEM:
Dependencies


## ITEM:
Understand dependencies in ComfyUI


## ITEM:
A workflow file depends on other files


## ITEM:
We often obtain various workflow files from the community, but frequently find that the
workflow cannot run directly after loading. This is because a workflow file depends on
other files besides the workflow itself, such as media asset inputs, models, custom


## ITEM:
nodes, related Python dependencies, etc. ComfyUI workflows can only run normally
when all relevant dependencies are satisfied.


## ITEM:
ComfyUI workflow dependencies mainly fall into the following categories:


## ITEM:
• Assets (media files including audio, video, images, and other inputs)


## ITEM:
• Python dependencies


## ITEM:
• Models (such as Stable Diﬀusion models, etc.)


## ITEM:
Assets


## ITEM:
An AI model is an example of an asset. In media production, an asset is some media
file that supplies input data. For example, a video editing program operates on movie
files stored on disk. The editing program’s project file holds links to these movie file
assets, allowing non-destructive editing that doesn’t alter the original movie files.


## ITEM:
ComfyUI works the same way. A workflow can only run if all of the required assets are
found and loaded. Generative AI models, images, movies, and sounds are some
examples of assets that a workflow might depend upon. These are therefore known as
dependent assets or asset dependencies.


## ITEM:
Python Dependencies


## ITEM:
ComfyUI is a Python-based project. We build a standalone Python environment to run
ComfyUI, and all related dependencies are installed in this isolated Python
environment.


## ITEM:
ComfyUI Dependencies


## ITEM:
You can view ComfyUI’s current dependencies in the requirements.txt file:


## ITEM:
Copy


## ITEM:
Ask AI


## ITEM:
comfyui-frontend-package==1.14.5


## ITEM:
torch


## ITEM:
torchsde


## ITEM:
torchvision


## ITEM:
torchaudio


## ITEM:
numpy>=1.25.0


## ITEM:
einops


## ITEM:
transformers>=4.28.1


## ITEM:
tokenizers>=0.13.3


## ITEM:
sentencepiece


## ITEM:
safetensors>=0.4.2


## ITEM:
aiohttp>=3.11.8


## ITEM:
yarl>=1.18.0


## ITEM:
pyyaml


## ITEM:
Pillow


## ITEM:
scipy


## ITEM:
tqdm


## ITEM:
psutil


## ITEM:
#non essential dependencies:


## ITEM:
kornia>=0.7.1


## ITEM:
spandrel


## ITEM:
soundfile


## ITEM:
av


## ITEM:
As ComfyUI evolves, we may adjust dependencies accordingly, such as adding new
dependencies or removing ones that are no longer needed. So if you use Git to update
ComfyUI, you need to run the following command in the corresponding environment
after pulling the latest updates:


## ITEM:
Copy


## ITEM:
Ask AI


## ITEM:
```bash
pip install -r requirements.txt
```


## ITEM:
This ensures that ComfyUI’s dependencies are up to date for proper operation. You can
also modify specific package dependency versions to upgrade or downgrade certain
dependencies.


## ITEM:
Additionally, ComfyUI’s frontend ComfyUI_frontend is currently maintained as a
separate project. We update the comfyui-frontend-package dependency version after
the corresponding version stabilizes. If you need to switch to a diﬀerent frontend
version, you can check the version information here.


## ITEM:
You need to navigate to the corresponding plugin directory in your ComfyUI Python
environment and run pip install -r requirements.txt to install the dependencies.


## ITEM:
python_embeded\python.exe -m pip install -r
ComfyUI\custom_nodes\<custom_node_name>\requirements.txt


## ITEM:
to install the dependencies for the corresponding node.


## ITEM:
Dependency Conflicts


## ITEM:
• You can try manually installing specific versions of dependencies in the Python
virtual environment to resolve such issues.


## ITEM:
• Or create diﬀerent Python virtual environments for diﬀerent plugins to resolve
these issues.


## ITEM:
These types of dependency conflicts may be more diﬃcult to resolve, and you may
need to upgrade/downgrade ComfyUI or change the dependency versions of custom
nodes to resolve these issues.


## ITEM:
Models


## ITEM:
• Natively supported model workflows


## ITEM:
1. Load a template: Click any template you want to load its workflow.


## ITEM:
2. Download models: When loading a template, ComfyUI automatically checks
whether all required model files exist. If anything is missing, it will prompt you to
download the models.


## ITEM:
3. Run the workflow: Once all requirements—such as models, input images, and
prompts—are ready, click the Run button to start using the workflow.


## ITEM:
Model storage location


## ITEM:
Each workflow template embeds links to the required models. On first use, if the
corresponding model files are not detected, you will see a download prompt.


## ITEM:
1. For desktop version, when you click the Download button, the desktop program
will automatically download the model files for you.


## ITEM:
2. For other versions, the browser will be used to download the corresponding
model. You need to download the model and save it to the corresponding folder
under ComfyUI/models. For example, the model in the screenshot should be
saved in the following location:


## ITEM:
Copy


## ITEM:
Ask AI


## ITEM:
📂  ComfyUI/


## ITEM:
├── 📂  models/


## ITEM:
│   ├── 📂  diﬀusion_models/


## ITEM:
│   │   └── qwen_image_fp8_e4m3fn.safetensors


## ITEM:
│   ├── 📂  vae/


## ITEM:
│   │   └── qwen_image_vae.safetensors


## ITEM:
│   └── 📂  text_encoders/


## ITEM:
│       └── qwen_2.5_vl_7b_fp8_scaled.safetensors


## ITEM:
In the current version, missing-file detection only checks whether there is a file with the
same name in the corresponding top-level directory. For example, the file must exist
directly under ComfyUI/models/diﬀusion_models. If you have already downloaded the
model into a subfolder such as ComfyUI/models/diﬀusion_models/wan_video, you can
ignore the popup and simply ensure the correct model is selected in the corresponding
model loader node.


## ITEM:
If you’re curious how model links are embedded, we add a models field under the
node’s properties. Below is a complete snippet of a DualCLIPLoader node with
embedded model information:


## ITEM:
Copy


## ITEM:
Ask AI


## ITEM:
{


## ITEM:
"id": 40,


## ITEM:
"type": "DualCLIPLoader",


## ITEM:
"pos": [


## ITEM:
-320,


## ITEM:
290


## ITEM:
],


## ITEM:
"size": [


## ITEM:
270,


## ITEM:
130


## ITEM:
],


## ITEM:
"flags": {},


## ITEM:
"order": 0,


## ITEM:
"mode": 0,


## ITEM:
"inputs": [],


## ITEM:
"outputs": [


## ITEM:
{


## ITEM:
"name": "CLIP",


## ITEM:
"type": "CLIP",


## ITEM:
"links": [


## ITEM:
64


## ITEM:
]


## ITEM:
}


## ITEM:
],


## ITEM:
"properties": {


## ITEM:
"Node name for S&R": "DualCLIPLoader",


## ITEM:
"cnr_id": "comfy-core",


## ITEM:
"ver": "0.3.40",


## ITEM:
"models": [


## ITEM:
{


## ITEM:
"name": "clip_l.safetensors",


## ITEM:
"url": "https://huggingface.co/comfyanonymous/flux_text_encoders/resolve/
main/clip_l.safetensors",


## ITEM:
"directory": "text_encoders"


## ITEM:
},


## ITEM:
{


## ITEM:
"name": "t5xxl_fp16.safetensors",


## ITEM:
"url": "https://huggingface.co/comfyanonymous/flux_text_encoders/resolve/
main/t5xxl_fp16.safetensors",


## ITEM:
"directory": "text_encoders"


## ITEM:
}


## ITEM:
]


## ITEM:
},


## ITEM:
"widgets_values": [


## ITEM:
"clip_l.safetensors",


## ITEM:
"t5xxl_fp16.safetensors",


## ITEM:
"flux",


## ITEM:
"default"


## ITEM:
]


## ITEM:
}


## ITEM:
The models field inside properties includes name, url, and directory.


## ITEM:
• 	 name: the model file name


## ITEM:
• 	 url: a direct download link to the file (not a repository page)


## ITEM:
• 	 directory: which subfolder under ComfyUI/models to store the file, e.g.
vae means ComfyUI/models/vae


## ITEM:
Currently, only links from Hugging Face and Civitai are supported. The model format
must be a safe format such as .safetensors or .sft. Formats like .gguf are considered
unsafe; when embedded they will be flagged as unsafe and the link will not be shown.


## ITEM:
Typically, the following three dependencies may be upgraded together when ComfyUI
is updated:


## ITEM:
Copy


## ITEM:
Ask AI


## ITEM:
comfyui-frontend-package==1.24.4


## ITEM:
If you’re not sure how to update correctly, see Update ComfyUI for how to update
ComfyUI and its dependencies.


## ITEM:
How to contribute templates to the ComfyUI repository?


## ITEM:
Subgraph - Simplify your workflow


## ITEM:
An introduction to the Subgraph feature in ComfyUI, including how to create, navigate,
and manage subgraphs.


## ITEM:
The subgraph feature requires ComfyUI frontend version 1.24.3 or later. If you don’t see
this feature, please refer to: How to Update ComfyUI


## ITEM:
• 	Images in this document are made with nightly version frontend, please refer to
the actual interface


## ITEM:
• 	Some features like converting subgraph back to nodes will be supported in the
future


## ITEM:
Comfy Org


## ITEM:
5.7K subscribers


## ITEM:
Subgraph Oﬃcial Release! Making Complex Workflows Clean and Eﬃcient


## ITEM:
Share


## ITEM:
Watch on


## ITEM:
A subgraph is a powerful ComfyUI feature that lets you package complex workflows
into a single reusable subgraph node, making them easier to manage and share.


## ITEM:
Think of a subgraph as a “folder” for your workflow – you can group related nodes
together and use the entire collection as one unified subgraph node.


## ITEM:
Use subgraphs to:


## ITEM:
• Simplify complex workflows


## ITEM:
• Reuse common node combinations


## ITEM:
• Build more eﬃcient workflows with modular components


## ITEM:
Creating a Subgraph


## ITEM:
1


## ITEM:
Select nodes


## ITEM:
Select the nodes you want to group in ComfyUI


## ITEM:
2


## ITEM:
Click the subgraph icon


## ITEM:
Find the subgraph icon in the toolbar


## ITEM:
3


## ITEM:
Subgraph created


## ITEM:
ComfyUI automatically creates a subgraph based on your selected nodes’ inputs and
outputs


## ITEM:
4


## ITEM:
Customize your subgraph


## ITEM:
Refer to Editing Subgraphs, you can edit and organize the subgraph to create a fully
functional node


## ITEM:
Working with Subgraphs


## ITEM:
Basic Operations


## ITEM:
Subgraphs work just like regular nodes. You can:


## ITEM:
• Change colors and names


## ITEM:
• Use bypass to disable


## ITEM:
• Apply all standard node operations


## ITEM:
Editing Subgraphs


## ITEM:
To enter edit mode:


## ITEM:
• Double-click the empty area inside the subgraph (not on widgets), or


## ITEM:
• Click the subgraph edit button


## ITEM:
In edit mode you’ll see:


## ITEM:
1. 	Navigation bar: Exit the current subgraph and return to the parent level


## ITEM:
2. 	Input slots: Internal node inputs exposed to the outside


## ITEM:
• 	Connect outputs to slots like normal nodes


## ITEM:
• 	Right-click connection points to rename/delete exposed slots


## ITEM:
3. 	Output slots: Outputs exposed to the outside (same functionality as input slots)


## ITEM:
Working with slots:


## ITEM:
1. Default slot (labeled 1): Use this to add new input/output connections


## ITEM:
2. Right-click existing slots to rename, delete, or disconnect from original nodes


## ITEM:
Note: Slot connections follow standard data type validation rules


## ITEM:
Nested Subgraphs


## ITEM:
Create even more complex workflows by nesting subgraphs within subgraphs.


## ITEM:
The navigation bar shows your current level and lets you easily move between nested
subgraphs.


## ITEM:
Partial Execution - Run Only Part
of Your workflow in ComfyUI


## ITEM:
How to use and the requirements for the Partial Execution
feature in ComfyUI


## ITEM:
The Partial Execution feature is located in the ComfyUI node
selection toolbox. It allows you to run only a part of your
workflow instead of executing all nodes. This feature is only
available when the selected node is an output node, and when
available, it appears as a green triangle icon.


## ITEM:
What is Partial Execution?


## ITEM:
Partial Execution, as the name suggests, lets you run only a part
of your workflow instead of executing all nodes in the workflow.


## ITEM:
The diagram above compares Partial Execution and running the
entire workflow:


## ITEM:
1. Partial Execution (left): Only runs the branch of the workflow
from the starting node to the output node.


## ITEM:
2. Run Workflow (right): Runs all nodes in the workflow.


## ITEM:
This feature allows you to flexibly execute specific parts of your
workflow, rather than running the entire workflow every time.


## ITEM:
How to Use the Partial Execution Feature?


## ITEM:
To use the Partial Execution feature, the currently selected node
must be an output node, such as preview or save nodes. When
the corresponding node meets the criteria, after selecting the
node, the button in the toolbox will display as a green triangle
icon. Click this icon to run the partial workflow.


## ITEM:
Common Issues


## ITEM:
1. User - User settings related to ComfyUI account, mainly used
for logging into ComfyUI account to use API nodes


## ITEM:
2. Credits - Entry for purchasing credits and credit balance
history, only visible after logging into ComfyUI account


## ITEM:
3. Comfy - Detailed description of ComfyUI core setting options


## ITEM:
The account system was added to support API Nodes, which enable calls to closed-
source model APIs, greatly expanding the possibilities of ComfyUI. Since these API
calls consume tokens, we have added a corresponding user system.


## ITEM:
Currently, we support the following login methods:


## ITEM:
• Email login


## ITEM:
• Google login


## ITEM:
• Github login


## ITEM:
• API Key login (for non-whitelisted site authorization)


## ITEM:
We will provide relevant login requirements and explanations in this document.


## ITEM:
ComfyUI Version Requirements


## ITEM:
The credit system was added to support the API Nodes, as calling closed-source AI
models requires token consumption, so proper credit management is necessary. By
default, the credits interface is not displayed. Please first log in to your ComfyUI
account in Settings -> User, and then you can view your associated account’s credit
information in Settings -> Credits.


## ITEM:
ComfyUI will always remain fully open-source and free for local users.


## ITEM:
How to Purchase Credits?


## ITEM:
Below is a demonstration video for purchasing credits:


## ITEM:
Detailed steps are as follows:


## ITEM:
1


## ITEM:
Log in to your ComfyUI account


## ITEM:
Log in to your ComfyUI account in Settings -> User


## ITEM:
2


## ITEM:
Go to `Settings` -> `Credits` to purchase credits


## ITEM:
After logging in, you should see the Credits option added to the menu


## ITEM:
Go to Settings -> Credits to purchase credits


## ITEM:
3


## ITEM:
Set the amount of credits to purchase


## ITEM:
In the popup, set the purchase amount and click the Buy button


## ITEM:
4


## ITEM:
Make payment through Stripe


## ITEM:
On the payment page, please follow these steps:


## ITEM:
1. Select the currency for payment


## ITEM:
2. Confirm that the email is the same as your ComfyUI registration email


## ITEM:
3. Choose your payment method


## ITEM:
• Credit Card


## ITEM:
• WeChat (only supported when paying in USD)


## ITEM:
• Alipay (only supported when paying in USD)


## ITEM:
4. Click the Pay button or the Generate QR Code button to complete the payment
process


## ITEM:
5


## ITEM:
Complete payment and check your credit balance


## ITEM:
After completing the payment, please return to Menu -> Credits to check if your
balance has been updated. Try refreshing the interface or restarting if necessary


## ITEM:
A: No, when your credit balance is negative, you will not be able to run API Nodes


## ITEM:
Q: Can I get a refund for unused credits?


## ITEM:
A: Currently, we do not support refunds


## ITEM:
Q: How do I check my current balance and usage?


## ITEM:
A: Click on Settings -> Credits to see your current balance and access the Credit
History entry


## ITEM:
Q: Can I share my credits with other users?


## ITEM:
A: You can log into the same account on multiple devices, but we do not support
sharing credits with other users


## ITEM:
Q: How do I know how many credits I've consumed each time?


## ITEM:
A: Due to diﬀerent image sizes and generation quantities, the Tokens and Credits
consumed each time vary. In Settings -> Credits, you can see the credits consumed
each time and the corresponding credit history


## ITEM:
Q: Why don't I see WeChat or Alipay payment options?


## ITEM:
A: Please ensure you are paying in USD, as WeChat and Alipay are only supported
when paying in USD


## ITEM:
```bash
# Section: Comfy
```


## ITEM:
API Nodes


## ITEM:
Show API node pricing badge


## ITEM:
• 	Default Value: Enabled


## ITEM:
• 	Function: Controls whether to display pricing badges on API nodes, helping
users identify the usage cost of API nodes


## ITEM:
For more information about API nodes, please refer to API Nodes


## ITEM:
Dev Mode


## ITEM:
Enable dev mode options (API save, etc.)


## ITEM:
• 	Default Value: Disabled


## ITEM:
• 	Function: Enables development mode options (such as API save, etc.)


## ITEM:
Edit Token Weight


## ITEM:
Ctrl+up/down precision


## ITEM:
• 	Default Value: 0.01


## ITEM:
• 	Function: When using CLIPTextEncode type nodes or text input node widgets,
use Ctrl+up/down to quickly adjust weights. This option changes the weight
value for each adjustment


## ITEM:
Locale


## ITEM:
Language


## ITEM:
• 	Options: English, 中⽂ (Chinese),⽇本語 (Japanese), 한국어 (Korean), Русский
(Russian), Español (Spanish), Français (French)


## ITEM:
• 	Default Value: Auto-detect browser language


## ITEM:
• 	Function: Modify the display language of ComfyUI interface


## ITEM:
Menu


## ITEM:
Use new menu


## ITEM:
• 	Default Value: Top


## ITEM:
• 	Function: Select menu interface and position, currently only supports Top,
Bottom, Disabled


## ITEM:
• 	Top


## ITEM:
• 	Bottom


## ITEM:
• 	Disabled


## ITEM:
The menu interface will be displayed at the top of the workspace


## ITEM:
Model Library


## ITEM:
Model Library refers to the model management function in the ComfyUI sidebar menu.
You can use this function to view models in your ComfyUI/models and additionally
configured model folders.


## ITEM:
What name to display in the model library tree view


## ITEM:
• 	Default Value: title


## ITEM:
• 	Function: Select the name format to display in the model library tree view,
currently only supports filename and title


## ITEM:
Automatically load all model folders


## ITEM:
• 	Default Value: Disabled


## ITEM:
• 	Function: Whether to automatically detect model files in all folders when clicking
the model library. Enabling may cause loading delays (requires traversing all
folders). When disabled, files in the corresponding folder will only be loaded
when clicking the folder name.


## ITEM:
Node


## ITEM:
During the iteration process of ComfyUI, we will adjust some nodes and enable some
nodes. These nodes may undergo major changes or be removed in future versions.
However, to ensure compatibility, deprecated nodes have not been removed. You can
use the settings below to enable whether to display experimental nodes and
deprecated nodes.


## ITEM:
Show deprecated nodes in search


## ITEM:
• 	Default Value: Disabled


## ITEM:
• 	Function: Controls whether to display deprecated nodes in search. Deprecated
nodes are hidden by default in the UI, but remain eﬀective in existing workflows.


## ITEM:
Show experimental nodes in search


## ITEM:
• 	Default Value: Enabled


## ITEM:
• 	Function: Controls whether to display experimental nodes in search.
Experimental nodes are some new feature support, but are not fully stable and
may change or be removed in future versions.


## ITEM:
Node Search Box


## ITEM:
Number of nodes suggestions


## ITEM:
• 	Default Value: 5


## ITEM:
• 	Function: Used to modify the number of recommended nodes in the related
node context menu. The larger the value, the more related recommended nodes
are displayed.


## ITEM:
Show node frequency in search results


## ITEM:
• 	Default Value: Disabled


## ITEM:
• 	Function: Controls whether to display node usage frequency in search results


## ITEM:
Show node id name in search results


## ITEM:
• 	Default Value: Disabled


## ITEM:
• 	Function: Controls whether to display node ID names in search results


## ITEM:
Show node category in search results


## ITEM:
• 	Default Value: Enabled


## ITEM:
• 	Function: Controls whether to display node categories in search results, helping
users understand node classification information


## ITEM:
Node preview


## ITEM:
• 	Default Value: Enabled


## ITEM:
• 	Function: Controls whether to display node previews in search results, making it
convenient for you to quickly preview nodes


## ITEM:
Node search box implementation


## ITEM:
• 	Default Value: default


## ITEM:
• 	Function: Controls whether the timing of node widget value updates is before or
after workflow execution, such as updating seed values


## ITEM:
Textarea widget spellcheck


## ITEM:
• 	Default Value: Disabled


## ITEM:
• 	Function: Controls whether text area widgets enable spellcheck, providing
spellcheck functionality during text input. This functionality is implemented
through the browser’s spellcheck attribute


## ITEM:
Queue


## ITEM:
Queue history size


## ITEM:
• 	Default Value: 100


## ITEM:
• 	Function: Controls the queue history size recorded in the sidebar queue history
panel. The larger the value, the more queue history is recorded. When the
number is large, loading the page will also consume more memory


## ITEM:
Queue Button


## ITEM:
Batch count limit


## ITEM:
• 	Default Value: 100


## ITEM:
• 	Function: Sets the maximum number of tasks added to the queue in a single
click, preventing accidentally adding too many tasks to the queue


## ITEM:
Validation


## ITEM:
Validate node definitions (slow)


## ITEM:
• 	Default Value: Disabled


## ITEM:
• 	Function: Controls whether to validate all node definitions at startup (slow). Only
recommended for node developers. When enabled, the system will use Zod
schemas to strictly validate each node definition. This functionality will consume
more memory and time


## ITEM:
• 	Error Handling: Failed node definitions will be skipped and warning information
will be output to the console


## ITEM:
Since detailed schema validation needs to be performed on all node definitions, this
feature will significantly increase startup time, so it is disabled by default and only
recommended for node developers


## ITEM:
Validate workflows


## ITEM:
• 	Default Value: Enabled


## ITEM:
• 	Function: Ensures the structural and connection correctness of workflows. If
enabled, the system will call useWorkflowValidation().validateWorkflow() to
validate workflow data


## ITEM:
• 	Validation Process: The validation process includes two steps:


## ITEM:
• 	Schema validation: Use Zod schemas to validate workflow structure


## ITEM:
• 	Link repair: Check and repair connection issues between nodes


## ITEM:
• 	Error Handling: When validation fails, error prompts will be displayed, but
workflow loading will not be blocked


## ITEM:
Window


## ITEM:
Show confirmation when closing window


## ITEM:
• 	Default Value: Enabled


## ITEM:
• 	Function: When there are modified but unsaved workflows, controls whether to
display confirmation when closing the browser window or tab, preventing
accidental window closure that leads to loss of unsaved workflows


## ITEM:
Workflow


## ITEM:
Persist workflow state and restore on page (re)load


## ITEM:
• 	Default Value: Enabled


## ITEM:
• 	Function: Controls whether to restore workflow state on page (re)load,
maintaining workflow content after page refresh


## ITEM:
Auto Save


## ITEM:
• 	Default Value: oﬀ


## ITEM:
• 	Function: Controls the auto-save behavior of workflows, automatically saving
workflow changes to avoid data loss


## ITEM:
Auto Save Delay (ms)


## ITEM:
• 	Default Value: 1000


## ITEM:
• 	Function: Sets the delay time for auto-save, only eﬀective when auto-save is set
to “after delay”


## ITEM:
Show confirmation when deleting workflows


## ITEM:
• 	Default Value: Enabled


## ITEM:
• 	Function: Controls whether to display a confirmation dialog when deleting
workflows in the sidebar, preventing accidental deletion of important workflows


## ITEM:
Opened workflows position


## ITEM:
• 	Options: Sidebar, Topbar, Topbar (Second Row)


## ITEM:
• 	Default Value: Topbar


## ITEM:
• 	Function: Controls the display position of opened workflow tabs, currently only
supports Sidebar, Topbar, Topbar (Second Row)


## ITEM:
Prompt for filename when saving workflow


## ITEM:
• 	Default Value: Enabled


## ITEM:
• 	Function: Controls whether to prompt for filename input when saving workflows,
allowing users to customize workflow filenames


## ITEM:
Sort node IDs when saving workflow


## ITEM:
• 	Default Value: Disabled


## ITEM:
• 	Function: Determines whether to sort node IDs when saving workflows, making
workflow file format more standardized and convenient for version control


## ITEM:
Show missing nodes warning


## ITEM:
• 	Default Value: Enabled


## ITEM:
• 	Function: Controls whether to display warnings for missing nodes in workflows,
helping users identify unavailable nodes in workflows


## ITEM:
Show missing models warning


## ITEM:
• 	Default Value: Enabled


## ITEM:
• 	Function: We support adding model link information to widget values in
workflow files for prompts when loading model files. When enabled, if you don’t
have the corresponding model files locally, warnings for missing models in
workflows will be displayed


## ITEM:
Require confirmation when clearing workflow


## ITEM:
• 	Default Value: Enabled


## ITEM:
• 	Function: Controls whether to display a confirmation dialog when clearing
workflows, preventing accidental clearing of workflow content


## ITEM:
Save node IDs to workflow


## ITEM:
• 	Default Value: Enabled


## ITEM:
• 	Function: Controls whether to save node IDs when saving workflows, making
workflow file format more standardized and convenient for version control


## ITEM:
```bash
# Section: Lite Graph
```


## ITEM:
• 	Function: The selection toolbox is a floating quick action toolbar that appears on
nodes after they are selected, providing common quick operations such as
partial execution, pinning, deletion, color modification, etc.


## ITEM:
Low quality rendering zoom threshold


## ITEM:
• 	Default Value: 0.6


## ITEM:
• 	Range: 0.1 - 1.0


## ITEM:
• 	Function: When auto-snap is enabled or when moving nodes while holding the
Shift key, this parameter determines the grid size for snapping. The default value
is 10, and you can adjust it according to your needs.


## ITEM:
Enable fast-zoom shortcut (Ctrl + Shift + Drag)


## ITEM:
• 	Default Value: Enabled


## ITEM:
• 	Function: Enables the Ctrl + Shift + Left Mouse Button Drag fast zoom function,
providing a faster zoom operation method


## ITEM:
• 	Function: Sets the rendering style of connections, controlling the visual style of
links between nodes


## ITEM:
Group


## ITEM:
This section of settings is mainly related to node group functionality


## ITEM:
Double click group title to edit


## ITEM:
• 	Default Value: Enabled


## ITEM:
• 	Function: Controls whether you can double-click the node title to edit it, allowing
users to rename nodes, marked as part 1 in the image


## ITEM:
Group selected nodes padding


## ITEM:
• 	Default Value: 10


## ITEM:
• 	Range: 0 - 100


## ITEM:
• 	Function: Sets the inner padding when grouping selected nodes, controlling the
spacing between the group frame and nodes, marked as the arrow annotation
part 2 in the image


## ITEM:
Link


## ITEM:
Link midpoint markers


## ITEM:
• 	Default Value: Circle


## ITEM:
• 	Options: None, Circle, Arrow


## ITEM:
• 	Function: Sets the marker style at link midpoints, displaying direction indicators
at link midpoints


## ITEM:
Link Release


## ITEM:
This menu section currently mainly controls related operations when link connections
are released. The current two related operations are:


## ITEM:
A node recommendation list related to the current input/output will appear after release


## ITEM:
A search box will be launched after release


## ITEM:
Action on link release (Shift)


## ITEM:
• 	Default Value: search box


## ITEM:
• 	Options: context menu, search box, no action


## ITEM:
• 	Function: Sets the action when releasing links while holding the Shift key,
special behavior when releasing links while holding Shift


## ITEM:
Action on link release (No modifier)


## ITEM:
• 	Default Value: context menu


## ITEM:
• 	Options: context menu, search box, no action


## ITEM:
• 	Function: Sets the default action when releasing links, controls the behavior
after dragging and releasing links


## ITEM:
Node


## ITEM:
Always shrink new nodes


## ITEM:
• 	Default Value: Enabled


## ITEM:
• 	Function: Controls whether to automatically shrink when creating new nodes, so
nodes can always display the minimum size, but may cause some text display to
be truncated when adding, requiring manual adjustment of node size


## ITEM:
Enable DOM element clipping (enabling may reduce performance)


## ITEM:
• 	Default Value: Enabled


## ITEM:
• 	Function: Enables DOM element clipping (may aﬀect performance), optimizes
rendering but may reduce performance


## ITEM:
Middle-click creates a new Reroute node


## ITEM:
• 	Default Value: Enabled


## ITEM:
• 	Function: Creates a new reroute node when middle-clicking, quickly creates
reroute nodes for organizing connections


## ITEM:
Keep all links when deleting nodes


## ITEM:
• 	Default Value: Enabled


## ITEM:
• 	Function: Automatically bypasses connections when deleting intermediate
nodes, attempts to reconnect input and output links when deleting nodes


## ITEM:
Snap highlights node


## ITEM:
• 	Default Value: Enabled


## ITEM:
• 	Function: Highlights nodes when dragging links to them, provides visual
feedback, shows connectable nodes. When enabled, the eﬀect is as shown in
the image below, the corresponding side of the link will display highlighted style


## ITEM:
Auto snap link to node slot


## ITEM:
• 	Default Value: Enabled


## ITEM:
• 	Function: Automatically snaps to available slots when dragging links to nodes,
simplifies connection operations, automatically finds suitable input slots


## ITEM:
Enable Tooltips


## ITEM:
• 	Default Value: Enabled


## ITEM:
• 	Function: Some node information will contain tooltips, including parameter
descriptions, etc. When enabled, these tooltips will be displayed when hovering
the mouse, as shown in the image below


## ITEM:
Tooltip Delay


## ITEM:
• 	Default Value: 500


## ITEM:
• 	Function: Controls the delay time for tooltips, in milliseconds. Setting to 0 means
displaying tooltips immediately


## ITEM:
Node life cycle badge mode


## ITEM:
• 	Default Value: Show all


## ITEM:
• 	Function: Controls the display of node lifecycle markers, showing node status
information


## ITEM:
Node ID badge mode


## ITEM:
• 	Default Value: Show all


## ITEM:
• 	Function: Controls the display of node ID markers, showing node unique
identifiers


## ITEM:
Node source badge mode


## ITEM:
• 	Options:


## ITEM:
• 	None


## ITEM:
• 	Hide built-in


## ITEM:
• 	Show all


## ITEM:
• 	Function: Controls whether you can double-click the node title to edit it, allowing
users to rename nodes


## ITEM:
Node Widget


## ITEM:
Float widget rounding decimal places [0 = auto]


## ITEM:
• 	Default Value: 0 (auto)


## ITEM:
• 	Range: 0 - 6


## ITEM:
• 	Function: Sets the decimal places for float widget rounding, 0 means auto,
requires page reload


## ITEM:
Disable default float widget rounding


## ITEM:
• 	Default Value: Disabled


## ITEM:
• 	Function: Controls whether to disable default float widget rounding, requires
page reload, cannot be disabled when the node backend has set rounding


## ITEM:
Disable node widget sliders


## ITEM:
• 	Default Value: Disabled


## ITEM:
• 	Function: Controls whether to disable slider controls in node widgets, forcing
text input instead of sliders


## ITEM:
Preview image format


## ITEM:
• 	Default Value: Empty string (use original format)


## ITEM:
• 	Function: Sets the format for preview images in image widgets, converts to
lightweight formats like webp, jpeg, etc.


## ITEM:
Show width × height below the image preview


## ITEM:
• 	Default Value: Enabled


## ITEM:
• 	Function: Displays width × height information below image previews, showing
image dimension information


## ITEM:
Pointer


## ITEM:
Enable trackpad gestures


## ITEM:
• 	Default Value: Enabled


## ITEM:
• 	Function: Used to determine the smoothness of curves on both sides of reroute
nodes. Larger values make curves smoother, smaller values make curves
sharper.


## ITEM:
```bash
# Section: Appearance
```


## ITEM:
The color palette allows you to modify many specific properties. Here are some of the
most commonly customized elements, with colors represented in hexadecimal format:


## ITEM:
1. The JSON comments below are for illustration only. Do not copy the content
below for modification as it will cause the theme to malfunction.


## ITEM:
2. Since we are still iterating frequently, the content below may change with
ComfyUI frontend updates. If you need to modify, please export the theme
configuration from settings and then modify it.


## ITEM:
Copy


## ITEM:
Ask AI


## ITEM:
{


## ITEM:
"id": "dark",                     // Must be unique, cannot be the same as other theme IDs


## ITEM:
"name": "Dark (Default)",         // Theme name, displayed in theme selector


## ITEM:
"colors": {


## ITEM:
"node_slot": {                  // Node connection slot color configuration


## ITEM:
"CLIP": "#FFD500",            // CLIP model connection slot color


## ITEM:
"CLIP_VISION": "#A8DADC",     // CLIP Vision model connection slot color


## ITEM:
"CLIP_VISION_OUTPUT": "#ad7452", // CLIP Vision output connection slot color


## ITEM:
"CONDITIONING": "#FFA931",     // Conditioning control connection slot color


## ITEM:
"CONTROL_NET": "#6EE7B7",     // ControlNet model connection slot color


## ITEM:
"IMAGE": "#64B5F6",           // Image data connection slot color


## ITEM:
"LATENT": "#FF9CF9",          // Latent space connection slot color


## ITEM:
"MASK": "#81C784",            // Mask data connection slot color


## ITEM:
"MODEL": "#B39DDB",           // Model connection slot color


## ITEM:
"STYLE_MODEL": "#C2FFAE",     // Style model connection slot color


## ITEM:
"VAE": "#FF6E6E",             // VAE model connection slot color


## ITEM:
"NOISE": "#B0B0B0",           // Noise data connection slot color


## ITEM:
"GUIDER": "#66FFFF",          // Guider connection slot color


## ITEM:
"SAMPLER": "#ECB4B4",         // Sampler connection slot color


## ITEM:
"SIGMAS": "#CDFFCD",          // Sigmas data connection slot color


## ITEM:
"TAESD": "#DCC274"            // TAESD model connection slot color


## ITEM:
},


## ITEM:
• 	Function: Set the opacity of nodes, where 0 represents completely transparent
and 1 represents completely opaque.


## ITEM:
Node Widget


## ITEM:
Textarea Widget Font Size


## ITEM:
• 	Range: 8 - 24


## ITEM:
• 	Function: Set the font size in textarea widgets. Adjusts the text display size in
text input boxes to improve readability.


## ITEM:
Sidebar


## ITEM:
Unified Sidebar Width


## ITEM:
• 	Function: When enabled, the sidebar width will be unified to a consistent width
when switching between diﬀerent sidebars. If disabled, diﬀerent sidebars can
maintain their custom widths when switching.


## ITEM:
Sidebar Size


## ITEM:
• 	Function: Control the size of the sidebar, can be set to normal or small.


## ITEM:
Sidebar Location


## ITEM:
• 	Function: Control whether the sidebar is displayed on the left or right side of the
interface, allowing users to adjust the sidebar position according to their usage
habits.


## ITEM:
Tree Explorer


## ITEM:
Tree Explorer Item Padding


## ITEM:
• 	Function: Set the padding of items in the tree explorer (sidebar panel), adjusting
the spacing between items in the tree structure.


## ITEM:
Advanced Customization with user.css


## ITEM:
For cases where the color palette doesn’t provide enough control, you can use custom
CSS via a user.css file. This method is recommended for advanced users who need to
customize elements that aren’t available in the color palette system.


## ITEM:
Requirements


## ITEM:
• ComfyUI frontend version 1.20.5 or newer


## ITEM:
Setting Up user.css


## ITEM:
1. Create a file named user.css in your ComfyUI user directory (same location as
your workflows and settings - see location details below)


## ITEM:
2. Add your custom CSS rules to this file


## ITEM:
3. Restart ComfyUI or refresh the page to apply changes


## ITEM:
User Directory Location


## ITEM:
This location contains your workflows, settings, and other user-specific files.


## ITEM:
After finding the above folder location, please copy the corresponding CSS file to the
corresponding user directory, such as the default user folder being ComfyUI/user/
default, then restart ComfyUI or refresh the page to apply changes.


## ITEM:
user.css Examples and Related Instructions


## ITEM:
The user.css file is loaded early in the application startup process. So you may need to
use !important in your CSS rules to ensure they override the default styles.


## ITEM:
user.css Customization Examples


## ITEM:
Copy


## ITEM:
Ask AI


## ITEM:
/* Increase font size in inputs and menus for better readability */


## ITEM:
.comfy-multiline-input, .litecontextmenu .litemenu-entry {


## ITEM:
font-size: 20px !important;


## ITEM:
}


## ITEM:
/* Make context menu entries larger for easier selection */


## ITEM:
• 	Oﬃcial Website: Links to the ComfyOrg oﬃcial website


## ITEM:
Since the version information here mainly corresponds to stable version information, if
you are using the nightly version, the corresponding commit hash will not be displayed
here. If you are using the nightly version, you can use the git log command in the
corresponding ComfyUI main directory to view the corresponding commit hash and
other information. Another common issue is that diﬀerent dependency packages may
fail and rollback during updates.


## ITEM:
Function: Limits the maximum size of single file uploads, in MB, default 100MB. Aﬀects
upload limits for images, models and other files


## ITEM:
CUDA


## ITEM:
CUDA device index to use


## ITEM:
Function: Specifies which NVIDIA graphics card to use. 0 represents the first graphics
card, 1 represents the second, and so on. Important for multi-GPU systems


## ITEM:
Use CUDA malloc for memory allocation


## ITEM:
Function: Controls whether to use CUDA’s memory allocator. Can improve memory
management eﬃciency in certain situations


## ITEM:
Inference


## ITEM:
Global floating point precision


## ITEM:
Function: Sets the numerical precision for model calculations. FP16 saves VRAM but
may aﬀect quality, FP32 is more precise but uses more VRAM


## ITEM:
UNET precision


## ITEM:
Options:


## ITEM:
• 	 auto: Automatically selects the most suitable precision


## ITEM:
• 	 fp64: 64-bit floating point precision, highest precision but largest VRAM
usage


## ITEM:
• 	 fp32: 32-bit floating point precision, standard precision


## ITEM:
• 	 fp16: 16-bit floating point precision, can save VRAM


## ITEM:
• 	 bf16: 16-bit brain floating point precision, between fp16 and fp32


## ITEM:
• 	 fp8_e4m3fn: 8-bit floating point precision (e4m3), minimal VRAM usage


## ITEM:
• 	 fp8_e5m2: 8-bit floating point precision (e5m2), minimal VRAM usage


## ITEM:
Function: Specifically controls the computational precision of the UNET core
component of diﬀusion models. Higher precision can provide better image generation
quality but uses more VRAM. Lower precision can significantly save VRAM but may
aﬀect the quality of generated results.


## ITEM:
VAE precision


## ITEM:
Options and Recommendations:


## ITEM:
• 	 auto: Automatically selects the most suitable precision, recommended for
users with 8-12GB VRAM


## ITEM:
• 	 fp16: 16-bit floating point precision, recommended for users with 6GB or
less VRAM, can save VRAM but may aﬀect quality


## ITEM:
• 	 fp32: 32-bit floating point precision, recommended for users with 16GB
or more VRAM who pursue the best quality


## ITEM:
• 	 bf16: 16-bit brain floating point precision, recommended for newer
graphics cards that support this format, can achieve better performance
balance


## ITEM:
Function: Controls the computational precision of the Variational Autoencoder (VAE),
aﬀecting the quality and speed of image encoding/decoding. Higher precision can
provide better image reconstruction quality but uses more VRAM. Lower precision can
save VRAM but may aﬀect image detail restoration.


## ITEM:
Run VAE on CPU


## ITEM:
Function: Forces VAE to run on CPU, can save VRAM but will reduce processing speed


## ITEM:
Text Encoder precision


## ITEM:
Options:


## ITEM:
• 	 auto: Automatically selects the most suitable precision


## ITEM:
• 	 fp8_e4m3fn: 8-bit floating point precision (e4m3), minimal VRAM usage


## ITEM:
• 	 fp8_e5m2: 8-bit floating point precision (e5m2), minimal VRAM usage


## ITEM:
• 	 fp16: 16-bit floating point precision, can save VRAM


## ITEM:
• 	 fp32: 32-bit floating point precision, standard precision


## ITEM:
Function: Controls the computational precision of the text prompt encoder, aﬀecting
the accuracy of text understanding and VRAM usage. Higher precision can provide
more accurate text understanding but uses more VRAM. Lower precision can save
VRAM but may aﬀect prompt parsing eﬀectiveness.


## ITEM:
Memory


## ITEM:
Force channels-last memory format


## ITEM:
Function: Changes the data arrangement in memory, may improve performance on
certain hardware


## ITEM:
DirectML device index


## ITEM:
Function: Specifies the device when using DirectML acceleration on Windows, mainly
for AMD graphics cards


## ITEM:
Disable IPEX optimization


## ITEM:
Function: Disables Intel CPU optimization, mainly aﬀects Intel processor performance


## ITEM:
VRAM management mode


## ITEM:
Options:


## ITEM:
• 	 auto: Automatically manages VRAM, allocating VRAM based on model
size and requirements


## ITEM:
• 	 lowvram: Low VRAM mode, uses minimal VRAM, may aﬀect generation
quality


## ITEM:
• 	 normalvram: Standard VRAM mode, balances VRAM usage and
performance


## ITEM:
• 	 highvram: High VRAM mode, uses more VRAM for better performance


## ITEM:
• 	 novram: No VRAM usage, runs entirely on system memory


## ITEM:
• 	 cpu: CPU-only mode, doesn’t use graphics card


## ITEM:
Function: Controls VRAM usage strategy, such as automatic management, low VRAM
mode, etc.


## ITEM:
Reserved VRAM (GB)


## ITEM:
Function: Amount of VRAM reserved for the operating system and other programs,
prevents system freezing


## ITEM:
Disable smart memory management


## ITEM:
Function: Disables automatic memory optimization, forces models to move to system
memory to free VRAM


## ITEM:
Preview


## ITEM:
Method used for latent previews


## ITEM:
Options:


## ITEM:
• 	 none: No preview images displayed, only shows progress bar during
generation


## ITEM:
• 	 auto: Automatically selects the most suitable preview method,
dynamically adjusts based on system performance and VRAM


## ITEM:
• 	 latent2rgb: Directly converts latent space data to RGB images for
preview, faster but average quality


## ITEM:
• 	 taesd: Uses lightweight TAESD model for preview, balances speed and
quality


## ITEM:
Function: Controls how to preview intermediate results during generation. Diﬀerent
preview methods aﬀect preview quality and performance consumption. Choosing the
right preview method can find a balance between preview eﬀects and system resource
usage.


## ITEM:
Size of preview images


## ITEM:
Function: Sets the resolution of preview images, aﬀects preview clarity and
performance. Larger sizes provide higher preview quality but also consume more
VRAM


## ITEM:
Cache


## ITEM:
Use classic cache system


## ITEM:
Function: Uses traditional caching strategy, more conservative but stable


## ITEM:
Use LRU caching with a maximum of N node results cached


## ITEM:
Function: Uses Least Recently Used (LRU) algorithm caching system, can cache a
specified number of node computation results


## ITEM:
Description:


## ITEM:
• Set a specific number to control maximum cache count, such as 10, 50, 100,
etc.


## ITEM:
• Caching can avoid repeated computation of the same node operations,
improving workflow execution speed


## ITEM:
• When cache reaches the limit, automatically clears the least recently used
results


## ITEM:
• Cached results occupy system memory (RAM/VRAM), larger values use more
memory


## ITEM:
Usage Recommendations:


## ITEM:
• Default value is null, meaning LRU caching is not enabled


## ITEM:
• Set appropriate cache count based on system memory capacity and usage
requirements


## ITEM:
• Recommended for workflows that frequently reuse the same node
configurations


## ITEM:
• If system memory is suﬃcient, larger values can be set for better performance
improvement


## ITEM:
Attention


## ITEM:
Cross attention method


## ITEM:
Options:


## ITEM:
• 	 auto: Automatically selects the most suitable attention computation
method


## ITEM:
• 	 split: Block-wise attention computation, can save VRAM but slower
speed


## ITEM:
• 	 quad: Uses quad attention algorithm, balances speed and VRAM usage


## ITEM:
• 	 pytorch: Uses PyTorch native attention computation, faster but higher
VRAM usage


## ITEM:
Function: Controls the specific algorithm used when the model computes attention.
Diﬀerent algorithms make diﬀerent trade-oﬀs between generation quality, speed, and
VRAM usage. Usually recommended to use auto for automatic selection.


## ITEM:
Force attention upcast


## ITEM:
Function: Forces high-precision attention computation, improves quality but increases
VRAM usage


## ITEM:
Prevent attention upcast


## ITEM:
Function: Disables high-precision attention computation, saves VRAM


## ITEM:
General


## ITEM:
Disable xFormers optimization


## ITEM:
Function: Disables the optimization features of the xFormers library. xFormers is a
library specifically designed to optimize the attention mechanisms of Transformer
models, typically improving computational eﬃciency, reducing memory usage, and
accelerating inference speed. Disabling this optimization will:


## ITEM:
• Fall back to standard attention computation methods


## ITEM:
• May increase memory usage and computation time


## ITEM:
• Provide a more stable runtime environment in certain situations


## ITEM:
Use Cases:


## ITEM:
• When encountering compatibility issues related to xFormers


## ITEM:
• When more precise computation results are needed (some optimizations may
aﬀect numerical precision)


## ITEM:
Function: Does not save workflow information in generated images, reducing file size,
but also means the loss of corresponding workflow information, preventing you from
using workflow output files to reproduce the corresponding generation results


## ITEM:
Function: Sets the default storage path for input files (such as images, models)


## ITEM:
Output directory


## ITEM:
Function: Sets the save path for generation results


## ITEM:
Symptoms: “Prompt execution failed” dialog with “Show report” button, workflow
stops executing


## ITEM:
Quick fixes:


## ITEM:
1. Click “Show report” - Read the detailed error message to identify the specific
issue


## ITEM:
3. Verify model files - See Models documentation for model setup


## ITEM:
4. Check VRAM usage - Close other applications using GPU memory


## ITEM:
Slow Performance


## ITEM:
Symptoms: Very slow generation times, system freezing, out of memory errors


## ITEM:
Quick fixes:


## ITEM:
1. Lower resolution/batch size - Reduce image size or number of images


## ITEM:
2. Use memory optimization flags - See performance optimization section below


## ITEM:
3. Close unnecessary applications - Free up RAM and VRAM


## ITEM:
4. Check CPU/GPU usage - Use Task Manager to identify bottlenecks


## ITEM:
Performance Optimization Commands:


## ITEM:
For low VRAM systems:


## ITEM:
Copy


## ITEM:
Ask AI


## ITEM:
```bash
# Low VRAM mode (uses cpu for text encoder)
```


## ITEM:
```bash
python main.py --lowvram
```


## ITEM:
```bash
# CPU mode (very slow but works with any hardware, only use as absolute last resort)
```


## ITEM:
```bash
python main.py --cpu
```


## ITEM:
For better performance:


## ITEM:
Copy


## ITEM:
Ask AI


## ITEM:
```bash
# Disable previews (saves VRAM and processing)
```


## ITEM:
```bash
python main.py --preview-method none
```


## ITEM:
```bash
# Use optimized attention mechanisms
```


## ITEM:
```bash
python main.py --use-pytorch-cross-attention
```


## ITEM:
```bash
python main.py --use-flash-attention
```


## ITEM:
```bash
# Async weight oﬄoading
```


## ITEM:
```bash
python main.py --async-oﬄoad
```


## ITEM:
For memory management:


## ITEM:
Copy


## ITEM:
Ask AI


## ITEM:
```bash
# Reserve specific VRAM amount for OS (in GB)
```


## ITEM:
```bash
python main.py --reserve-vram 2
```


## ITEM:
```bash
# Disable smart memory management
```


## ITEM:
```bash
python main.py --disable-smart-memory
```


## ITEM:
```bash
# Use diﬀerent caching strategies
```


## ITEM:
```bash
python main.py --cache-none      # Less RAM usage, but slower
```


## ITEM:
```bash
python main.py --cache-lru 10    # Cache 10 results, faster
```


## ITEM:
```bash
python main.py --cache-classic   # Use the old style (aggressive) caching.
```


## ITEM:
• 	Missing models: Models are not copied during migration, only linked. Verify
model paths


## ITEM:
```bash
# Install dependencies
```


## ITEM:
```bash
pip install -r requirements.txt
```


## ITEM:
```bash
# For NVIDIA GPUs (CUDA 12.8)
```


## ITEM:
```bash
pip install torch torchvision torchaudio --extra-index-url https://download.pytorch.org/
whl/cu128
```


## ITEM:
```bash
# For AMD GPUs (Linux only - ROCm 6.3)
```


## ITEM:
```bash
pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/
rocm6.3
```


## ITEM:
Linux-Specific Issues


## ITEM:
LD_LIBRARY_PATH errors:


## ITEM:
Common symptoms:


## ITEM:
• “libcuda.so.1: cannot open shared object file”


## ITEM:
• “libnccl.so: cannot open shared object file”


## ITEM:
• “ImportError: libnvinfer.so.X: cannot open shared object file”


## ITEM:
Solutions:


## ITEM:
API Nodes Not Working


## ITEM:
Symptoms: API calls fail, timeout errors, quota exceeded


## ITEM:
Solutions:


## ITEM:
1. Check API key validity - Verify keys in user settings


## ITEM:
2. Check account credits - Ensure suﬃcient API credits


## ITEM:
3. Verify internet connection - Test with other online services


## ITEM:
4. Check service status - Provider may be experiencing downtime


## ITEM:
Connection Issues


## ITEM:
Symptoms: “Failed to connect to server”, timeout errors


## ITEM:
Solutions:


## ITEM:
1. Check firewall settings - Allow ComfyUI through firewall


## ITEM:
2. Try diﬀerent port - Default is 8188, try 8189 or 8190


## ITEM:
3. Disable VPN temporarily - VPN may be blocking connections


## ITEM:
4. Check proxy settings - Disable proxy if not required


## ITEM:
Frontend Issues


## ITEM:
“Frontend or Templates Package Not Updated”:


## ITEM:
Copy


## ITEM:
Ask AI


## ITEM:
```bash
# After updating ComfyUI via Git, update frontend dependencies
```


## ITEM:
```bash
pip install -r requirements.txt
```


## ITEM:
“Error Toast About Workflow Failing Validation”:


## ITEM:
• Disable workflow validation in settings temporarily


## ITEM:
• Report the issue to the ComfyUI team


## ITEM:
Login Issues When Not on Localhost:


## ITEM:
• 	Normal login only works when accessing from localhost


## ITEM:
• 	For LAN/remote access: Generate API key at platform.comfy.org/login


## ITEM:
• 	Use API key in login dialog or with --api-key command line argument


## ITEM:
Hardware-Specific Issues


## ITEM:
NVIDIA GPU Issues


## ITEM:
“Torch not compiled with CUDA enabled” error:


## ITEM:
Copy


## ITEM:
Ask AI


## ITEM:
```bash
# First uninstall torch
```


## ITEM:
```bash
pip uninstall torch
```


## ITEM:
```bash
# Install stable PyTorch with CUDA 12.8
```


## ITEM:
```bash
pip install torch torchvision torchaudio --extra-index-url https://download.pytorch.org/
whl/cu128
```


## ITEM:
```bash
# For nightly builds (might have performance improvements)
```


## ITEM:
```bash
pip install --pre torch torchvision torchaudio --index-url https://download.pytorch.org/
whl/nightly/cu128
```


## ITEM:
```bash
# Verify CUDA support
```


## ITEM:
```bash
python -c "import torch; print(torch.cuda.is_available())"
```


## ITEM:
GPU not detected:


## ITEM:
Copy


## ITEM:
Ask AI


## ITEM:
```bash
# Check if GPU is visible
```


## ITEM:
```bash
nvidia-smi
```


## ITEM:
```bash
# Check driver version and CUDA compatibility
```


## ITEM:
```bash
nvidia-smi --query-gpu=driver_version --format=csv
```


## ITEM:
AMD GPU Issues


## ITEM:
ROCm support (Linux only):


## ITEM:
Copy


## ITEM:
Ask AI


## ITEM:
```bash
# Install stable ROCm PyTorch (6.3.1 at the time of writing)
```


## ITEM:
```bash
pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/
rocm6.3
```


## ITEM:
```bash
# For nightly builds (ROCm 6.4 at the time of writing), which might have performance
improvements)
```


## ITEM:
```bash
pip install --pre torch torchvision torchaudio --index-url https://download.pytorch.org/
whl/nightly/rocm6.4
```


## ITEM:
Unsupported AMD GPUs:


## ITEM:
Copy


## ITEM:
Ask AI


## ITEM:
```bash
# For RDNA2 or older (6700, 6600)
```


## ITEM:
```bash
HSA_OVERRIDE_GFX_VERSION=10.3.0 python main.py
```


## ITEM:
```bash
# For RDNA3 cards (7600)
```


## ITEM:
```bash
HSA_OVERRIDE_GFX_VERSION=11.0.0 python main.py
```


## ITEM:
Performance optimization:


## ITEM:
Copy


## ITEM:
Ask AI


## ITEM:
```bash
# Enable experimental memory eﬃcient attention (no longer necessary with PyTorch
2.4)
```


## ITEM:
```bash
TORCH_ROCM_AOTRITON_ENABLE_EXPERIMENTAL=1 python main.py --use-
pytorch-cross-attention
```


## ITEM:
```bash
# Enable tunable operations (slow first run, but faster subsequent runs)
```


## ITEM:
```bash
PYTORCH_TUNABLEOP_ENABLED=1 python main.py
```


## ITEM:
Apple Silicon (M1/M2/M3) Issues


## ITEM:
MPS backend setup:


## ITEM:
Copy


## ITEM:
Ask AI


## ITEM:
```bash
# Install PyTorch nightly for Apple Silicon
```


## ITEM:
```bash
# Follow Apple's guide: https://developer.apple.com/metal/pytorch/
```


## ITEM:
```bash
# Check MPS availability
```


## ITEM:
```bash
python -c "import torch; print(torch.backends.mps.is_available())"
```


## ITEM:
• 	Test with default workflow


## ITEM:
• Workflow file (.json) that reproduces the issue


## ITEM:
Root cause: Using models from diﬀerent architecture families together


## ITEM:
Solutions


## ITEM:
1. 	Verify model family compatibility:


## ITEM:
• 	Flux models use 16-channel latent space with dual text encoder
conditioning (CLIP-L + T5-XXL)


## ITEM:
• 	SD1.5 models use 4-channel latent space with single CLIP ViT-L/14 text
encoder


## ITEM:
• 	SDXL models use 4-channel latent space with dual text encoders (CLIP
ViT-L/14 + OpenCLIP ViT-bigG/14)


## ITEM:
• 	SD3 models use 16-channel latent space with triple text encoder
conditioning (CLIP-L + OpenCLIP bigG + T5-XXL)


## ITEM:
• 	ControlNet models must match the architecture of the base checkpoint
(SD1.5 ControlNets only work with SD1.5 checkpoints, SDXL ControlNets
only work with SDXL checkpoints, etc.)


## ITEM:
2. 	Common mismatch scenarios and fixes: Flux + wrong VAE:


## ITEM:
Copy


## ITEM:
Ask AI


## ITEM:
Problem: Using taesd or sdxl_vae.safetensors with Flux checkpoint


## ITEM:
3. 	Fix: Use ae.safetensors (Flux VAE) from Hugging Face Flux releases


## ITEM:
4.


## ITEM:
Flux + incorrect CLIP configuration:


## ITEM:
Copy


## ITEM:
Ask AI


## ITEM:
Problem: Using t5xxl_fp8_e4m3fn.safetensors in both CLIP slots of
DualClipLoader


## ITEM:
5. 	Fix: Use t5xxl_fp8_e4m3fn.safetensors in one slot and clip_l.safetensors in the
other


## ITEM:
6.


## ITEM:
ControlNet architecture mismatch:


## ITEM:
Copy


## ITEM:
Ask AI


## ITEM:
Problem: SD1.5 ControlNet with SDXL checkpoint (or vice versa)


## ITEM:
7. 	Error: "mat1 and mat2 shapes cannot be multiplied (154x2048 and 768x320)"


## ITEM:
8. 	Fix: Use ControlNet models designed for your checkpoint architecture


## ITEM:
9. 	     - SD1.5 checkpoints require SD1.5 ControlNets


## ITEM:
10. 	     - SDXL checkpoints require SDXL ControlNets


## ITEM:
11.


## ITEM:
12. 	Quick diagnostics:


## ITEM:
Copy


## ITEM:
Ask AI


## ITEM:
```bash
# Check if error occurs at VAE decode stage
```


## ITEM:
13. 	# Look for "expected input[X, Y, Z] to have N channels, but got M channels"


## ITEM:
14. 	# Y value indicates channel count: 4 = SD models, 16 = Flux models


## ITEM:
15.


## ITEM:
16. 	Prevention strategies:


## ITEM:
• 	Keep all workflow models within the same architecture family


## ITEM:
• 	Download complete model packages from same source/release (often all
in a Hugging Face repo)


## ITEM:
• 	When trying new models, start with the template workflows or oﬃcial
ComfyUI workflow examples before customizing


## ITEM:
Missing Models Error


## ITEM:
Example error message:


## ITEM:
Copy


## ITEM:
Ask AI


## ITEM:
Prompt execution failed


## ITEM:
Prompt outputs failed validation:


## ITEM:
CheckpointLoaderSimple:


## ITEM:
- Value not in list: ckpt_name: 'model-name.safetensors' not in []


## ITEM:
Solutions


## ITEM:
1. 	Download required models:


## ITEM:
• 	Verify models are in correct subfolders


## ITEM:
2. 	Check model paths:


## ITEM:
• 	Checkpoints: models/checkpoints/


## ITEM:
• 	VAE: models/vae/


## ITEM:
• 	LoRA: models/loras/


## ITEM:
• 	ControlNet: models/controlnet/


## ITEM:
• 	Embeddings: models/embeddings/


## ITEM:
3. 	Share models between UIs or use custom paths:


## ITEM:
• 	See ComfyUI Model Sharing and Custom Model Directory Configuration
for detailed instructions


## ITEM:
• 	Edit extra_model_paths.yaml file to add custom model directories


## ITEM:
Model Search Path Configuration


## ITEM:
If you have models in custom locations, see the detailed guide for ComfyUI Model
Sharing and Custom Model Directory Configuration to configure ComfyUI to find them.


## ITEM:
Model Loading Errors


## ITEM:
Error message: “Error while deserializing header”


## ITEM:
Solutions


## ITEM:
1. Re-download the model - File may be corrupted during download


## ITEM:
2. Check available disk space - Ensure enough space for model loading (models
can be 2-15GB+)


## ITEM:
3. Check file permissions - Ensure ComfyUI can read the model files


## ITEM:
4. Test with diﬀerent model - Verify if issue is model-specific or system-wide


## ITEM:
Model Performance Issues


## ITEM:
Slow Model Loading


## ITEM:
Symptoms: Long delays when switching models or starting generation


## ITEM:
Solutions:


## ITEM:
1. 	Use faster storage:


## ITEM:
• 	Move models to SSD if using HDD


## ITEM:
• 	Use NVMe SSD for best performance


## ITEM:
2. 	Adjust caching settings:


## ITEM:
Copy


## ITEM:
Ask AI


## ITEM:
```bash
python main.py --cache-classic       # Use the old style (aggressive) caching.
```


## ITEM:
3. 	python main.py --cache-lru 10         # Increase size of LRU cache


## ITEM:
4.


## ITEM:
Memory Issues with Large Models


## ITEM:
“RuntimeError: CUDA out of memory”:


## ITEM:
Copy


## ITEM:
Ask AI


## ITEM:
```bash
# Progressive memory reduction
```


## ITEM:
```bash
python main.py --lowvram          # First try
```


## ITEM:
```bash
python main.py --novram           # If lowvram insuﬃcient
```


## ITEM:
```bash
python main.py --cpu              # Last resort
```


## ITEM:
Model-specific memory optimization:


## ITEM:
Copy


## ITEM:
Ask AI


## ITEM:
```bash
# Force lower precision
```


## ITEM:
```bash
python main.py --force-fp16
```


## ITEM:
```bash
# Reduce attention memory usage
```


## ITEM:
```bash
python main.py --use-pytorch-cross-attention
```


## ITEM:
For additional model configuration and setup information, see the Models
documentation.


## ITEM:
Enabled custom
nodes > 1?


## ITEM:
Disabled custom
nodes > 1?


## ITEM:
Continue binary
search on enabled
nodes


## ITEM:
Continue binary
search on disabled
nodes


## ITEM:
• A: Custom
nodes with


## ITEM:
En
d
.
