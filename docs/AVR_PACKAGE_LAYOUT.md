# AVR Package Layout

The AVR toolchain package must extract into:

avr/
├── bin/
├── lib/
├── libexec/
├── share/
└── manifest.json

## Folder Description

### bin/

Contains executable tools:

- avr-gcc
- avr-g++
- avr-ar
- avr-as
- avr-ld
- avr-objcopy
- avr-objdump
- avr-size
- avr-nm
- avr-strip
- avrdude

### lib/

Contains runtime libraries required by the tools.

### libexec/

Contains GCC internal executables.

Example:

- cc1
- cc1plus
- collect2

### share/

Contains:

- avr device specifications
- avrdude.conf
- documentation

### manifest.json

Contains package metadata.

Example:

{
  "toolchain": "avr",
  "version": "1.0.0",
  "target": "atmega328p",
  "architecture": "aarch64-linux-android"
}
