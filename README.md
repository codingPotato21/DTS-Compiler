# DTS Preprocessor and Compiler Script

This script preprocesses Device Tree Source (DTS) files using the C preprocessor (`cpp`) and compiles them into Device Tree Blob (DTB) or Device Tree Overlay (DTBO) files using `dtc`. It provides a convenient way to preprocess and compile DTS files for embedded systems development, particularly targeting the ARM architecture.

## Usage

The script accepts the following command-line arguments:

```
-i, --input      Input DTS file
-o, --output     Output format (dtb, dts, or dtbo)
-h, --help       Display help menu
```

### Examples

1. Preprocess a DTS file and generate a DTB file:
   ```
   ./makedtb -i input_filename.dts -o dtb
   ```

2. Preprocess a DTS file and generate a DTBO file:
   ```
   ./makedtb -i input_filename.dts -o dtbo
   ```

3. Preprocess a DTS file and keep it as DTS:
   ```
   ./makedtb -i input_filename.dts -o dts
   ```

## Requirements
Make sure to have these installed on your system before running the script. Google is your friend to know how to get them for your distribution.
- `arm-none-eabi-cpp`: C preprocessor for the ARM architecture.
- `dtc`: Device Tree Compiler.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

