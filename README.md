## Embedded code samples for Atmel AVR microcontrollers

### How to setup the environment?

### Install Prerequisites
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
  <img src="https://github.com/user-attachments/assets/b26bf4c2-954d-4b55-ba59-01909dfc951e" width="50%" height="50%" /><br>
  <b>Note:</b> Your header files will be red underlined.<br>This is an expected behavior.<br>To resolve this you must configure VS Code.<br><br>
  - Press <b>F1</b> and in the searchbox type <b>C/C++</b> <br>
  - Then select <b>C/C++: Edit Configurations (UI)</b><br><br>
  <img src="https://github.com/user-attachments/assets/7f502d4f-5255-4542-86d5-b2358820893c" width="50%" height="50%" /><br><br>
  - Set <b>Configuration Name</b> ( Linux or Win32 ...etc. )<br><br>
  <img src="https://github.com/user-attachments/assets/19126ef9-a53c-49a5-ab7c-c9e60c406fdd" width="50%" height="50%" /><br><br>
  - Locate <b>avr-gcc</b> on your Machine<br>
  - Edit the <b>Compiler Path</b><br><br>
  <img src="https://github.com/user-attachments/assets/239dcd6b-3a0d-4d27-b38d-5011e5343e79" width="50%" height="50%" /><br>
  <b>Note:</b> you will might need to use quotation marks<br>for the <b>Compiler Path</b> if there are empty spaces in it<br><br>
  - Select <b>IntelliSense mode</b><br><br>
  <img src="https://github.com/user-attachments/assets/68aad793-1107-4302-ae71-535d2b2fbf81" width="50%" height="50%" /><br>
  <b>Note:</b> the <b>gcc-x86 (legacy)</b> worked fine for me<br>but make sure to test your platform specific <b>IntelliSense mode</b><br>( i.e. <b>linux-gcc-x86</b> or <b>windows-gcc-x86</b> )<br><br>
  - Save the Configuration and check your Source Code<br><br>
  <img src="https://github.com/user-attachments/assets/b7277027-434c-4d58-a298-9ecf65dd2b56" width="50%" height="50%" /><br>
  <b>Note:</b> header file names are not underlined anymore
  <br>
  however methods and some definitions are.
  <br>
  This is an expected behavior.
  <br>
  You need to select the proper Microcontroller!
  <br>
  <br>
  - Press and hold <b>Ctrl</b> and click on the <b>avr/io.h</b> header file in your source
  <br>
  - This will bring you to <b>io.h</b> where you can look up your <b>Microcontroller definition
  </b>
  <br>
  - Copy your Microcontroller definition<br><br>
  <img src="https://github.com/user-attachments/assets/2ac5d640-4ba3-4c8f-985a-fbb932e01a67" width="50%" height="50%" />
  <br>
  <br>
  - Go back to the <b>C/C++ Configurations</b> and edit the <b>Defines</b> section<br>
  - Paste your <b>Microcontroller Definition</b> here and save it<br><br>
  <img src="https://github.com/user-attachments/assets/11e48bb2-45b7-4a23-b5bf-4705711a1ae3" width="50%" height="50%" />
  <br>
  <br>
  - Check if IntelliSense and Smart Hints work<br>
  - If nothing is underlined and all functionalities work you are <b>done 📗
  </b>
  <br>
<img src="https://github.com/user-attachments/assets/eb631695-f2b1-4d10-a238-acb5003bc2ba" width="50%" height="50%" />
</details>

<details>
  <summary><b>Populate your Makefile</b></summary>
  <br>
  <br>
  
  Copy the name of your <b>Programmer Hardware</b>
  <br>
  
  ```bash
  avrdude -c ?
  ```
  <img src="https://github.com/user-attachments/assets/7758c9df-86cf-4bcb-bc04-dc7f8eb41489" width="50%" height="50%" />
  <br>
  <br>
  <br>
  Copy the name of your <b>Microcontroller</b>
  <br>
  
  ```bash
  avrdude -p ?
  ```
  <img src="https://github.com/user-attachments/assets/9ea12bd7-6f81-4923-87a3-407280066c9f" width="20%" height="20%" />
  <br>
  <br>
  <br>
  Construct the terminal command to <b>Flash the HEX File</b>
  <br>
  
  ```bash
  avrdude -c stk500v2 -p m328p -U main.hex
  ```

  <br>
  <br>
  Copy the name of your MCU for the Compiler
  
  ```bash
  avr-gcc --target-help
  ```

  <img src="https://github.com/user-attachments/assets/6e4febad-8233-4e10-aa59-ae4a957d1683" width="50%" height="50%" />
  <br>
  <br>
  <br>
  Check the <b>Crystal Oscillator Frequency</b>
  <br>
  For example if the frequency is <b>16 Mhz</b> the argument will be this:

  
  ```bash
  16000000UL
  ```

  <br>
  <br>

  Construct the terminal command to <b>Compile the HEX File</b>
  <br>
  <i>avr-gcc&emsp;<source_file>&emsp;<mcu_type>&emsp;<clock_frequency>&emsp;<output_file></i>
  <br>
  
  ```bash
  avr-gcc main.c -mmcu=atmega328p -DF_CPU=16000000UL -0s -o main.hex
  ```
  <b>Note:</b> the <b>-0s</b> argument will minimize the output file size


  Populate your <b>Makefile</b> to Compile and Flash
  <br>
  <img src="https://github.com/user-attachments/assets/4aeb44db-a554-4e8d-a15c-a18e3aed78f8" width="50%" height="50%" />

  
  
</details>
<br><br><br><br><br><br><br><br>
