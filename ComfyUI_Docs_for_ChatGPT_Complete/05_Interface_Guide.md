# SECTION: INTERFACE_GUIDE


## ITEM:
• 	Standard Canvas Mode: Added standard canvas mode, can be switched in Lite
Graph > Canvas > Canvas Navigation Mode


## ITEM:
You can also temporarily hide links in the Canvas Menu.


## ITEM:
We are also continuously improving the native reroute functionality in litegraph. We
recommend using this feature in the future to reorganize connections.


## ITEM:
Color-coding


## ITEM:
_____________________________________
_____________________________________
_____________________________________
Interface Guide


## ITEM:
Mask Editor - Create and Edit Masks in ComfyUI


## ITEM:
Learn how to use the Mask Editor in ComfyUI, including settings and usage
instructions


## ITEM:
The Mask Editor is a very useful feature in ComfyUI that allows users to create and edit
masks within images without needing to use other applications.


## ITEM:
The Mask Editor is currently triggered through the Load Image node. After uploading
an image, you can right-click on the node and select Open in MaskEditor from the
menu to open the Mask Editor.


## ITEM:
You can then click with your mouse on the image to create and edit masks.


## ITEM:
Interface Guide


## ITEM:
_____________________________________
_____________________________________
_____________________________________
Interface Guide


## ITEM:
_____________________________________
_____________________________________
_____________________________________
Interface Guide


## ITEM:
_____________________________________
_____________________________________
_____________________________________
ComfyUI Settings


## ITEM:
ComfyUI Settings Overview


## ITEM:
Detailed description of ComfyUI settings overview


## ITEM:
This section covers detailed setting descriptions in the ComfyUI
frontend settings menu. All user settings are automatically saved
to the ComfyUI/user/default/comfy.settings.json file.


## ITEM:
You can use the Ctrl + , keyboard shortcut to open the settings
panel, then click on the corresponding setting options to
configure them.


## ITEM:
ComfyUI Settings Menu


## ITEM:
```bash
# Table of Contents
```


## ITEM:
4. Lite Graph - Detailed description of Canvas (Lite Graph) setting
options in ComfyUI


## ITEM:
5. Appearance - Modify ComfyUI appearance options such as
themes, background colors, sidebar position, etc.


## ITEM:
6. Extension - Manage the enable/disable status of frontend
extension plugins in ComfyUI


## ITEM:
7. 3D - Some setting options for 3D node initialization


## ITEM:
8. Comfy Desktop - Desktop update settings, mirror settings, etc.
(only eﬀective for ComfyUI Desktop)


## ITEM:
9. Mask Editor - Adjust mask editor usage preferences


## ITEM:
10. Keybinding - Modify ComfyUI keyboard shortcut settings


## ITEM:
12. About - Learn about current ComfyUI version information,
device runtime information, etc., which is very useful for daily
feedback


## ITEM:
13. Server Config


## ITEM:
Modify ComfyUI configuration file, this setting is only eﬀective for ComfyUI
Desktop


## ITEM:
```bash
# Section: User
```


## ITEM:
ComfyUI Settings


## ITEM:
Account Management


## ITEM:
In this document, we will introduce the account management features of ComfyUI,
including account login, registration, and logout operations.


## ITEM:
ComfyUI Settings


## ITEM:
Credits Management


## ITEM:
In this article, we will introduce ComfyUI’s credit management features, including how
to obtain, use, and view credits.


## ITEM:
ComfyUI Settings


## ITEM:
Comfy Settings


## ITEM:
Detailed description of ComfyUI core setting options


## ITEM:
• 	Function: Select the implementation method of the node search box
(experimental feature). If you select litegraph (legacy), it will switch to the early
ComfyUI search box


## ITEM:
Node Widget


## ITEM:
Widget control mode


## ITEM:
• 	Options: before, after


## ITEM:
Save and restore canvas position and zoom level in workflows


## ITEM:
• 	Default Value: Enabled


## ITEM:
• 	Function: Controls whether to save and restore canvas position and zoom level
in workflows, restoring the previous view state when reopening workflows


## ITEM:
ComfyUI Settings


## ITEM:
ComfyUI LiteGraph (Canvas) Settings


## ITEM:
Detailed description of ComfyUI graphics rendering engine LiteGraph setting options


## ITEM:
LiteGraph is the underlying graphics rendering engine of ComfyUI. The settings in this
category mainly control the behavior and appearance of graphical interfaces such as
canvas, nodes, and links.


