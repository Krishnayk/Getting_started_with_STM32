# 🔌 Serial Communication on STM32 (USART)  

This guide explains how to set up and use **USART Serial Communication** in **STM32CubeIDE** with an STM32 Nucleo board.  

---

## 📌 Steps  

### 1. Create a New STM32 Project  
- Follow the same process as in **Blink LED** example:  
  - Open STM32CubeIDE → **New → STM32 Project**.  
  - Select your STM32 board (e.g., Nucleo-F401RE).  
  - Complete general setup.  

---

### 2. Configure USART Pins  
- In **CubeMX Configuration**, enable **USART2 TX** and **USART2 RX** pins.  
- Make sure both TX and RX are properly assigned and enabled.  

![usart config](https://github.com/user-attachments/assets/d7dcf283-ea84-4c42-9864-a85acfc94e65)  

⚠️ Important: Ensure your STM32 chip supports **USART2** (TX & RX).  

---

### 3. Code Setup (`main.c`)  

#### a) Include Required Header  
Add the `string.h` library to use serial functions.  

![include string.h](https://github.com/user-attachments/assets/1e968ba4-8faf-4b7b-85ca-1aef391fdfd1)  

#### b) Check & Include HAL USART Functions  
Verify that the USART initialization lines are present. If not, include them.  

![usart init](https://github.com/user-attachments/assets/9f5ea8c5-1388-4c32-9e88-7763a62dd14d)  
![hal usart](https://github.com/user-attachments/assets/caaf8790-ba70-4662-8da7-0e8a48ee3e2b)  

The **red box** highlights the key **text declaration line** for sending data.  
Also add the 
"HAL_UART_Transmit(&huart2, (const uint8_t*) msg, strlen(msg), TIMEOUT);"

---

### 4. Build & Run the Project  

- Build the project (`Project Explorer → Right-click → Build Project`).  
- After flashing, go to **Serial Console** in STM32CubeIDE.  

![serial console](https://github.com/user-attachments/assets/52550796-061c-4b20-8617-048f69edb5c4)  

---

### 5. Configure Serial Console  

- When prompted, select **UTF-8 encoding**.  

![utf8 encoding](https://github.com/user-attachments/assets/dbd4d3dd-eee7-403b-b64b-d056d0f334a9)  

- Use **Step Over (F6)** while debugging to execute the code line by line.  
- At the `hal_UART_Transmit` line, you will see the output appear in the **Serial Console**.  

![serial output](https://github.com/user-attachments/assets/ce0b2bf6-ecb1-4506-b3fa-bc0c7b797fdc)  

---

## 🎉 Result  

- Successfully send and view text/data over **USART Serial** inside STM32CubeIDE.  
- The output will appear in the **Console Window** during program execution.  

---

## 📖 References  

- [STM32CubeIDE Documentation](https://www.st.com/en/development-tools/stm32cubeide.html)  
- [USART Communication on STM32 (ST Wiki)](https://wiki.st.com/stm32mcu/wiki/Serial_peripheral_interface_(SPI)_overview)  
