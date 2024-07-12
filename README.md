## Embedded code samples for Atmel AVR microcontrollers
### Cross-Platform Development with Visual Studio Code

### How to setup the environment?

#### Prerequisites
- Install [Visual Studio Code](https://code.visualstudio.com/)
- Install [avrdude](https://github.com/avrdudes/avrdude)
- Install avr-gcc

##### Installation Process
<details>
  <summary>Arch Linux</summary>

```bash
sudo pacman -S avrdude avr-gcc avr-libc
git clone https://aur.archlinux.org/visual-studio-code-bin.git
cd visual-studio-code-bin
makepkg -si
```
  
</details>
<details>
  <summary>Ubuntu Linux</summary>

```bash
sudo apt-get update
sudo apt-get install gcc-avr binutils-avr avr-libc gdb-avr avrdude
sudo apt-get install avrdude
sudo apt install code
```

</details>
<details>
  <summary>Windows</summary>

- Install the [AVR Toolchain](https://ww1.microchip.com/downloads/aemDocuments/documents/DEV/ProductDocuments/SoftwareTools/avr8-gnu-toolchain-3.7.0.1796-win32.any.x86_64.zip) from Microchip
- Install [Visual Studio Code](https://code.visualstudio.com/Download)
  
</details>


#### Configure Visual Studio Code
- Install C/C++ Extension Pack for VS Code
<img src="https://github.com/user-attachments/assets/6f6e1ffc-b966-4313-8e2b-5fa0b5422b17" width="50%" height="50%" />  
- 
