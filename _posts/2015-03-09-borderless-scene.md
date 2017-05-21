---
layout: page
title: BorderlessScene
categories: Java
icon: java.svg
---
# BorderlessScene

Undecorated JavaFX Scene with implemented move, resize, minimise, maximise, close and Windows Aero Snap controls.

Usage:
```java
// Constructor using your primary stage and the root Parent of your content.
BorderlessScene scene = new BorderlessScene(yourPrimaryStage, yourParent);
yourPrimaryStage.setScene(scene); // Set the scene to your stage and you're done!

// Maximise (on/off) and minimise the application:
scene.maximise();
scene.minimise();

// To move the window around by pressing a node:
scene.setMoveControl(yourNode);

// To disable resize:
scene.setResizable(false);

// To switch the content during runtime:
scene.setContent(yourNewParent);

// Check if maximised:
Boolean bool = scene.isMaximised();

// Get windowed* size and position:
scene.getWindowedSize();
scene.getWindowedPosition();
```
_*windowed = not maximised_

[View the project on GitHub](https://github.com/NicolasSenet-Larson/BorderlessScene)
