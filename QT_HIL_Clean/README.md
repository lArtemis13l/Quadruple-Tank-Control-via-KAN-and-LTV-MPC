# Hardware Implementation Environment (Raw Artifacts)

**Warning:** This directory contains the raw C code used to generate the results for the IEEE ICCA submission. To preserve the scientific integrity of the experiments and the exact state that produced the figures, these files have **not** been refactored or sanitized.

## File Guide

While the codebase is raw, the following files represent the core workflow:

*   **`.settings`**: STM32CubeIDE settings.
*   **`Core`**: The .c and .h files used in implementation.
*   **`Drivers`**: Directory containing drivers used in the simulation.

Hardware implentation requires USART3 **enabled**. Ensure that the **`QT_HIL_Clean.ioc`** is properly configured and communication speed is set to 921600 baud before proceeding on.

## Note on Code Style
These notebooks are effectively "Digital Laboratory Notes." They contain debug prints, experimental branches, and intermediate outputs. They are provided "AS IS" under the Apache 2.0 license to ensure transparency and reproducibility of the 1µs vs 19ms (stutters reaching 81ms) benchmark results.
