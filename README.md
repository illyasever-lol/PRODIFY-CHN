# PRODIFY - The Nintendo Switch PRODINFO Editor

<div align="center">
  <img src="https://github.com/sthetix/PRODIFY/blob/main/prodify.jpg" alt="PRODIFY" width="400"/>
  <br>
  <br>
</div>

<div align="center">
  <img src="https://github.com/illyasever-lol/PRODIFY-CHN/blob/main/PRODIFYCHN1.5.jpg" alt="PRODIFY" width="400"/>
  <br>
  <br>
</div>

<div align="center">
  <img src="https://raw.githubusercontent.com/illyasever-lol/PRODIFY-CHN/refs/heads/main/nyx20460507_143159.bmp" alt="PRODIFY" width="400"/>
  <br>
  <br>
</div>

## 基于sthetix的PRODIFY和lsp199308的修改版本
v1.5
- 1、增加wlan、蓝牙mac地址读取，并基于新序列号生成、自动写入

v1.3
- 1、修复序列号区域马来版不正确添加序列号
- 2、增加NX-Wifi-Region-Changer的wifi区域信道修改功能
- 3、全部内容、提示、选项汉化

可通过sha256检测，修改后WIFI、蓝牙功能均可正常使用

                                       Have fun~


PRODIFY is a tool for editing decrypted `prodinfo` files on Nintendo Switch consoles. It lets users modify the serial number and adjust the body or bezel color. Primarily for banned consoles, it can also normalize serial and body color when using a donor NAND generated by `prodinfo_gen`.

## Features

- **Serial Number Editing**: Easily modify the console's serial number within the decrypted `prodinfo` file.
- **Body and Bezel Color Customization**: Adjust the color settings for the console's body and bezel, with real-time updates and CRC-16 checksum calculation to ensure integrity.
- **Normalization**: Normalize the serial number and body color when using a donor NAND, ensuring consistency.

## Prerequisites

Before using PRODIFY, ensure you have:

- **Operating System**: Windows 7 or higher.
- **Decrypted `prodinfo` File**: Ensure the `prodinfo` file is decrypted; encrypted files are not supported.

## Usage

1. **Launch PRODIFY**:
   - Double-click `prodify.exe` to start the application.

2. **Load `prodinfo` File**:
   - Click the "Load PRODINFO" button and select the decrypted `prodinfo` file you wish to edit.

3. **Edit Serial Number**:
   - The current serial number is displayed. Enter a new serial number if needed (14 characters max).

4. **Customize Colors**:
   - Modify the "Bezel Color" and "Main Color" by either entering a HEX color code directly or using the color picker. The tool automatically calculates and updates the CRC-16 checksum to ensure the integrity of the changes.

5. **Update `prodinfo` File**:
   - Click "Update PRODINFO" to save your changes. The tool will update the serial number, colors, and calculate the SHA-256 hash for the file.

## Important Notes

- **Intended Use**: PRODIFY is intended primarily for use on banned consoles. Modifying `prodinfo` files on active or online consoles may result in a ban.
- **Normalization**: When using a donor NAND generated with `prodinfo_gen`, PRODIFY can normalize the serial number and body color to match the console's original settings.
