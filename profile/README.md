# Amora

Amora develops powerful, modular tools for game development. We believe in clean architecture, open source practices, and providing developers with engines and tools that are extensible, testable, and production-ready.

## Our Products

### [Sero](https://github.com/amora/sero) — Game Engine

**Status:** Active  
**License:** MIT (Open Source)

A modular C++23 game engine designed for 2D games with integrated rendering, physics, audio, and scripting capabilities.

#### Core Features

**Architecture & Design**
- **Layered architecture** with explicit interfaces (IApplication, IScene, IRenderer, etc.)
- **Entity-Component-System (ECS)** — `EntityManager`, `ComponentRegistry`, `SystemExecutor` with deterministic stage execution
- **Clean separation** of concerns — easily swap backends and mock subsystems for testing

**Simulation & Rendering**
- **Fixed-step simulation** — Configurable tick rate (20 TPS default), arbitrary FPS rendering
- **Tick accumulator** — Handles variable frame times gracefully
- **OpenGL rendering** via GLFW — Direct hardware access with clean abstraction layer

**Scripting & Logic**
- **Lua 5.4 integration** — Full-featured scripting with sol2 C++ bindings
- **Hot-reload support** — Scripts can be modified and reloaded without restarting
- **ScriptComponent** — Lua lifecycle hooks: `on_start`, `on_update`, `on_destroy`

**Integrated Subsystems**
- **Physics** — Box2D 2D physics engine
- **Audio** — miniaudio backend with spatial audio support
- **Input handling** — GLFW with virtual action mapping and rebinding
- **Asset management** — Typed asset loader system with hot-reload
- **Filesystem abstraction** — File watching and path handling
- **Text rendering** — FreeType font rendering and glyph rasterization
- **Job system** — Thread pool for background tasks
- **Event bus** — Deferred event dispatch for decoupled game logic
- **Logging** — spdlog integration with pluggable backends
- **Debug UI** — Optional Dear ImGui overlay (toggled with F3)

#### Built-in Dependencies

All required libraries are included:
- GLFW (windowing & input)
- OpenGL (graphics)
- Box2D (2D physics)
- Lua 5.4 (scripting)
- sol2 (C++/Lua bindings)
- miniaudio (audio)
- spdlog (logging)
- FreeType (font rendering)
- nlohmann/json (serialization)
- stb (image loading)
- Dear ImGui (debug UI)

#### Design Philosophy

Sero follows clean architecture principles with emphasis on:
- **Testability** — Interface-based design allows mocking and unit testing
- **Extensibility** — Swap rendering backends, audio systems, or physics engines
- **Portability** — Minimal platform-specific code through abstraction layers
- **Determinism** — Fixed-tick simulation enables replays and network synchronization

### Project Atlas

**Status:** In Development  
**Tagline:** Developer Tooling

A comprehensive suite of developer tools for game development workflow optimization. Details coming soon at preview.

### Project Lumen

**Status:** Research & Development  
**Tagline:** R&D Initiatives

Exploratory research initiatives in our pipeline. More information will be announced as projects mature.

## Getting Started

- **Repository** — [https://github.com/amora/sero](https://github.com/amora/sero)

## About Amora

We're building the next generation of game development tools. Our focus is on:
- **Quality** — Production-ready code with comprehensive documentation
- **Openness** — MIT-licensed, community-driven development
- **Simplicity** — Intuitive APIs without sacrificing power
- **Performance** — Efficient implementations with minimal overhead

---

*Organization repository setup with [Claude Code](https://claude.com/claude-code)*
