# Project Overview

## File Structure

Explanation of the different directories in Yuzu source code.

| Path | Description |
| - | - |
| `/.ci`          | Continuous Integration configuration |
| `/.github`      | GitHub repository workflows and templates |
| `/.reuse`       | License information |
| `/CMakeModules` | CMake modules |
| `/dist`         | Files used by the program, such as its icon |
| `/externals`    | Git submodules |
| `/hooks`        | Git hooks |
| `/LICENSES`     | Copies of software licenses |
| `/src`          | Source code |
| `/tools`        | Scripts and various tools |

| Path | Description |
| - | - |
| `/src/android`           | Separate Java application for Android UI |
| `/src/audio_core`        | Emulate Switch audio |
| `/src/common`            | Common functionality used around the programs |
| `/src/core`              | Emulate Switch hardware |
| `/src/dedicated_room`    | Separate application for hosting dedicated rooms |
| `/src/frontend_common`   | Common functionality used by the desktop UI |
| `/src/hid_core`          | Emulate Switch inputs |
| `/src/input_common`      | Common functionality for handling inputs to Yuzu |
| `/src/network`           | Networking multiplayer sessions |
| `/src/shader_recompiler` | Recompile Switch shaders for the current machine |
| `/src/tests`             | Tests |
| `/src/video_core`        | GPU rendering |
| `/src/web_service`       | Yuzu web services (telemetry, announcing multiplayer rooms) |
| `/src/yuzu`              | Separate application for desktop UI |
| `/src/yuzu_cmd`          | Separate application for desktop command line UI |

| Path | Description |
| - | - |
| `/src/audio_core/adsp`     | Represents Application Digital Signal Processor (ADSP) used for audio |
| `/src/audio_core/common`   | Common functionality used by audio |
| `/src/audio_core/device`   | Input output audio streams |
| `/src/audio_core/in`       | Audio input to emulated Switch |
| `/src/audio_core/opus`     | Handles Opus audio format |
| `/src/audio_core/out`      | Audio output from emulated Switch |
| `/src/audio_core/renderer` | Emulate Switch Audio system |
| `/src/audio_core/sink`     | Audio sinks |

| Path | Description |
| - | - |
| `/src/core/arm`      | Emulates ARM CPU |
| `/src/core/crypto`   | Cryptography and Switch encryption schemes |
| `/src/core/debugger` | Debugger support |
| `/src/core/file_sys` | Switch File system |
| `/src/core/frontend` | Interface for rendering emulated system |
| `/src/core/hle`      | High-level emulation (HLE) of kernel (firmware) features |
| `/src/core/frontend` | Emulates Switch network |
| `/src/core/loader`   | Loads various file formats (NSP, NCA, etc) |
| `/src/core/memory`   | Handles cheats |
| `/src/core/tools`    | Various tools for working with emulated system |

| Path | Description |
| - | - |
| `/src/hid_core/frontend`  | Emulate Switch touch, motion, controller inputs |
| `/src/hid_core/hidbus`    | Emulate special Switch devices (Ring-Con) |
| `/src/hid_core/irsensor`  | Emulate Joy-Con IR sensor |
| `/src/hid_core/resources` | Represents various HIDs of the Switch (buttons, motion sensors, etc) |

| Path | Description |
| - | - |
| `/src/input_common/drivers` | Represents various inputs to Yuzu |
| `/src/input_common/helpers` | Common functionality used by input_common |

| Path | Description |
| - | - |
| `/src/shader_recompiler/backend`  | Generate shader output for computer running Yuzu from intermediate representation (IR) |
| `/src/shader_recompiler/frontend` | Process Switch shader inputs into intermediate representation (IR) |
| `/src/shader_recompiler/ir_opt`   | Intermediate representation (IR) optimizer |

| Path | Description |
| - | - |
| `/src/video_core/buffer_cache`    | Vulkan buffer cache |
| `/src/video_core/control`         | Holds rendering commands from Switch |
| `/src/video_core/engines`         | Represents Switch Nvidia Tegra rendering hardware |
| `/src/video_core/host_shaders`    | Shaders for the computer running Yuzu |
| `/src/video_core/host1x`          | Represents Switch Nvidia Tegra host1x module |
| `/src/video_core/macro`           | Used to implement macros in Maxwell 3D engine |
| `/src/video_core/query_cache`     | Vulkan query cache |
| `/src/video_core/renderer_null`   | Renderer which does nothing |
| `/src/video_core/renderer_opengl` | OpenGL renderer |
| `/src/video_core/renderer_vulkan` | Vulkan renderer |
| `/src/video_core/textures`        | Converts textures from Switch |
| `/src/video_core/texture_cache`   | Holds textures that have been converted from Switch |
| `/src/video_core/vulkan_common`   | Common functionality for Vulkan renderer |

| Path | Description |
| - | - |
| `/src/yuzu/applets`       | Dialogs on the Switch recreated in Qt (keyboard, controller select) |
| `/src/yuzu/configuration` | Configuration menu |
| `/src/yuzu/debugger`      | Debugger menu |
| `/src/yuzu/multiplayer`   | Multiplayer menu |
| `/src/yuzu/util`          | Common functionality used in UI |

## Project Structure

The project has 4 applications (different executables) which are compiled.

| Application Path | Description |
| - | - |
| `/src/android`        | Java application for Android UI |
| `/src/dedicated_room` | Hosting dedicated rooms |
| `/src/yuzu`           | Desktop UI |
| `/src/yuzu_cmd`       | Desktop command line UI |