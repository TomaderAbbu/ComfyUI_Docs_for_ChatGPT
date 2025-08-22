# SECTION: ADVANCED_USAGE


## ITEM:
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


## ITEM:
• 	API Reliability: Core API enhancements provide more stable foundation for
custom node development


## ITEM:
• 	Execution Flexibility: New partial execution capabilities allow for more eﬃcient
debugging and development


## ITEM:
• 	Template Updates: Multiple template version updates (0.1.36, 0.1.37, 0.1.39) for
improved custom node development


## ITEM:
• 	Documentation: Enhanced fast_fp16_accumulation documentation


## ITEM:
• 	Custom Node Management: New --whitelist-custom-nodes argument pairs with
--disable-all-custom-nodes


## ITEM:
• 	Performance Optimizations: Dual CFG node now optimizes automatically when
CFG is 1.0


## ITEM:
• 	GitHub Actions Integration: Automated release webhook notifications


## ITEM:
Image Processing Improvements


## ITEM:
• 	Custom Node Support: Added pyproject.toml support for better dependency
management


## ITEM:
• 	Help Menu Integration: New help system in the Node Library sidebar


## ITEM:
• 	Template Updates: Enhanced project templates for custom node development


## ITEM:
To get started, try out some of the oﬃcial workflows. These use only the Core nodes
included in the ComfyUI installation. A thriving community of developers has created a
rich ecosystem of custom nodes to extend the functionality of ComfyUI.


## ITEM:
Simple Example


## ITEM:
Visual programming


## ITEM:
A node-based computer program like ComfyUI provides a level of power and flexibility
that can’t be achieved with traditional menu- and button-driven applications. The
ComfyUI node graph is not limited by the tools provided in a traditional computer
application. It’s a high-level visual programming environment allowing users to design
complex systems without needing to write program code or understand advanced
mathematics.


## ITEM:
Many other computer applications use this same node graph paradigm. Examples
include the compositing application called Nuke, the 3D programs Maya and Blender,
the Unreal real-time graphics engine, and the interactive media authoring program
called Max.


## ITEM:
More Complex Example


## ITEM:
Procedural framework


## ITEM:
Another term used to describe a node-based application is procedural framework.
Procedural means generative: some procedure or algorithm is employed to generate
content such as a 3D model or a musical composition.


## ITEM:
ComfyUI is all of these things: a node graph, a visual programming environment, and a
procedural framework. What makes ComfyUI diﬀerent (and amazing!) is that its
radically open structure allows us to generate any type of media asset such as picture,
movie, sound, 3D model, AI model, etc.


## ITEM:
In ComfyUI, nodes are the fundamental building blocks for executing tasks. Each node
is an independently built module, whether it’s a Comfy Core node or a Custom Node,
with its own unique functionality. Nodes connect to each other through links, allowing
us to build complex functionality like assembling LEGO blocks. The combinations of
diﬀerent nodes create the unlimited possibilities of ComfyUI.


## ITEM:
For example, in the K-Sampler node, you can see it has multiple inputs and outputs,
and also includes multiple parameter settings. These parameters determine the logic of
node execution. Behind each node is well-written Python logic, allowing you to achieve
corresponding functionality without having to write code yourself.


## ITEM:
As ComfyUI is still in rapid iteration and development, we are continuously improving it
every day. Therefore, some operations mentioned in this article may change or be
omitted. Please refer to the actual interface. If you find changes in actual operations, it
may be due to our iterative updates. You can also fork this repo and help us improve
this documentation.


## ITEM:
• 	Custom node missing: The workflow uses custom nodes developed by
third-party authors, but your local ComfyUI version doesn’t have these
custom nodes installed. You can use ComfyUI-Manager to find and install
the missing custom nodes


## ITEM:
Currently, Comfy Core nodes use a fox icon for display, while custom nodes use their
names. This way you can quickly understand which node package a node comes from.


## ITEM:
You can set the corresponding display in the menu:


## ITEM:
Node Context Menus


## ITEM:
Node context menus are mainly divided into two types:


## ITEM:
• Context menu for the node itself


## ITEM:
• Context menu for inputs/outputs


## ITEM:
Node Context Menu


