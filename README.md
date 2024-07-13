## Embedded code samples for Atmel AVR microcontrollers
### Cross-Platform Development with Visual Studio Code

### How to setup the environment?

#### Prerequisites
- [Visual Studio Code](https://code.visualstudio.com/)
- [avrdude](https://github.com/avrdudes/avrdude)
- [avr-gcc](https://gcc.gnu.org/wiki/avr-gcc)

### Installation Process
<details>
  <summary><img src="https://github.com/user-attachments/assets/6adedf3c-1d29-43f4-8e96-8c3d6cdcae11" width="3%" height="3%" /><b> Arch Linux</b></summary>

```bash
sudo pacman -S base-devel usbutils avrdude avr-gcc avr-libc  
git clone https://aur.archlinux.org/visual-studio-code-bin.git
cd visual-studio-code-bin
makepkg -si
```
  
</details>

<details>
  <summary><img src="https://github.com/user-attachments/assets/731b966d-2257-4276-9d8b-ac7f43758c4d" width="3%" height="3%" /><b> Ubuntu Linux</b></summary>

```bash
sudo apt update
sudo apt install gcc build-essential
sudo apt install gcc-avr binutils-avr avr-libc gdb-avr
sudo apt install libusb-dev avrdude
sudo apt install code
```
</details>

<details>
  <summary><img src="https://github.com/user-attachments/assets/7cf4fdb1-c479-407a-89a4-1a254f1301ec" width="3%" height="3%" /><b> Windows</b></summary>  
  <br>
  - Install <a href="https://winavr.sourceforge.net">WinAVR</a> for a Light-Weight Compiler<br>
  - Or install the full <a href="https://ww1.microchip.com/downloads/aemDocuments/documents/DEV/ProductDocuments/SoftwareTools/avr8-gnu-toolchain-3.7.0.1796-win32.any.x86_64.zip">AVR Toolchain</a><br>
  - Install <a href="https://code.visualstudio.com/Download">Visual Studio Code</a><br>
</details>


### Configure Visual Studio Code

<details>
  <summary><b>Install VS Code Extensions</b></summary><br>
  - Open <b>Extensions</b> in the left pane or press <b>Ctrl+Shift+X</b>b><br><br>
  - Search for <b>C/C++ Extension Pack</b> and click "Install"<br>
  <img src="https://github.com/user-attachments/assets/329c0eb9-de80-4733-9330-db12b8b6e119" width="50%" height="50%" /><br><br>
  - Search for <b>Makefile</b> Tools and click <b>Install</b><br> 
  <img src="https://github.com/user-attachments/assets/ab3f2da6-5baa-40f6-8655-79ee52b7e633" width="50%" height="50%" />
</details>

<details>
  <summary><b>Create New Project</b></summary><br>
  - Create an empty folder anywhere<br>
  - Open the empty folder ( Ctrl+O )<br>
  - Create an empty <b>C/C++ File</b> and a <b>Makefile</b> ( Right click -> New File )<br><br>
  <img src="https://github.com/user-attachments/assets/2a41e63a-a7a6-4da5-9505-1d13e64303cb" width="50%" height="50%" />
</details>

<details>
  <summary><b>Populate your Source File</b></summary><br>
  - Populate your <b>Source File</b><br><br>
  <img src="https://github.com/user-attachments/assets/2685af51-a058-40ae-85c2-d0153a6467cb" width="50%" height="50%" /><br>
  <b>Note:</b> Your header files will be red underlined.<br>This is an expected behavior.<br>To resolve this you must configure VS Code.<br><br>
  - Press <b>F1</b> and in the searchbox type <b>C/C++</b> <br>
  - Then select <b>C/C++: Edit Configurations (UI)</b><br><br>
  <img src="https://github.com/user-attachments/assets/7f502d4f-5255-4542-86d5-b2358820893c" width="50%" height="50%" /><br><br>
  - Set <b>Configuration Name</b> ( Linux or Win32 ...etc. )<br><br>
  <img src="https://github.com/user-attachments/assets/19126ef9-a53c-49a5-ab7c-c9e60c406fdd" width="50%" height="50%" /><br><br>


</details>

<br><br><br><br><br><br><br><br>
