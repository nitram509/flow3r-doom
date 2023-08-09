| Supported Targets | ESP32-S3/flow3r
| ----------------- | --------------- |

# flow3r Hello World Example

Starts a FreeRTOS task to turn on all LEDs

## How to use example

- Install ESP IDF 5.1 (ideally with FPU patch backported, see flow3r docs)
- Run `git submodule update`
- Run `idf.py build` to build
- Run `idf.py app-flash` to flash the app without touching flow3r bootloader and recovery
- Copy `build/Go_Green.bin` to flow3r's internal flash or SD card to flash via recovery mode

## Example folder contents

The project **go_green** contains one source file in C language [go_green_main.c](main/go_green_main.c). The file is located in folder [main](main).

ESP-IDF projects are built using CMake. The project build configuration is contained in `CMakeLists.txt` files that provide set of directives and instructions describing the project's source files and targets (executable, library, or both).

Below is short explanation of remaining files in the project folder.

```
├── CMakeLists.txt
├── main
│   ├── CMakeLists.txt
│   └── go_green_main.c
└── README.md                  This is the file you are currently reading
```

For more information on structure and contents of ESP-IDF projects, please refer to Section [Build System](https://docs.espressif.com/projects/esp-idf/en/latest/esp32/api-guides/build-system.html) of the ESP-IDF Programming Guide.

## Troubleshooting

* Program upload failure

    * Hardware connection is not correct: run `idf.py -p PORT monitor`, and reboot your board to see if there are any output logs.

## Technical support and feedback

Please use the following feedback channels:

* For technical queries, go to the [esp32.com](https://esp32.com/) forum
* For a feature request or bug report, create a [GitHub issue](https://github.com/espressif/esp-idf/issues)

We will get back to you as soon as possible.