## ITEM:
By right-clicking on a node, you can expand the corresponding node context menu:


## ITEM:
In the node’s right-click context menu, you can:


## ITEM:
• Adjust the node’s color style


## ITEM:
• Modify the title


## ITEM:
• Clone, copy, or delete the node


## ITEM:
• Set the node’s mode


## ITEM:
In this menu, besides appearance-related settings, the following menu operations are
important:


## ITEM:
• 	Mode: Set the node’s mode: Always, Never, Bypass


## ITEM:
• 	Toggle between Widget and Input mode for node inputs: Switch between widget
and input mode for node inputs


## ITEM:
Mode


## ITEM:
For modes, you may notice that we currently provide: Always, Never, On Event, On
Trigger - four modes, but actually only Always and Never are eﬀective. On Event and
On Trigger are currently ineﬀective as we haven’t fully implemented this feature.
Additionally, you can understand Bypass as a mode. Below is an explanation of the
available modes:


## ITEM:
• 	Always: The default node mode. The node will execute whenever it runs for the
first time or when any of its inputs change since the last execution


## ITEM:
Custom Nodes


## ITEM:
ComfyUI includes many powerful nodes in the base installation package. These are
known as Comfy Core nodes. Additionally, the ComfyUI community has created an
amazing array of custom nodes to perform a wide variety of functions.


## ITEM:
ComfyUI Manager


## ITEM:
The ComfyUI Manager window makes it easy to perform custom node management
tasks such as search, install, update, disable, and uninstall. The Manager is included in
the ComfyUI desktop application, but not in the ComfyUI server application.


## ITEM:
Installing the ComfyUI Manager


## ITEM:
If you’re running the ComfyUI server application, you need to install the Manager. If
ComfyUI is running, shut it down before proceeding.


## ITEM:
The first step is to install Git, a command-line application for software version control.
Git will download the ComfyUI Manager from github.com. Download Git from git-
scm.com and install it.


## ITEM:
For details or special cases, see ComfyUI Manager Install.


## ITEM:
Custom Nodes


## ITEM:
Learn about installing, enabling dependencies, updating, disabling, and uninstalling
custom nodes in ComfyUI


## ITEM:
About Custom Nodes


## ITEM:
Additionally, there are numerous custom nodes created by various authors from the
ComfyUI community. These custom nodes bring extensive functionality to ComfyUI,
greatly expanding its capabilities and feature boundaries.


## ITEM:
In this guide, we’ll cover various operations related to custom nodes, including
installation, updates, disabling, uninstalling, and dependency installation.


## ITEM:
Anyone can develop their own custom extensions for ComfyUI and share them with
others. You can find many community custom nodes here. If you want to develop your
own custom nodes, visit the section below to get started:


## ITEM:
Start Developing Custom Nodes


## ITEM:
Learn how to start developing a custom node


## ITEM:
Custom Node Management


## ITEM:
In this section we will cover:


## ITEM:
• Installing custom nodes


## ITEM:
• Custom node version control


## ITEM:
• Uninstalling custom nodes


## ITEM:
• Temporarily disabling custom nodes


## ITEM:
• Handling custom node dependency conflicts


## ITEM:
1. Installing Custom Nodes


## ITEM:
Currently, ComfyUI supports installing custom nodes through multiple methods,
including:


## ITEM:
• 	Install via ComfyUI Manager (Recommended)


## ITEM:
• 	Install via Git


## ITEM:
We recommend installing custom nodes through ComfyUI Manager, which is a highly
significant tool in the ComfyUI custom node ecosystem. It makes custom node
management (such as searching, installing, updating, disabling, and uninstalling)
simple - you just need to search for the node you want to install in ComfyUI Manager
and click install.


## ITEM:
However, since all custom nodes are currently stored on GitHub, for regions that
cannot access GitHub normally, we have written detailed instructions for diﬀerent
custom node installation methods in this guide.


## ITEM:
Additionally, since we recommend using ComfyUI Manager for plugin management, we
recommend using this tool for plugin management. You can find its source code here.
Therefore, in this documentation, we will use installing ComfyUI Manager as a custom
node installation example, and supplement how to use it for node management in the
relevant introduction sections.