## ITEM:
Canvas


## ITEM:
Show selection toolbox


## ITEM:
• 	Default Value: Enabled


## ITEM:
• 	Function: When rendering the interface, especially when the workflow is
particularly complex and the entire canvas is particularly large, the frontend
rendering of corresponding elements will consume a lot of memory and cause
lag. By lowering this threshold, you can control elements to enter low quality
rendering mode when scaled to a specific percentage, thereby reducing memory
consumption. The corresponding diﬀerent rendering modes are shown below


## ITEM:
Maximum FPS


## ITEM:
• 	Default Value: 0 (use screen refresh rate)


## ITEM:
• 	Range: 0 - 120


## ITEM:
• 	Function: Limits the rendering frame rate of the canvas. 0 means using the
screen refresh rate. Higher FPS will make the canvas rendering smoother, but
will also consume more performance. Too low values will cause more obvious
stuttering.


## ITEM:
Always snap to grid


## ITEM:
• 	Default Value: Disabled


## ITEM:
• 	Function: When this option is not enabled, you can hold the Shift key to align
node edges with the grid. When enabled, node edges will automatically align
with the grid without holding the Shift key.


## ITEM:
Snap to grid size


## ITEM:
• 	Range: 1 - 500


## ITEM:
Show graph canvas menu


## ITEM:
• 	Default Value: Enabled


## ITEM:
• 	Function: Controls whether to display the canvas menu in the bottom right
corner


## ITEM:
The canvas menu is located in the bottom right corner of the entire ComfyUI interface,
containing operations such as canvas zooming, temporarily hiding all connections,
quickly scaling the workflow to fit the canvas, etc., as shown in the image below


## ITEM:
Canvas zoom speed


## ITEM:
• 	Default Value: 1.1


## ITEM:
• 	Range: 1.01 - 2.5


## ITEM:
• 	Function: Controls the speed of canvas zooming, adjusts the sensitivity of
mouse wheel zooming


## ITEM:
Show canvas info on bottom left corner (fps, etc.)


## ITEM:
• 	Default Value: Enabled


## ITEM:
• 	Function: Controls whether to display canvas information in the bottom left
corner, showing performance metrics like FPS


## ITEM:
Context Menu


## ITEM:
Scale node combo widget menus (lists) when zoomed in


## ITEM:
• 	Default Value: Enabled


## ITEM:
• 	Function: Controls whether to scale node combo widget menus (lists) when
zoomed in, allowing users to select node combo widgets


## ITEM:
Graph


## ITEM:
Link Render Mode


## ITEM:
• 	Default Value: 2 (Spline)


## ITEM:
• 	Options: Straight, Linear, Spline, Hidden


## ITEM:
• 	Function: This setting enables trackpad mode for the canvas, allowing two-
finger pinch zoom and drag.


## ITEM:
Double click interval (maximum)


## ITEM:
• 	Default Value: 300


## ITEM:
• 	Function: Maximum time (milliseconds) between two clicks of a double-click.
Increasing this value helps solve issues where double-clicks are sometimes not
recognized.


## ITEM:
Pointer click drift delay


## ITEM:
• 	Default Value: 150


## ITEM:
• 	Function: Maximum time (milliseconds) to ignore pointer movement after
pressing the pointer button. Helps prevent accidental mouse movement when
clicking.


## ITEM:
Pointer click drift (maximum distance)


## ITEM:
• 	Default Value: 6


## ITEM:
• 	Function: If the pointer moves more than this distance while holding the button,
it is considered a drag (rather than a click). Helps prevent accidental mouse
movement when clicking.


## ITEM:
Reroute


## ITEM:
Reroute spline oﬀset


## ITEM:
• 	Default Value: 20


## ITEM:
ComfyUI Settings


## ITEM:
Customizing ComfyUI Appearance


## ITEM:
Learn how to customize the appearance of ComfyUI using color palettes and
advanced CSS options


## ITEM:
ComfyUI oﬀers flexible appearance customization options that allow you to personalize
the interface to your preferences.


## ITEM:
Color Palette System


## ITEM:
The primary way to customize ComfyUI’s appearance is through the built-in color
palette system.


## ITEM:
This allows you to:


## ITEM:
1. Switch ComfyUI themes


## ITEM:
2. Export the currently selected theme as JSON format


