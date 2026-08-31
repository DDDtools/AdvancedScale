# ◆ `Advanced Scale` tool

> Advanced Scale is a bounding box scaling tool for the Unreal Editor

<br>

## ◆ `Installation`

> 1. Install the plugin to your project
> 2. Enable Advanced Scale in the plugin list
>
> <p align="center">
>   <img src="Images/Install.png">
> </p>

<br>

## ◆ `Turn on Tool`

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
> - Corner Handles - Turn on Corner and Edge handles
> - Local Offset - Adjusts each object’s position along its local axes while scaling
> - Show in Game View - Display bounding box of Advanced Scale tool in Game View mode

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

> To activate Edge/Corner handles, hold `Ctrl` or select the `Corner Handles` checkbox from the menu at the bottom left. Hover your mouse over the place where the handle should be
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
> When a flat object is selected, `Flat Mode` is activated. `Face Handles` are displayed only on four sides. `Corner Handles` are displayed in corners
> 
> <p align="center">
>   <img src="Images/Gif_7.gif" height="300">
> </p>
>
> - #### Flattened object
> When an object is flattened to a certain thickness (specified in the plugin settings), `Flat Mode` is activated for `Corner Handles`
>
> <p align="center">
>   <img src="Images/Gif_8.gif" height="300">
> </p>

<br>

### 6. Hotkeys usage
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
> Hold `V` while dragging a handle to enable vertex snapping
>
> <p align="center">
>   <img src="Images/Gif_12.gif" height="300">
> </p>








### 7. Multi objects
> - #### Multiple objects
> Advanced Scale supports scaling multiple objects simultaneously, including those that are rotated relative to each other $\color{red}{\Large\text{(see the Limitations section for limitations)}}$
>
> <p align="center">
>   <img src="Images/Gif_9.gif" height="200">
>   <img src="Images/Gif_10.gif" height="200">
> </p>