## ITEM:
• 	Install via ComfyUI Manager


## ITEM:
• 	Install via Git


## ITEM:
Since ComfyUI Manager has very rich functionality, we will use a separate document to
introduce the ComfyUI Manager installation chapter. Please visit the link below to learn
how to use ComfyUI Manager to install custom nodes.


## ITEM:
Install Custom Nodes with ComfyUI Manager


## ITEM:
Learn how to use ComfyUI Manager to install custom nodes


## ITEM:
Custom nodes all require the installation of related dependencies. For example, for
ComfyUI-Manager, you can visit the requirements.txt file to view the dependency
package requirements.


## ITEM:
In the previous steps, we only cloned the custom node code locally and did not install
the corresponding dependencies, so next we need to install the corresponding
dependencies.


## ITEM:
Actually, if you use ComfyUI-Manager to install plugins, ComfyUI Manager will
automatically help you complete the dependency installation. You just need to restart
ComfyUI after installing the plugin. This is why we strongly recommend using ComfyUI
Manager to install custom nodes.


## ITEM:
But perhaps you may not be able to use ComfyUI Manager to install custom nodes
smoothly in some situations, so we provide this more detailed dependency installation
guide.


## ITEM:
If you run pip install -r requirements.txt directly in the system-level terminal, the
corresponding dependencies may be installed in the system-level Python environment,
which will cause the dependencies to still be missing in ComfyUI’s environment,
preventing the corresponding custom nodes from running normally.


## ITEM:
Of course, you can replace ComfyUI-Manager with the name of the custom node you
actually installed, but make sure that a requirements.txt file exists in the corresponding
node directory.


## ITEM:
Custom Node Version Control


## ITEM:
Custom node version control is actually based on Git version control. You can manage
node versions through Git, but ComfyUI Manager has already integrated this version
management functionality very well. Many thanks to @Dr.Lt.Data for bringing us such a
convenient tool.


## ITEM:
• 	Version Management with ComfyUI Manager


## ITEM:
• 	Version Management with Git


## ITEM:
Since we are iterating on ComfyUI Manager, the actual latest interface and steps may
change significantly


## ITEM:
1


## ITEM:
Enter Node Management Interface


## ITEM:
Perform the corresponding operations as shown to enter the ComfyUI Manager
interface


## ITEM:
2


## ITEM:
Find the Corresponding Custom Node Package


## ITEM:
You can use the corresponding filters to filter out installed node packages and then
perform the corresponding node management


## ITEM:
3


## ITEM:
Perform Version Switching


## ITEM:
Uninstalling Custom Nodes


## ITEM:
To be updated


## ITEM:
Temporarily Disabling Custom Nodes


## ITEM:
To be updated


## ITEM:
Custom Node Dependency Conflicts


## ITEM:
To be updated


## ITEM:
ComfyUI Manager


## ITEM:
As ComfyUI continues to develop, ComfyUI Manager plays an increasingly important
role in ComfyUI. Currently, ComfyUI-Manager has oﬃcially joined the Comfy Org
organization, oﬃcially becoming part of ComfyUI’s core dependencies, and continues
to be maintained by the original author Dr.Lt.Data. You can read this blog post for more
information. In future iterations, we will greatly optimize the use of ComfyUI Manager,
so the interface shown in this documentation may diﬀer from the latest version of
ComfyUI Manager.


## ITEM:
Installing the Manager


## ITEM:
If you are running the ComfyUI server application, you need to install the manager. If
ComfyUI is running, please close it before continuing.


## ITEM:
The first step is to install Git, which is a command-line application for software version
control. Git will download the ComfyUI manager from github.com. Download and install
Git from git-scm.com.


## ITEM:
Developing a Custom Node


## ITEM:
If you have some development capabilities, please start with the documentation below
to learn how to begin developing a custom node.


## ITEM:
Start Developing Custom Nodes


## ITEM:
Learn how to start developing a custom node


## ITEM:
2. The ComfyUI Manager helps to automate the process
of searching, downloading, and installing


## ITEM:
3. Restart ComfyUI if it’s running


## ITEM:
Add Extra Custom Nodes Path


