# Eclipse-Arrebol

**HPC · GPU Computing · CUDA · Linux Kernel · Low-level Systems**

I build and study systems across the boundary between software and hardware, from Linux device drivers and GPU runtimes to compute kernels and LLM inference. I use hands-on projects to understand how memory, execution, and data movement fit together.

## Tech Stack

- **Languages:** C, C++, CUDA, RISC-V assembly
- **Systems:** Linux kernel, PCI drivers, QEMU, memory management
- **GPU computing:** Kernel programming, GPU runtimes, KV caching, LLM inference

## Selected Projects

### [gpgpu_driver](https://github.com/Eclipse-Arrebol/gpgpu_driver)

An experimental GPGPU software stack for a QEMU virtual GPU, connecting a Linux PCI driver to a user-space runtime and hand-written RV32 GPU kernels.

- Kernel dispatch through `mmap` and `ioctl`, with interrupt-based completion.
- Buddy and slab VRAM allocation, plus a Qwen2-0.5B FP32 token-level greedy inference demo.

### [LiteLLMEngine](https://github.com/Eclipse-Arrebol/LiteLLMEngine)

A learning-oriented C++/CUDA inference engine for Qwen3, exploring the internals of LLM decoding and request execution.

- Tensor storage, weight loading, core inference operators, and contiguous and paged KV caches.
- Multi-request generation and batch decode, with a CUDA paged attention kernel that reads KV pages through block tables.

## Blog

[**Read my notes and write-ups →**](https://eclipse-arrebol.pages.dev/)
