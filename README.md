# SUZUNO32RV - CH32V203 Prototyping board

<img src="https://github.com/verylowfreq/board_suzuno32rv/assets/60875431/f60dd19a-8617-4681-9ba2-af1d0fa96077" width="480">

**SUZUNO32RV** is a MCU prototyping board with **RISC-V MCU CH32V203C8T6** (LQFP 48pin) in the famous "UNO"-shape board.

**CH32V** series is a microprocessor chip of RISC-V by WCH. The chip has RISC-V 32bit CPU core and STM32-like peripherals. The price is cheap but powerful.

SUZUNO32RV has **Type-C** port (as USB device; USBD) and **Type-A** port (as USB Host, and Device with additional cable; USBFS). So you can develop USB device and/or USB Host role program.

**SUZUNO32RV**は**RISC-Vチップ "CH32V"** を搭載した、UNO形状のマイコンボードです。

**CH32V**はWCHによるRISC-Vマイコンです。32ビットRISC-Vコアと、STM32のペリフェラルが実装されていて、安価ながらもパワフルです。

SUZUNO32RVはデバイスとしての**Type-Cポート** (USBD) と、ホストとしての**Type-Aポート**（USBFS; あるいは追加のケーブルを準備してデバイスとして）が実装されているので、USBデバイス・ホスト機能の開発もできます。

## Specs / 仕様

 - CH32V203C8T6
   - RISC-V CPU 144MHz, ROM 64KB, RAM 20KB
 - Digital: 25pins
 - Analog: 6 + more pins
 - USB connector: Type-C, Type-A
 - Program download method: WCH LinkE cable (WCH LinkUtility), USB download (WCHISPStudio)
 - Power supply: Type-C (5V), Pin headers (5V or 3.3V)
 - Crystal: 8MHz (NOTE: CH32V203C8T6 can also run without external crystal)
 - 

## Sample code / サンプルコード

### Act as USB keyboard device / USBキーボードとして振舞う

https://github.com/verylowfreq/arduino_ch32v203_usbdevice_keyboard

### Act as USB Host and read the key input from USB keyboard / USBホストとして、USBキーボードの入力を読み取る

https://github.com/verylowfreq/arduino_ch32v203_usbdevice_keyboard

### Load JPEG image files from USB stick and show on SPI LCD / USBメモリからJPEGファイルを読み込み、SPI接続の液晶画面へ表示する

https://github.com/verylowfreq/pio_ch32v203_usbms_imageviewer

## Resources / 資料

 - Short guide / 簡易説明書
   - (To be uploaded)
 - Schematic / 回路
   - (To be uploaded/アップロード予定)

## Additional note / 追記

I also made "Suzuduino UNO" as former board. This board uses CH32V203K8T6 (LQFP 32pin) and good for hand soldering.

"Suzuduino UNO" というボードも製作・頒布しています。これは手ハンダ実装に適した基板で、CH32V203K8T6 (LQFP 32pin) を採用したものです。

https://github.com/verylowfreq/suzuduino-uno-v1/
