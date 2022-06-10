# VS Gaze Detector

A gaze detector using Visual Scripting.

[https://github.com/prossel/VS-gaze-detector](https://github.com/prossel/VS-gaze-detector)

![screenshot](Screenshots/GazeEvents.png)

## Installation

* Download latest .unitypackage file from [https://github.com/prossel/VS-gaze-detector/releases](https://github.com/prossel/VS-gaze-detector/releases)
* Add to your unity project

## Getting started

### Add the GazeRaycaster to the camera

* Add a Script Machine component to the Main Camera game object
* Select the GazeRaycaster graph
* Optionnally add another script machine connected to the Mouse Look Around graph

  ![Camera setup](Screenshots/CameraGazeRaycaster.png)

### Use the gaze events

* Add a script machine to an object your want to react on gaze events
* Edit the graph
* Use the fuzzy finder to add a GazeEnter (in Nesting) subgraph
  ![Add GazeEnter](Screenshots/FuzzyAddGazeEnter.png)
* Connect the GazeEnter node to whatever you want
  ![Add GazeEnter](Screenshots/GazeEnter.png)
* Repeat the same process for the GazeExit or GazeTimer

### GazeTimer

The GazeTimer event triggers its output after a configurable delay (duration input parameter) has elapsed, following the GazeEnter event. It does not trigger if the GazeExit occurs before the duration.

When the repeat parameter is checked, then the timer will trigger again after each duration.

## History

See [CHANGELOG.md](CHANGELOG.md)