## ITEM:
3. Load custom theme configuration from JSON file


## ITEM:
4. Delete custom theme configuration


## ITEM:
For appearance needs that cannot be satisfied by the color palette, you can perform
advanced appearance customization through the user.css file


## ITEM:
How to Customize Color Themes


## ITEM:
"litegraph_base": {             // LiteGraph base interface configuration


## ITEM:
"BACKGROUND_IMAGE": "",        // Background image, default is empty


## ITEM:
"CLEAR_BACKGROUND_COLOR": "#222", // Main canvas background color


## ITEM:
"NODE_TITLE_COLOR": "#999",    // Node title text color


## ITEM:
"NODE_SELECTED_TITLE_COLOR": "#FFF", // Selected node title color


## ITEM:
"NODE_TEXT_SIZE": 14,          // Node text size


## ITEM:
"NODE_TEXT_COLOR": "#AAA",     // Node text color


## ITEM:
"NODE_TEXT_HIGHLIGHT_COLOR": "#FFF", // Node text highlight color


## ITEM:
"NODE_SUBTEXT_SIZE": 12,       // Node subtext size


## ITEM:
"NODE_DEFAULT_COLOR": "#333",   // Node default color


## ITEM:
"NODE_DEFAULT_BGCOLOR": "#353535", // Node default background color


## ITEM:
"NODE_DEFAULT_BOXCOLOR": "#666", // Node default border color


## ITEM:
"NODE_DEFAULT_SHAPE": 2,        // Node default shape


## ITEM:
"NODE_BOX_OUTLINE_COLOR": "#FFF", // Node border outline color


## ITEM:
"NODE_BYPASS_BGCOLOR": "#FF00FF", // Node bypass background color


## ITEM:
"NODE_ERROR_COLOUR": "#E00",    // Node error state color


## ITEM:
"DEFAULT_SHADOW_COLOR": "rgba(0,0,0,0.5)", // Default shadow color


## ITEM:
"DEFAULT_GROUP_FONT": 24,       // Group default font size


## ITEM:
"WIDGET_BGCOLOR": "#222",       // Widget background color


## ITEM:
"WIDGET_OUTLINE_COLOR": "#666", // Widget outline color


## ITEM:
"WIDGET_TEXT_COLOR": "#DDD",    // Widget text color


## ITEM:
"WIDGET_SECONDARY_TEXT_COLOR": "#999", // Widget secondary text color


## ITEM:
"WIDGET_DISABLED_TEXT_COLOR": "#666", // Widget disabled state text color


## ITEM:
"LINK_COLOR": "#9A9",          // Connection line color


## ITEM:
"EVENT_LINK_COLOR": "#A86",    // Event connection line color


## ITEM:
"CONNECTING_LINK_COLOR": "#AFA", // Connecting line color


## ITEM:
"BADGE_FG_COLOR": "#FFF",      // Badge foreground color


## ITEM:
"BADGE_BG_COLOR": "#0F1F0F"    // Badge background color


## ITEM:
},


## ITEM:
"comfy_base": {                  // ComfyUI base interface configuration


## ITEM:
"fg-color": "#ﬀf",            // Foreground color


## ITEM:
"bg-color": "#202020",         // Background color


## ITEM:
"comfy-menu-bg": "#353535",    // Menu background color


## ITEM:
"comfy-menu-secondary-bg": "#303030", // Secondary menu background color


## ITEM:
"comfy-input-bg": "#222",      // Input field background color


## ITEM:
"input-text": "#ddd",          // Input text color


## ITEM:
"descrip-text": "#999",        // Description text color


## ITEM:
"drag-text": "#ccc",           // Drag text color


## ITEM:
"error-text": "#ﬀ4444",       // Error text color


## ITEM:
"border-color": "#4e4e4e",     // Border color


## ITEM:
"tr-even-bg-color": "#222",    // Table even row background color


## ITEM:
"tr-odd-bg-color": "#353535",  // Table odd row background color


## ITEM:
"content-bg": "#4e4e4e",       // Content area background color


## ITEM:
"content-fg": "#ﬀf",          // Content area foreground color


## ITEM:
"content-hover-bg": "#222",    // Content area hover background color


## ITEM:
"content-hover-fg": "#ﬀf",    // Content area hover foreground color


## ITEM:
"bar-shadow": "rgba(16, 16, 16, 0.5) 0 0 0.5rem" // Bar shadow eﬀect


## ITEM:
}


