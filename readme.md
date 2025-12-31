[EN](#en) / [FI](#fi)

# Meshtastic 2.7.22 for Heltec V2

This repository provides the compiled firmware for Meshtastic 2.7.22 for the Heltec V2 board, since the official Meshtastic Flasher tool currently only supports Heltec V3.

<a name="en"></a>

## 🚀 Flashing Instructions

### 🔧 1. Putting Heltec V2 into Programming Mode

1. Connect the Heltec V2 to your computer via USB.
2. Hold the **PRG** (Program) button on the board.
3. While holding **PRG**, press and release the **RST** (Reset) button.
4. Release the **PRG** button.
5. The device is now in bootloader mode and ready to be flashed.

### ✨ 2. Flashing with ESP Web Flasher

1. Go to [ESP Web Flasher](https://esptool.spacehuhn.com).
2. Click **Connect** and select your Heltec V2 device from the list.
3. Manually add each file and set the correct address:
    - `bootloader.bin` → `0x1000`
    - `partitions.bin` → `0x8000`
    - `firmware.bin` → `0x10000`
4. Click **Start** and wait for the process to finish.
5. Reboot the device once flashing is complete.

![Flashing addresses for Meshtastic on Heltec V2](img/adresses.png "ESP Web Flasher address setup")

***

<a name="fi"></a>

## 🚀 Laiteohjelmiston Asennusohjeet

### 🔧 1. Heltec V2:n Asettaminen Ohjelmointitilaan

1. Yhdistä Heltec V2 tietokoneeseesi USB-kaapelilla.
2. Pidä laitteen **PRG**-painiketta (Program) pohjassa.
3. Samalla kun pidät **PRG**-painiketta pohjassa, paina ja vapauta **RST**-painike (Reset).
4. Vapauta **PRG**-painike.
5. Laite on nyt lataustilassa ja valmis asennettavaksi.

### ✨ 2. Asennus ESP Web Flasherilla

1. Avaa [ESP Web Flasher](https://esptool.spacehuhn.com).
2. Napsauta **Connect** ja valitse Heltec V2 -laitteesi luettelosta.
3. Lisää jokainen tiedosto manuaalisesti ja aseta oikea osoite:
    - `bootloader.bin` → `0x1000`
    - `partitions.bin` → `0x8000`
    - `firmware.bin` → `0x10000`
4. Napsauta **Start** ja odota, että prosessi on valmis.
5. Käynnistä laite uudelleen, kun asennus on valmis.

![Meshtasticin flash-osoitteet Heltec V2:lle](img/adresses.png "ESP Web Flasher -osoitteiden asetus")
