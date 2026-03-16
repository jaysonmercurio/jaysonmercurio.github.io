---
name: FPGA-Based Brick Breakout Game
tools: [Vitis Design Suite, Verilog, C]
image: 
description: A project implemented in both PL and PS 
---

## FPGA-Based Brick Breakout Game

This project was made during my Advanced Computer Design graduate course during the Spring 2025 semester. My groupmates and I set out to create a brickout game from scratch using the [Digilent Zybo Z7 Dev Board](https://digilent.com/shop/zybo-z7-zynq-7000-arm-fpga-soc-development-board/). The project was split into two parts: *programmable logic* and the *processing system*.

![Image of the game screen](..assets/projects/brick_breakout)

---

### Goal

Create a brick breakout game with joystick functionality. Upon boot up, the ball will start on the paddle and will be released when a button is pressed. Added goals woud be to add a running score and difficulty setting.

---

### Components
#### Programmable Logic
Programmable logic (PL) is what configures the digital design of the FPGA chip on the board. For the implementation of this project, we created the following in PL:
- HDMI Output
- Block RAM Interface
- SPI Joystick communication

#### Processing System
The processing system (PS) uses the ARM-Cortex-A9 on this FPGA dev board. This portion strictly uses software rather than bare-metal. The following were implemented within PS:
- Frame Rendering
- Game Logic
- Framebuffer Memory Access
- Joystick Polling


<p class="text-center">
{% include elements/button.html link="https://github.com/jaysonmercurio" text="Github" %}
</p>