## ITEM:
}


## ITEM:
}


## ITEM:
Canvas


## ITEM:
Background Image


## ITEM:
• 	Requirements: ComfyUI frontend version 1.20.5 or newer


## ITEM:
• 	Function: Set a custom background image for the canvas to provide a more
personalized workspace. You can upload images or use web images to set the
background for the canvas.


## ITEM:
Node


## ITEM:
Node Opacity


## ITEM:
.litegraph .litemenu-entry,


## ITEM:
.litemenu-title {


## ITEM:
font-size: 24px !important;


## ITEM:
}


## ITEM:
/* Custom styling for specific elements not available in the color palette */


## ITEM:
.comfy-menu {


## ITEM:
border: 1px solid rgb(126, 179, 189) !important;


## ITEM:
border-radius: 0px 0px 0px 10px !important;


## ITEM:
backdrop-filter: blur(2px);


## ITEM:
}


## ITEM:
Best Practices


## ITEM:
1. Start with the color palette for most customizations


## ITEM:
2. Use user.css only when necessary for elements not covered by the color palette


## ITEM:
3. Export your theme before making significant changes so you can revert if
needed


## ITEM:
4. Share your themes with the community to inspire others


## ITEM:
ComfyUI Settings


## ITEM:
ComfyUI 3D Settings


## ITEM:
Detailed description of ComfyUI 3D setting options


## ITEM:
This section of settings is mainly used to control the initialization settings of 3D-related
components in ComfyUI, including camera, lighting, scene, etc. When creating new 3D
components, they will be initialized according to these settings. After creation, these
settings can still be adjusted individually.


## ITEM:
Camera


## ITEM:
Initial Camera Type


## ITEM:
• 	Options:


## ITEM:
• 	perspective


## ITEM:
• 	orthographic


## ITEM:
• 	Function: Controls whether the default camera is perspective or orthographic
when creating new 3D components. This default setting can still be switched
individually for each component after creation


## ITEM:
Light


## ITEM:
The light settings in this section are used to set the default lighting settings for 3D
components. The corresponding settings in the 3D settings in ComfyUI can also be
modified.


## ITEM:
Light Adjustment Increment


## ITEM:
• 	Default Value: 0.5


## ITEM:
• 	Function: Controls the step size when adjusting light intensity in 3D scenes.
Smaller step values allow for finer light adjustments, while larger values make
each adjustment more noticeable


## ITEM:
Light Intensity Minimum


## ITEM:
• 	Default Value: 1


## ITEM:
• 	Function: Sets the minimum light intensity value allowed in 3D scenes. This
defines the lowest brightness that can be set when adjusting the lighting of any
3D control


## ITEM:
Light Intensity Maximum


## ITEM:
• 	Default Value: 10


## ITEM:
• 	Function: Sets the maximum light intensity value allowed in 3D scenes. This
defines the upper limit of brightness that can be set when adjusting the lighting
of any 3D control


## ITEM:
Initial Light Intensity


## ITEM:
• 	Default Value: 3


## ITEM:
• 	Function: Sets the default brightness level of lights in 3D scenes. This value
determines the intensity with which lights illuminate objects when creating new
3D controls, but each control can be adjusted individually after creation


## ITEM:
Scene


## ITEM:
Initial Background Color


## ITEM:
• 	Function: Controls the default background color of 3D scenes. This setting
determines the background appearance when creating new 3D components, but
each component can be adjusted individually after creation


## ITEM:
• 	Default Value: 282828 (dark gray)


## ITEM:
Change the background color, which can also be adjusted in the canvas.


## ITEM:
Initial Preview Visibility


## ITEM:
• 	Function: Controls whether the preview screen is displayed by default when
creating new 3D components. This default setting can still be toggled
individually for each component after creation


## ITEM:
• 	Default Value: true (enabled)


## ITEM:
Initial Grid Visibility


## ITEM:
• 	Function: Controls whether the grid is displayed by default when creating new
3D components. This default setting can still be toggled individually for each
component after creation


## ITEM:
• 	Default Value: true (enabled)


## ITEM:
Hide or show the grid on initialization


## ITEM:
```bash
# Section: Comfy Desktop
```


## ITEM:
ComfyUI Settings


## ITEM:
Comfy Desktop General Settings


## ITEM:
Detailed description of ComfyUI Desktop general setting options


