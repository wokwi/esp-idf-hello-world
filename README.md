# Precompiled ESP32 IDF Hello World

This is a precompiled version of the ESP32 IDF Hello World example. You can run it with Wokwi, either using the [Wokwi for VS Code Extension](https://docs.wokwi.com/vscode/getting-started) or through the command line using [wokwi-cli](https://github.com/wokwi/wokwi-cli).

## Running with VS Code

1. Install the [Wokwi for VS Code Extension](https://marketplace.visualstudio.com/items?itemName=wokwi.wokwi-vscode)
2. Open this folder in VS Code
3. Press "F1" and choose "Wokwi: Start Simulator"

## Running with wokwi-cli

1. Install [wokwi-cli](https://github.com/wokwi/wokwi-cli)
2. Run `wokwi-cli <path-to-this-folder>`

## Recompiling

To recompile this program, install esp-idf and then run:

```
cd $IDF_PATH/examples/get-started/hello_world
idf.py set-target esp32
idf.py build
```

Then copy `build/hello_world.bin`, `build/bootloader/bootloader.bin`, `build/partition_table/partition-table.bin` and `build/hello_world.elf` to the `bin` directory inside this repo.
