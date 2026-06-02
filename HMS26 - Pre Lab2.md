---
title: "Prelaboratorio 2 - Tarjetas IoT"
layout: post
date: 2026-06-02
categories: [IoT, Hardware, Microcontroladores]
---

## 📑 Resumen de la investigación

### Raspberry Pi 3B+
- **Procesador:** Broadcom BCM2837, quad-core ARM Cortex-A53 a 1.2 GHz (RISC).  
- **GPIO:** 40 pines, 26 de propósito general (SPI, I²C, UART, PWM).  
- **Librerías:**  
  - Python: `RPi.GPIO`, `gpiozero`, `pigpio`.  
  - C/C++: `wiringPi`, `bcm2835`.  

### Raspberry Pi Pico W
- **Procesador:** RP2040, dual-core ARM Cortex-M0+ a 133 MHz (RISC).  
- **GPIO:** 26 pines (I²C, SPI, UART, PWM, ADC).  
- **Librerías:**  
  - Python: MicroPython (`machine`).  
  - C/C++: Pico SDK.  

### Arduino UNO R4 WiFi
- **Procesador:** Renesas RA4M1, ARM Cortex-M4 a 48 MHz (RISC).  
- **GPIO:** 14 digitales (6 PWM), 6 analógicas.  
- **Librerías:**  
  - Python: `pyserial` (comunicación USB/serial).  
  - C/C++: Arduino Core (`digitalWrite`, `digitalRead`, `pinMode`).  

### Arduino Nano ESP32
- **Procesador:** ESP32-S3, dual-core Xtensa LX7 de 32 bits (RISC).  
- **GPIO:** ~34 pines configurables (PWM, ADC, DAC, I²C, SPI, UART).  
- **Librerías:**  
  - Python: MicroPython (`machine`).  
  - C/C++: ESP-IDF, Arduino Core para ESP32.  

---

## 📊 Comparación rápida

| Tarjeta              | Procesador                | Tipo | GPIO disponibles | Librerías Python | Librerías C/C++ |
|----------------------|---------------------------|------|-----------------|------------------|-----------------|
| **Raspberry Pi 3B+** | ARM Cortex-A53 (1.2 GHz)  | RISC | 26 GPIO         | RPi.GPIO, gpiozero, pigpio | wiringPi, bcm2835 |
| **Raspberry Pi Pico W** | ARM Cortex-M0+ (133 MHz) | RISC | 26 GPIO         | MicroPython (`machine`) | Pico SDK |
| **Arduino UNO R4 WiFi** | ARM Cortex-M4 (48 MHz)   | RISC | 14 digitales, 6 analógicas | pyserial | Arduino Core |
| **Arduino Nano ESP32** | Xtensa LX7 dual-core (32-bit) | RISC | ~34 GPIO        | MicroPython | ESP-IDF, Arduino Core |

---

## ✅ Conclusiones
- Todas las tarjetas usan **arquitecturas RISC**, optimizadas para eficiencia y bajo consumo.  
- **Raspberry Pi 3B+** es potente y corre Linux, ideal para proyectos complejos.  
- **Raspberry Pi Pico W** es económico y sencillo, con Wi-Fi integrado.  
- **Arduino UNO R4 WiFi** moderniza la clásica UNO con ARM Cortex-M4 y conectividad inalámbrica.  
- **Arduino Nano ESP32** combina el ecosistema Arduino con la potencia del ESP32-S3.  
- En Python predominan **MicroPython** y `RPi.GPIO`; en C/C++ los SDK oficiales y Arduino Core son los más usados.  

---
