# Switch Hardware Emulation

Located in `/src/core`.

These files are used to emulate the Switch hardware. The top-level class is `Core::System`.

ARM CPU is emulated using JIT with [dynarmic](https://github.com/yuzu-mirror/dynarmic).

Debugger GDB can be remotely connected.