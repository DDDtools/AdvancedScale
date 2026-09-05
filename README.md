# ◆ `Advanced Scale` tool - V 1.00

> Advanced Scale is a bounding box scaling tool for the Unreal Editor.
Advanced Scale doesn't modify the default Scale tool. It adds a separate scaling tool that changes the position and/or scale of selected objects.
> 
> <p align="center">
>   <img src="Images/Gif_1.gif" height="100" align="middle">
>   <img src="Images/Gif_3.gif" height="100" align="middle">
>   <img src="Images/Gif_5.gif" height="100" align="middle">
>   <img src="Images/Gif_11.gif" height="100" align="middle">
>   <img src="Images/Gif_10_1.gif" height="100" align="middle">
> </p>

<br>

## ◆ `Installation`

> 1. Install the plugin in your project
> 2. Enable Advanced Scale in the Plugins list
>
> <p align="center">
>   <img src="Images/Install.png">
> </p>

<br>

## ◆ `Turn On the Tool`

> Press `Alt+T` (default) or click the three-color button at the top of the viewport. The button position depends on the Unreal Engine version
>
> <p align="center">
>   <img src="Images/Button.png" height="300">
> </p>
<p>&nbsp;</p> 

## ◆ `Advanced Scale usage`

<blockquote>

### 1. Hotkeys

> - `Alt+T` - Turn Advanced Scale on
> - `Ctrl` - Hold `Ctrl` to enable Edge/Corner Handles
> - `Shift` - Hold `Shift` while dragging a handle to scale uniformly
> - `Alt` - Hold `Alt` while dragging a handle to scale from both sides
> - `V` - Hold `V` while dragging a handle to enable vertex snapping

<p>&nbsp;</p>

### 2. Menu

> By default, the menu is located in the lower left corner of the viewport
>
> <p align="center">
>   <img src="Images/Menu.png" height="300">
> </p>
>
> - Corner Handles - Enables Corner and Edge Handles
> - Show in Game View - Displays the Advanced Scale bounding box in Game View mode

<br>

### 3. Face Handles

> **`Face Handles`** are located at the center of each face. Drag a handle to scale the selection along a single axis while the opposite face remains fixed
>
> <p align="center">
>   <img src="Images/Gif_1.gif" height="300">
>   <img src="Images/Gif_2.gif" height="300">
> </p>

<br>

### 4. Edge/Corner Handles

> To activate Edge/Corner handles, hold `Ctrl` or select the `Corner Handles` checkbox from the menu at the bottom left. Hover the mouse over the location where the handle should appear
>
> <p align="center">
>   <img src="Images/CornerHandles.png" height="300" align="middle">
>   <img src="Images/Gif_6.gif" height="300" align="middle">
> </p>
>
> - #### Edge Handles
> `Edge Handles` are located on the edges of the bounding box. Drag a handle to scale the selection along two axes simultaneously while keeping the opposite edges fixed
>
> <p align="center">
>   <img src="Images/Gif_3.gif" height="300">
>   <img src="Images/Gif_4.gif" height="300">
> </p>
>
> - #### Corner Handles
> `Corner Handles` are located at the corners of the bounding box. Drag a handle to scale the selection along all relevant axes while keeping the opposite corner fixed
>
> <p align="center">
>   <img src="Images/Gif_5.gif" height="300">
> </p>

<br>

### 5. Flat Mode
> - #### Planar objects
> When a flat object is selected, `Flat Mode` is activated. `Face Handles` are displayed on only four sides. `Corner Handles` are displayed at the corners
> 
> <p align="center">
>   <img src="Images/Gif_7.gif" height="300">
> </p>
>
> - #### Flattened object
> When an object is flattened below a certain thickness (specified in the plugin settings), `Flat Mode` is activated for `Corner Handles`
>
> <p align="center">
>   <img src="Images/Gif_8.gif" height="300">
> </p>

<br>

### 6. Hotkeys Usage
> - #### Uniform Scale
> Hold `Shift` while dragging a handle to scale uniformly
>
> <p align="center">
>   <img src="Images/Gif_11.gif" height="300">
> </p>
>
> - #### 2-Side Scale
> Hold `Alt` while dragging a handle to scale from both sides
>
> <p align="center">
>   <img src="Images/Gif_12.gif" height="300">
> </p>
>
> - #### Vertex snapping
> Hold `V` while dragging a handle to enable vertex snapping. Move the cursor to the object you want to snap to, even if it is far away. Works with Face, Edge, and Corner Handles
>
> <p align="center">
>   <img src="Images/Gif_13.gif" height="300">
>   <img src="Images/Gif_14.gif" height="300">
> </p>

