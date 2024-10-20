# ARM_CORTEX_M0_SoC

In this project, I designed and developed a simple System on Chip (SoC) using the ARM Cortex M0 processor, interfaced with a Timer and GPIO/LED peripherals. The design was implemented and synthesized on the ARTY A7 FPGA kit, demonstrating basic functionality like interrupt handling and controlling the LEDs on the board.

### Working:

1. The Timer counts down from ‘0F’ to ‘00’.

2. When it hits ‘00’, an interrupt is triggered, and the system clears the interrupt using a specific clear register.

3. When the interrupt happens, the LEDs on the FPGA are set to display the value ‘FF’, turning all the LEDs on.

4. After a short delay, the LEDs are cleared, turning them off again

### Key Features:

1. ARM Cortex M0 Processor: The core of the SoC, handling all the processing and communication with the peripherals.

2. Timer Peripheral: A basic countdown timer that generates an interrupt when it reaches zero.

3. GPIO/LED Peripheral: Controls the FPGA board’s LEDs, making them light up when the timer interrupt is triggered.

4. Interrupt Handling: The SoC efficiently handles the timer interrupt and triggers LED behavior in response.

This project is a basic example of how to build a custom SoC using an ARM Cortex M0 processor, interfacing it with peripherals like timers and LEDs. It showcases how to handle interrupts and control outputs like LEDs in real-time
