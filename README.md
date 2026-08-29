#  Advanced Scale

Advanced Scale is a bounding box scaling tool for Unreal editor



## 1. Face Handles
Located at the center of each face. Drag a handle to scale the selection along a single axis while the opposite face remains fixed.

<p align="center">
  <img src="Images/Gif_1.gif" width="49%">
  <img src="Images/Gif_2.gif" width="49%">
</p>

## 2. Edge Handles
Located on the edges of the bounding box. Drag a handle to scale the selection along two axes simultaneously while keeping the opposite edges fixed.

## 3. Corner Handles
Located at the corners of the bounding box. Drag a handle to scale the selection along all relevant axes while keeping the opposite corner fixed.





......

**Editor Scale Box** is an Unreal Engine editor tool for intuitive object scaling and bounding-box editing directly in the viewport.

It adds a custom Scale Box mode to the Unreal Editor, allowing you to manipulate an object's bounds using interactive handles while keeping the workflow familiar to Unreal Engine users.

> **Status:** Work in progress

## Features

- Local-space bounding box around the selected actor
- Interactive box faces for resizing
- Works directly inside the Unreal Editor viewport
- Bounding box follows object translation, rotation, and scale
- Support for Unreal Engine grid snapping
- Vertex snapping support
- Customizable box color and transparency
- Support for different actor types
- Designed as a native Unreal Engine editor plugin

## Supported Unreal Engine Versions

Currently being developed and tested with:

- Unreal Engine 5.3

Support for additional Unreal Engine 5 versions is planned.

## Preview

Screenshots and videos will be added during development.

<!--
![Editor Scale Box](Images/EditorScaleBox.jpg)
-->

## Installation

Editor Scale Box is not currently distributed through this repository.

The plugin is planned for release through **Fab**.

A download link and installation instructions will be added here when the plugin becomes available.

## Usage

1. Select an actor in the Unreal Editor viewport.
2. Activate **Editor Scale Box** from the viewport toolbar.
3. The local bounding box appears around the selected actor.
4. Select and drag a box face to resize the object along the corresponding local axis.
5. Standard Unreal Engine viewport transformations remain available while the tool is active.

## Development

Editor Scale Box is currently under active development.

Planned improvements include:

- Improved interaction with box faces
- Grid snapping
- Vertex snapping
- Plugin settings
- Additional actor type support
- Support for multiple Unreal Engine versions

## Feedback

Bug reports, feature requests, and general feedback are welcome through GitHub Issues.

## License

The plugin itself is **not open source** and is not distributed through this repository.

This repository is used for documentation, previews, release information, and issue tracking.
