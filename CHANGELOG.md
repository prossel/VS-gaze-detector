# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [1.3.0] - 2022-06-21

### Changed

- Renamed events with "On" prefix: OnGazeEnter, OnGazeExit, OnGazeTimer to be coherent with other similar events (OnEnter, OnTriggerEnter...)

### Added

- OnGazeStay subgraph. Available in the fuzzy finder, usage is similar to OnTriggerStay.

### Deprecated

- RotateOnGaze subgraph is replaced by RotateOnGazeStay

## [1.2.0] - 2022-06-10

### Added

- GazeEnter, GazeExit, GazeTimer subgraphs. Available in the fuzzy finder, easier than using custom events.

### Deprecated

- VSGazeTimer is replaced by GazeTimer, see [UPGRADE.md](UPGRADE.md)

## [1.1.0] - 2022-05-13

### Added

- VSGazeTimer

## [1.0.0] - 2022-05-11

### Added

- Initial version