## ITEM:
General


## ITEM:
Window Style


## ITEM:
Function: Controls the title bar style of the application window


## ITEM:
Automatically check for updates


## ITEM:
Function: Automatically checks for ComfyUI Desktop updates and will remind you to
update when updates are available


## ITEM:
Send anonymous usage metrics


## ITEM:
Function: Sends anonymous usage statistics to help improve the software. Changes to
this setting require a restart to take eﬀect


## ITEM:
UV


## ITEM:
This section is mainly for users in China, because many of the original mirrors used by
Desktop are outside of China, so access may not be friendly for domestic users. You
can set your own mirror sources here to improve access speed and ensure that
corresponding packages can be accessed and downloaded normally.


## ITEM:
Python Install Mirror


## ITEM:
Function:


## ITEM:
```bash
# Section: Mask Editor
```


## ITEM:
ComfyUI Settings


## ITEM:
ComfyUI Mask Editor Settings


## ITEM:
Detailed description of ComfyUI mask editor setting options


## ITEM:
Brush Adjustment


## ITEM:
Brush adjustment speed multiplier


## ITEM:
• 	Function: Controls the speed of brush size and hardness changes during
adjustment


## ITEM:
• 	Description: Higher values mean faster changes


## ITEM:
Lock brush adjustment to dominant axis


## ITEM:
• 	Function: When enabled, brush adjustment will only aﬀect size or hardness
based on the direction you move


## ITEM:
• 	Description: This feature allows users to more precisely control brush property
adjustments


## ITEM:
New Editor


## ITEM:
Use new mask editor


## ITEM:
• 	Function: Switch to the new brush editor interface


## ITEM:
• 	Description: Allows users to switch between new and old editor interfaces


## ITEM:
• 	New Editor


## ITEM:
• 	Old Editor


## ITEM:
The new version has a better UI interface and interaction, with more complete
functionality


## ITEM:
```bash
# Section: Keybinding
```


## ITEM:
ComfyUI Settings


## ITEM:
ComfyUI Keyboard Shortcuts and Custom Settings


## ITEM:
Keyboard and mouse shortcuts for ComfyUI and related settings


## ITEM:
Currently, ComfyUI supports custom keyboard shortcuts. You can set the shortcuts by
clicking on Settings (gear icon) —> Keybinding.


## ITEM:
In the corresponding menu, you can see all the current shortcut settings for ComfyUI.
Click the edit icon before the corresponding command to customize the shortcut.


## ITEM:
Below is the current list of shortcuts for ComfyUI, which you can customize as needed.


## ITEM:
• 	Windows/Linux


## ITEM:
• 	MacOS


## ITEM:
Shortcut Command
Ctrl + Enter Queue prompt
Ctrl + Shift  Queue prompt (Front)
+ Enter
Ctrl + Alt +  Interrupt
Enter


## ITEM:
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


## ITEM:
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
```bash
# Section: Extension
```


## ITEM:
ComfyUI Settings


## ITEM:
Extension Settings


## ITEM:
Detailed description of ComfyUI extension management and setting options


## ITEM:
ComfyUI Settings


## ITEM:
About Page


## ITEM:
Detailed description of ComfyUI About settings page


## ITEM:
The About page is an information display panel in the ComfyUI settings system, used
to show application version information, related links, and system statistics. These
settings can provide us with critical information when you submit feedback or report
issues.


## ITEM:
Version Information Badges


## ITEM:
The About page displays the following core version information:


## ITEM:
• 	ComfyUI Version: Shows the backend ComfyUI version number, linked to the
oﬃcial GitHub repository


## ITEM:
• 	ComfyUI_frontend Version: Shows the frontend interface version number, linked
to the frontend GitHub repository


## ITEM:
• 	Discord Community: Provides a link to the ComfyOrg Discord server


## ITEM:
ComfyUI Settings


## ITEM:
Server Config


## ITEM:
Detailed description of ComfyUI server configuration options


## ITEM:
Currently the Server Config settings menu only exists in the Desktop version, and this
settings menu item does not exist in other versions


## ITEM:
Network


## ITEM:
Host: The IP address to listen on


## ITEM:
• 	Function: Sets the IP address the server binds to. Default 127.0.0.1 means only
local access is allowed. If you need LAN access, you can set it to 0.0.0.0


## ITEM:
• Disable node validation in ComfyUI settings
