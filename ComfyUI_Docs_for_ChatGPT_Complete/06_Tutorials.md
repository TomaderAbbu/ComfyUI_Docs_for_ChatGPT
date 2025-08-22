# SECTION: TUTORIALS


## ITEM:
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


## ITEM:
About Text-to-Image
Text-to-Image is a fundamental AI drawing feature that generates images from text
descriptions. It’s one of the most commonly used functions in AI art generation. You
can think of the process as telling your requirements (positive and negative prompts)
to an artist (the drawing model), who will then create what you want. Detailed
explanations about text-to-image will be covered in the Text to Image chapter.


## ITEM:
ComfyUI Text-to-Image Workflow Tutorial


## ITEM:
2. Load Default Text-to-Image Workflow
ComfyUI usually loads the default text-to-image workflow automatically when
launched. However, you can try different methods to load workflows to familiarize
yourself with ComfyUI’s basic operations:
•   Load from Workflow Template
•   Load from Images with Metadata
•   Load from workflow.json


## ITEM:
4. Select the first default workflow Image Generation to load it
Alternatively, you can select Browse workflow templates from the workflow menu


## ITEM:
For detailed text-to-image instructions, see our comprehensive guide:
ComfyUI Text-to-Image Workflow Guide


## ITEM:
Click here for detailed text-to-image workflow instructions


## ITEM:
• 	Cosmos Predict2 Support: Implementation for text-to-image (2B and 14B
models) and image-to-video generation workflows


## ITEM:
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


## ITEM:
Video Tutorial


## ITEM:
Your browser does not support the video tag.


## ITEM:
_____________________________________
_____________________________________
_____________________________________


## ITEM:
Templates - ComfyUI Built-in Workflow Templates


## ITEM:
Templates provide model workflows natively supported by ComfyUI and example
workflows from custom nodes. You can find and use workflows for currently supported
models here.


## ITEM:
Workflow Templates is the browser for ComfyUI’s natively supported model workflows
and also some example workflows from custom nodes.


## ITEM:
In ComfyUI’s Workflow Templates, you can find:


## ITEM:
Open via the menu Workflow —> Browse Workflow Templates.


## ITEM:
How to use templates


## ITEM:
You can use this tool to edit the model information in workflow templates. At the
moment, @ComfyUI-Wiki only adds support for native nodes.


## ITEM:
How to update templates?


## ITEM:
Templates are managed and updated as a separate dependency: comfyui-workflow-
templates.


## ITEM:
If, after updating ComfyUI, you don’t see the documentation or newly announced
templates, you may need to update the corresponding dependency. You can check
versions in ComfyUI/requirements.txt.


## ITEM:
comfyui-workflow-templates==0.1.52


## ITEM:
comfyui-embedded-docs==0.2.4


## ITEM:
All templates are hosted in the workflow_templates repository. You can contribute
templates by submitting a PR. For oﬃcial templates, we require the following:


## ITEM:
If a custom node author provides templates and example workflows, you can also find
them in the Templates browser. Usually, you can locate all templates by finding the
category named after the node.


## ITEM:
See Custom Node Templates for how to add workflow templates for your custom
nodes.


## ITEM:
Although we provide LAN listening settings for the Desktop version, as a desktop
application, it is not suitable for use as a server. We recommend that if you need to use
ComfyUI as a public service within the LAN, please refer to the manual deployment
tutorial to deploy the corresponding ComfyUI service.


## ITEM:
Port: The port to listen on


## ITEM:
Function: The port number the server listens on. Desktop version defaults to port 8000,
Web version typically uses port 8188


## ITEM:
TLS Key File: Path to TLS key file for HTTPS


## ITEM:
Function: The private key file path required for HTTPS encryption, used to establish
secure connections


## ITEM:
TLS Certificate File: Path to TLS certificate file for HTTPS


## ITEM:
Function: The certificate file path required for HTTPS encryption, used in conjunction
with the private key


## ITEM:
Enable CORS header: Use ”*” for all origins or specify domain


## ITEM:
Function: Cross-Origin Resource Sharing settings, allowing web browsers to access
the server from diﬀerent domains


## ITEM:
Maximum upload size (MB)


## ITEM:
• 	YouTube: ComfyUI Tutorials


## ITEM:
```bash
# Section: Model Issues
```