## ITEM:
Besides adding external models, you can also add custom nodes
paths that are not in the default path of ComfyUI


## ITEM:
Please note that this will not change the default installation path of custom
nodes, but will add an extra path search when starting ComfyUI. You still
need to complete the installation of custom node dependencies in the
corresponding environment to ensure the integrity of the running
environment.


## ITEM:
Below is a simple configuration example (MacOS), please modify
it according to your actual situation and add it to the
corresponding configuration file, save it and restart ComfyUI for
the changes to take eﬀect:


## ITEM:
Copy


## ITEM:
Ask AI


## ITEM:
• Custom nodes


## ITEM:
Custom Nodes


## ITEM:
Custom nodes are an important component of ComfyUI that extend its functionality.
They are created by the community and can be installed to add new capabilities to
your workflows.


## ITEM:
Custom Node Dependencies


## ITEM:
Thanks to the eﬀorts of many authors in the ComfyUI community, we can extend
ComfyUI’s functionality by using diﬀerent custom nodes, enabling impressive creativity.


## ITEM:
Typically, each custom node has its own dependencies and a separate
requirements.txt file. If you use ComfyUI Manager to install custom nodes, ComfyUI
Manager will usually automatically install the corresponding dependencies.


## ITEM:
There are also cases where you need to install dependencies manually. Currently, all
custom nodes are installed in the ComfyUI/custom_nodes directory.


## ITEM:
Dependency conflicts are a common issue when using ComfyUI. You might find that
after installing or updating a custom node, previously installed custom nodes can no
longer be found in ComfyUI’s node library, or error pop-ups appear. One possible
reason is dependency conflicts.


## ITEM:
There can be many reasons for dependency conflicts, such as:


## ITEM:
1. Custom node version locking


## ITEM:
Some plugins may fix the exact version of a dependency library (e.g.,
open_clip_torch==2.26.1), while other plugins may require a higher version (e.g.,
open_clip_torch>=2.29.0), making it impossible to satisfy both version requirements
simultaneously.


## ITEM:
During the installation of custom node dependencies, it may overwrite versions of
libraries already installed by other plugins. For example, multiple plugins may depend
on PyTorch but require diﬀerent CUDA versions, and the later installed plugin will break
the existing environment.


## ITEM:
Solutions:


## ITEM:
3. Custom node dependency versions incompatible with ComfyUI dependency
versions


## ITEM:
Models are a significant asset dependency for ComfyUI. Various custom nodes and
workflows are built around specific models, such as the Stable Diﬀusion series, Flux
series, Ltxv, and others. These models are an essential foundation for creation with
ComfyUI, so we need to ensure that the models we use are properly available.
Typically, our models are saved in the corresponding directory under ComfyUI/models/.
Of course, you can also create an extra_model_paths.yaml by modifying the template
to make additional model paths recognized by ComfyUI. This allows multiple ComfyUI
instances to share the same model library, reducing disk usage.


## ITEM:
Software


## ITEM:
An advanced application like ComfyUI also has software dependencies. These are
libraries of programming code and data that are required for the application to run.
Custom nodes are examples of software dependencies. On an even more fundamental
level, the Python programming environment is the ultimate dependency for ComfyUI.
The correct version of Python is required to run a particular version of ComfyUI.
Updates to Python, ComfyUI, and custom nodes can all be handled from the ComfyUI
Manager window.


## ITEM:
• Example workflows from custom nodes


## ITEM:
How to open Templates in ComfyUI


## ITEM:
Custom node templates


## ITEM:
If you are a custom node author, note that we currently only support a single directory
level under the templates folder (no nested subdirectories), and only JSON-format
templates are supported.


## ITEM:
How to add templates for custom nodes?


## ITEM:
Since custom nodes can also register corresponding setting
categories in the menu, our oﬃcial documentation currently only
includes native setting content. Additionally, some setting options
are only eﬀective for ComfyUI Desktop, which we have noted on
the corresponding pages.


## ITEM:
• 	Function: Controls the display mode of node source markers, showing node
source information. The corresponding display eﬀect is shown in the image
below. If show all is selected, it will display labels for both custom nodes and
built-in nodes, making it convenient for you to determine the corresponding
node source. The corresponding fox logo represents ComfyUI built-in nodes


