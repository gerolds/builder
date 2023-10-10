# Readymade.Builder
A framework for prototyping 3D builder games in Unity.

## Overview

Readymade.Builder is designed to be a drop-in featrue extenstion to any 3D game. It can be wholly contained in a single prefab, controls are fully confugurable via InputActionReferences. Any prefab can be placed with it by adding a `Placeable` component to its root. Optionally the prefab can be marked up with `Magnet` component which allow semantic snapping and implcit grids.

## Features

- Place any prefab that contains a renderer at runtime
- Placeable prefabs can be marked up with magnets for semantic snapping
- Automatically generated toolbar UI
- Single-Prefab, Drop-In, Plug-and-Play usage
- Saving and loading of placed object
- Simple statics system that discovers placed objects that have become disconnected from the ground or a foundation (e.g. for auto-destruct)
- Gameplad support
- Mouse & keyboard support

## Requirements

- Unity 2022.3.0 or later with the following packages installed:
  - Splines
  - Cinemachine
  - InputSystem
  - TextMeshPro
  - ProBuilder
  - Universal Render Pipeline (only for visual feedback, the builder module doesn't care)
  - Shader Graph (only for visual feedback, the builder module doesn't care)
  - Visual Effects Graph (only for visual feedback, the builder module doesn't care)
  - [Newtonsoft JSON](https://docs.unity3d.com/Packages/com.unity.nuget.newtonsoft-json@3.2/manual/index.html) (Used for runtime persistence)


## 3rd Party Dependencies (Open Source)

- [Vertx.Debugging](https://github.com/vertxxyz/Vertx.Debugging) (Used for drawing all gizmos)
- [UniTask](https://github.com/Cysharp/UniTask) (Used for all async operations)
- [NaughtyAttributes](https://github.com/dbrizov/NaughtyAttributes) (Used for modal inspectors until custom inspectors are added)
- [Newtonsoft JSON for Unity](https://github.com/applejag/Newtonsoft.Json-for-Unity) (Used for runtime persistence)
- [Graphy](https://openupm.com/packages/com.tayx.graphy/) (Performance monitor)

## 3rd Party Dependencies (Commercial)

These are optional for use with the builder module, but for building an actual project these are pretty much required. Make sure you have them installed if you want to use the unity project, they are not included in the repo and expected to be installed to their default location.

- A* Pathfinding Project Pro (Required for threaded, runtime recalculation of navmeshes)
- Quantum Console (Can technically be replaced by your own implementation)
