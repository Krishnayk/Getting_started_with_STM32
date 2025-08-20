

# 🚀 Blink LED on STM32  

This repository demonstrates the basic **LED Blink project** on an **STM32 Nucleo-F401RE** board.  
> ⚠️ Note: The steps here are for **Nucleo-F401RE**. For other STM32 boards, pin mappings and setup may differ. Always check the board **schematic** and adjust accordingly.  

---

## 📌 Prerequisites  
Before starting, ensure you have:  
- [STM32CubeIDE](https://www.st.com/en/development-tools/stm32cubeide.html) installed  
- A supported STM32 development board (e.g., Nucleo-F401RE)  
- USB cable for board connection  

---

## 🛠️ Steps to Create the Project  

### 1. Open STM32CubeIDE  
- Create a new **workspace**.  
- Go to **File → New → STM32 Project**.  

![create project](https://github.com/user-attachments/assets/ef9aace1-abf5-4a92-bdf9-712e2496fd44)  

---

### 2. Board Selection  
- Select your board (e.g., Nucleo-F401RE).  
- Continue through the setup wizards (**Yes → Yes**) until you reach the CubeMX configuration screen.  

![board setup](https://github.com/user-attachments/assets/5d7d103b-a752-4800-965c-e840022fd67e)  

---

### 3. Enable LED Pin  
- Check whether the onboard LED pin is enabled (**green**).  
- If not, enable it manually.  

![pin config](https://github.com/user-attachments/assets/31d74560-a599-4fc3-94da-64f5d75d22d9)  

---

### 4. Write Blink Code  
- Use the `main.c` file and add your **Blink LED code** inside the `while(1)` loop.  

![blink code](https://github.com/user-attachments/assets/4ce6a942-d082-4038-8f10-b8f9c9268f88)  

---

### 5. Build & Run  
- In **Project Explorer**, right-click your project → **Build Project**.  
- After a successful build:  
  - Go to the **Run Configurations** menu.  
  - Select **1 STM32 C/C++ Application**.  

![build run](https://github.com/user-attachments/assets/98e81708-dc0f-4ab0-9fbf-5d4b6e6c09e4)  

---

## 🎉 Result  
If everything is configured correctly, the **onboard LED will start blinking**!  

---

## 🔧 Troubleshooting  
- If the project doesn’t build, check:  
  - Correct board is selected in CubeMX.  
  - LED GPIO pin is configured as **Output**.  
- If flashing fails:  
  - Ensure the board is properly connected via USB.  
  - Try pressing the **RESET button** before running again.  

---


---

## 📖 References  
- [STM32CubeIDE Official Documentation](https://www.st.com/en/development-tools/stm32cubeide.html)  
- [Nucleo-F401RE Board User Manual](https://www.st.com/resource/en/user_manual/dm00105823-stm32-nucleo64-boards-mb1136-stmicroelectronics.pdf)  