## ITEM:
Double click node title to edit


## ITEM:
• 	Default Value: Enabled


## ITEM:
The Extension settings panel is a special management panel in the ComfyUI frontend
settings system, specifically used to manage the enable/disable status of frontend
extension plugins. Unlike Custom Nodes, this panel is only used to manage frontend
extensions registered by custom nodes, not to disable custom nodes themselves.


## ITEM:
These frontend extension plugins are used to enhance the ComfyUI experience, such
as providing shortcuts, settings, UI components, menu items, and other features.


## ITEM:
Extension status changes require a page reload to take eﬀect:


## ITEM:
Extension Settings Panel Features


## ITEM:
1. Extension List Management


## ITEM:
Displays all registered extensions, including:


## ITEM:
• Extension Name


## ITEM:
• Core extension identification (displays “Core” label)


## ITEM:
• Enable/disable status


## ITEM:
2. Search Functionality


## ITEM:
Provides a search box to quickly find specific extensions:


## ITEM:
3. Enable/Disable Control


## ITEM:
Each extension has an independent toggle switch:


## ITEM:
4. Batch Operations


## ITEM:
Provides right-click menu for batch operations:


## ITEM:
• Enable All extensions


## ITEM:
• Disable All extensions


## ITEM:
• Disable 3rd Party extensions (keep core extensions)


## ITEM:
Notes


## ITEM:
• Extension status changes require a page reload to take eﬀect


## ITEM:
• Some core extensions cannot be disabled


## ITEM:
• The system will automatically disable known problematic extensions


## ITEM:
• Extension settings are automatically saved to the user configuration file


## ITEM:
This Extension settings panel is essentially a “frontend plugin manager” that allows
users to flexibly control ComfyUI’s functional modules.


## ITEM:
```bash
# Section: About
```


## ITEM:
Custom Node Badges


## ITEM:
If custom nodes are installed, the About page will also display additional badge
information provided by custom nodes. These badges are registered by each custom
node through the aboutPageBadges property.


## ITEM:
System Info


## ITEM:
The bottom of the page displays detailed system statistics, including:


## ITEM:
• Hardware configuration information


## ITEM:
• Software environment information


## ITEM:
• System performance data


## ITEM:
Extension Developer Guide


## ITEM:
Extension developers can add custom badges to the About page by adding the
aboutPageBadges property to their extension configuration:


## ITEM:
Copy


## ITEM:
Ask AI


## ITEM:
app.registerExtension({


## ITEM:
name: 'MyExtension',


## ITEM:
aboutPageBadges: [


## ITEM:
{


## ITEM:
Disable loading all custom nodes


## ITEM:
3. Custom Node Issues


## ITEM:
```bash
# Section: Overview
```


## ITEM:
Check how to troubleshoot issues caused by custom nodes.


## ITEM:
“Can’t Find Custom Node”:


## ITEM:
For Custom Node Issues


## ITEM:
Where to report: Contact the specific custom node developer


## ITEM:
Required Information


## ITEM:
When reporting any issue, include:


## ITEM:
1


## ITEM:
System Information


## ITEM:
• 	From ComfyUI Interface


## ITEM:
• 	From Command Line


## ITEM:
System Information (can be found in the About page in settings):


## ITEM:
• 	Operating System (Windows 11, macOS 14.1, Ubuntu 22.04, etc.)


## ITEM:
• 	ComfyUI version (check About page in settings)


## ITEM:
• 	Python version: python --version


## ITEM:
• 	PyTorch version: python -c "import torch; print(torch.__version__)"


## ITEM:
• 	GPU model and driver version


## ITEM:
• List of installed custom nodes


## ITEM:
• 	Use ComfyUI Manager to auto-download models


## ITEM:
```bash
# Section: Custom Node Issues
```


## ITEM:
Troubleshoot and fix problems caused by custom nodes and extensions


## ITEM:
Restart ComfyUI and  Issue is in enabled
test custom nodes


## ITEM:
Issue is in disabled
custom nodes


## ITEM:
Found problematic
custom node


## ITEM:
End


## ITEM:
Two
Troubleshoo
ting
Methods
