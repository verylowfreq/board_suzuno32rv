# Suzuno32RV - CH32V203 Prototyping board

<img width="400" src="images/image_adsz32rv_1.jpg">

**チュートリアル・開発ガイドはこちら → [https://verylowfreq.github.io/suzunodoc/](https://verylowfreq.github.io/suzunodoc/)**


**Suzuno32RV** は **RISC-Vチップ "CH32V"** を搭載した、UNO形状のマイコンボードです。

**CH32V** はWCHによるRISC-Vマイコンです。32ビットRISC-Vコアと、STM32のペリフェラルが実装されていて、小さいながらもパワフルなチップです。

[WCH 32-bit Enhanced Low-Power RISC-V MCU – CH32V203](https://www.wch-ic.com/products/CH32V203.html)

Suzuno32RVはデバイスとしての**Type-Cポート** (USBD) と、ホストとしての**Type-Aポート**（USBFS/USBOTG_FS）が実装されているので、USBデバイス・ホスト機能の開発もできます。

<img width="400" src="images/image_adsz32rv_2.jpg">

**Suzuno32RV** is a MCU prototyping board with **RISC-V MCU CH32V203C8T6** (LQFP 48pin) in the famous "UNO"-shape board. **CH32V** series is a microprocessor chip of RISC-V by WCH. The chip has RISC-V 32bit CPU core and STM32-like peripherals. The price is cheap but powerful. This board has **Type-C** port (as USB device; USBD) and **Type-A** port (as USB Host; USBFS). So you can develop USB device and/or USB Host program.


## 仕様 / Specs

 - CH32V203C8T6
   - RISC-V CPU 144MHz, ROM 64KB, RAM 20KB
 - Digital: 25pins
 - Analog: 6 + more pins
 - USB connector: Type-C, Type-A
 - Program download method: WCH LinkE cable (WCH LinkUtility), USB download (WCHISPStudio)
 - Power supply: Type-C (5V), Pin headers (5V or 3.3V)
 - Crystal: 8MHz (NOTE: CH32V203C8T6 can also run without external crystal)


## サンプルコード / Sample code

### Act as USB keyboard device / USBキーボードとして振舞う

https://github.com/verylowfreq/arduino_ch32v203_usbdevice_keyboard

### Act as USB Host and read the key input from USB keyboard / USBホストとして、USBキーボードの入力を読み取る

https://github.com/verylowfreq/arduino_ch32v203_usbdevice_keyboard

### Load JPEG image files from USB stick and show on SPI LCD / USBメモリからJPEGファイルを読み込み、SPI接続の液晶画面へ表示する

https://github.com/verylowfreq/pio_ch32v203_usbms_imageviewer


## Resources / 資料

ビット・トレード・ワン取り扱いの Suzuno32RV (ADSZ32RV) の資料はこちらです。

 - ADSZ32RV 回路図 / Schematic for ADSZ32RV
   - [schematic_suzuno32rv_v1_bto.pdf](https://github.com/verylowfreq/board_suzuno32rv/blob/main/schematic_suzuno32rv_v1_bto.pdf)


以下は限定的に配布された先行版基板の資料です。

 - 簡易説明書 / Short guide
   - [suzuno32rv_shortguide_1.pdf](https://github.com/verylowfreq/board_suzuno32rv/blob/main/suzuno32rv_shortguide_1.pdf)
 - 回路図 / Schematic
   - [schematic_suzuno32rv_v1.pdf](https://github.com/verylowfreq/board_suzuno32rv/blob/main/schematic_suzuno32rv_v1.pdf)


## 関連する基板 / Related-board

わたしは "Suzuduino UNO" というボードも製作・頒布しています。これは手ハンダ実装に適した基板で、CH32V203K8T6 (LQFP 32pin) を採用したものです。

I also made "Suzuduino UNO" as former board. This board uses CH32V203K8T6 (LQFP 32pin) and good for hand soldering.

https://github.com/verylowfreq/suzuduino-uno-v1/
