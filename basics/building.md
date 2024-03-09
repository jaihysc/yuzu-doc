# Building Yuzu

Requires: Visual Studio 2022 (older versions may work)

1. Download the Yuzu source code

2. Inside the Yuzu directory, run

    ```bash
    git submodule update --init --recursive
    ```

3. Download `glslangValidator.exe` from [glslang main-tot](https://github.com/KhronosGroup/glslang/releases), extract it somewhere and add that folder to `PATH` environmental variable. Restart your computer.

4. Open the Yuzu directory in Visual Studio, configure CMake cache

5. Change the target to `yuzu.exe`

6. Build the project