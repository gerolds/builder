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

- Unity 2022.3.0 or later.
