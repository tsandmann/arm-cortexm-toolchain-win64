# arm-cortexm-toolchain-win64
A cross-compiler toolchain for Windows (64 Bit) host and arm-none-eabi targets optimized for cortex-m4f and cortex-m7f.

#### Installation
Checkout somewhere (e.g. to `C:\tools\arm-none-eabi`) and add the `bin` folder of that path (e.g `C:\tools\arm-none-eabi\bin`) to *PATH*.

#### Components and Versions
* gcc 10.1.0, newlib 3.3, binutils 2.34, gdb 9.1 (built with crosstool-ng)
  * newlib is built with nano malloc
  * newlib is available in two versions:
    1. with standard printf (*libc.a*)
    1. with nano formatted io printf (*libc_nano.a*), select with `--specs=nano.specs`
