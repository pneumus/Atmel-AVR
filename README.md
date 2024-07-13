## Embedded code samples for Atmel AVR microcontrollers
### Cross-Platform Development with Visual Studio Code

### How to setup the environment?

#### Prerequisites
- [Visual Studio Code](https://code.visualstudio.com/)
- [avrdude](https://github.com/avrdudes/avrdude)
- [avr-gcc](https://gcc.gnu.org/wiki/avr-gcc)

##### Installation Process
<details>
  <summary><img src="https://github.com/user-attachments/assets/6adedf3c-1d29-43f4-8e96-8c3d6cdcae11" width="3%" height="3%" />
Arch Linux</summary>

```bash
sudo pacman -S base-devel usbutils avrdude avr-gcc avr-libc  
git clone https://aur.archlinux.org/visual-studio-code-bin.git
cd visual-studio-code-bin
makepkg -si
```
  
</details>
<details>
  <summary><img src="https://github.com/user-attachments/assets/731b966d-2257-4276-9d8b-ac7f43758c4d" width="3%" height="3%" />
Ubuntu Linux</summary>

```bash
sudo apt update
sudo apt install gcc build-essential
sudo apt install gcc-avr binutils-avr avr-libc gdb-avr
sudo apt install libusb-dev avrdude
sudo apt install code
```

</details>
<details>
  <summary><img src="https://github.com/user-attachments/assets/7cf4fdb1-c479-407a-89a4-1a254f1301ec" width="3%" height="3%" />
Windows</summary>

- Install [WinAVR](https://winavr.sourceforge.net/) for a Ligth-Weight Compiler
- Or install the full [AVR Toolchain](https://ww1.microchip.com/downloads/aemDocuments/documents/DEV/ProductDocuments/SoftwareTools/avr8-gnu-toolchain-3.7.0.1796-win32.any.x86_64.zip)
- Install [Visual Studio Code](https://code.visualstudio.com/Download)
  
</details>


#### Configure Visual Studio Code
<details>
  <summary>Install C/C++ Extension Pack</summary>  
  - Open "Extensions" in the left pane or press Ctrl+Shift+X<br>
  - Search for "C/C++ Extension Pack"<br>   
  <img src="https://github.com/user-attachments/assets/6f6e1ffc-b966-4313-8e2b-5fa0b5422b17" width="50%" height="50%" />  
</details>
