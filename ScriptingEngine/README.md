# Custom Scripting Engine - Unity-Style MonoBehavior System

## Overview
This project was developed as part of a 6-month university team project to build a custom game engine from scratch.
My primary responsibility was the design and implementation of the scripting engine, inspired by Unity's
MonoBehaviour lifecycle, to support rapid prototyping and code portability.

During the first phase of development, the team used Unity to prototype gameplay while the custom engine was
under development. The scripting system was designed to closely match Unity's lifecycle semantics so prototype
code could be ported with minimal changes.

---

## My Role
**Primary Responsibility:** Scripting Engine / Runtime Systems

- Designed a Unity-style script lifecycle system (Start, Update, FixedUpdate, etc.)
- Implemented script binding to engine entities
- Defined execution order and lifecycle state transitions
- Matched Unity execution semantics to reduce porting friction
- Supported designers prototyping gameplay in Unity during early development

---

## Key Features
- MonoBehavior-style lifecycle management
- Enable / disable handling for scripts
- Runtime-safe creation and destruction of script instances
- Deterministic update ordering
- Unity-to-custom-engine API mapping for scripting code

---

## Technical Notes
- Script instances are registered with the scripting system and invoked during engine update phases
- Lifecycle transitions are explicitly managed to avoid invalid references during iteration
- Hot-reloading were intentionally omitted due to project scope and time constraints

---

## Prototype Gameplay (Contextual Reference)
**YouTube Playlist:** [Prototype Gameplay](https://www.youtube.com/watch?v=EXNcuSXSgZI&list=PLUyRFwTbZyB40iWJgs44lSrRT4p3lXsW3&index=1)

> Note: The gameplay footage shows a Unity-based prototype created by the design team.  
> My contribution was focused on the scripting engine architecture and lifecycle design rather than gameplay
> systems shown in the videos.

---

## Source Code Availability
The full engine source code is part of a shared university project and is not publicly available.
This page documents the scripting system's architecture, design goals, and behavior.
