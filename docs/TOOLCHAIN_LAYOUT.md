# CBCubeIDE Toolchain Layout

Every toolchain must extract into:

toolchains/
└── <toolchain>/
    ├── bin/
    ├── lib/
    ├── libexec/
    ├── share/
    └── manifest.json

Examples:

toolchains/avr/
toolchains/arm/
toolchains/esp32/

The IDE will automatically configure:

PATH=<toolchain>/bin
LD_LIBRARY_PATH=<toolchain>/lib