<br>

> ### 7. Grid snapping
> Enable `Snapping to the grid` to snap the handle to the grid while dragging
> <p align="center">
>   <img src="Images/Gif_15.gif" height="300">
> </p>

<br>

### 8. Multiple Objects $\color{red}{\text{(see the Limitations section for limitations)}}$
> Advanced Scale supports scaling multiple objects simultaneously, including those that are rotated relative to each other
> - #### Multiple objects rotated in 90-degree increments relative to each other
>
> <p align="center">
>   <img src="Images/Gif_9.gif" height="200">
>   <img src="Images/Gif_10.gif" height="200">
> </p>
>
> - #### Multiple objects rotated at arbitrary angles
> When moving the handles, objects are scaled along local axes and shifted relative to the bounding box
>
> <p align="center">
>   <img src="Images/Gif_16.gif" height="300">
> </p>
>
> - #### Local/World Alignment
> If multiple objects have the same rotation or are rotated in 90-degree increments relative to each other, the Scale Bounding Box uses local orientation 
> If multiple objects have different arbitrary rotations, the Scale Bounding Box uses world orientation
>
> <p align="center">
>   <img src="Images/Gif_17.gif" height="200">
>   <img src="Images/Gif_18.gif" height="200">
> </p>
<br>

### 9. $\color{red}{\text{Limitations}}$
> - #### Blueprint Support
> Version 1.00 does not support scaling components inside BP
>
> - #### Blueprint Scaling
> Blueprints in the scene do not scale correctly if their components are rotated relative to each other. Components are scaled along their local axes. Uniform BP scaling works as expected
>
> <table>
>   <tr>
>     <td align="center">
>       <img src="Images/Gif_19.gif" height="300"><br>
>       BP components with matching rotations
>     </td>
>     <td align="center">
>       <img src="Images/Gif_20.gif" height="300"><br>
>       BP components with different rotations
>     </td>
>       <td align="center">
>       <img src="Images/Gif_21.gif" height="300"><br>
>       Uniform scaling
>     </td>
>   </tr>
> </table>
>
> - #### Level Instance Scaling
> Level Instances with components rotated relative to each other may not scale correctly. Components are scaled along their local axes.
> Uniform LI scaling works as expected. Objects inside a Level Instance are scaled in the same way as multiple selected objects in the scene
>
> <table>
>   <tr>
>     <td align="center">
>       <img src="Images/Gif_19.gif" height="300"><br>
>       LI components are rotated equally
>     </td>
>     <td align="center">
>       <img src="Images/Gif_20.gif" height="300"><br>
>       LI components are rotated differently
>     </td>
>       <td align="center">
>       <img src="Images/Gif_22.gif" height="300"><br>
>       Scaling inside LI
>     </td>
>   </tr>
> </table>
>
</blockquote>

## ◆ `Plugin Settings`

> Go to `Editor Preferences > Plugins > Advanced Scale`

> ### 1. Appearance
> - Edge Color — Changes the color of the bounding frame
> - Face Handle Color — Changes the color of the handles located at the center of each face
> - Corner Handle Color — Changes the color of the two-axis corner handles
> - Box Corner Handle Color — Changes the color of the three-axis handles located at the actual corners of the box
>
> ### 2. Viewport Menu Settings
> - Bottom Offset (px) — Sets the distance between the bottom of the viewport and the Advanced Scale menu
> - Show Modifier Hints —Shows or hides the modifier key hints at the bottom of the viewport: `Ctrl — Corner Handles, Shift — Uniform Scale, Alt — Mirror Scale`
>
> ### 3. Point Handles
> - Interaction Radius (px) — Sets how close the mouse cursor must be to a point handle for it to react. This value is measured in screen pixels
>
> ### 4. Vertex Snapping
> - Search Radius — Sets the maximum world-space distance around the current mouse position used to search for vertex snap targets while holding `V`
> - Screen Snap Radius (px) — Sets how close a vertex must appear to the cursor on screen before it can be selected as a snap target
>
> ### 5. Flat Mode
> - Flat Mode Threshold — Determines when a thin object is treated as flat. The value is relative to its other dimensions: for example, 0.05 means 5%
