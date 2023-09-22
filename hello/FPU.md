The STM32F767ZI microcontroller from STMicroelectronics is based on the ARM Cortex-M7 core, and it includes a Floating-Point Unit (FPU). The FPU in the STM32F767ZI is an ARMv7-M FPU, specifically designed for the ARM Cortex-M series of microcontrollers.

The ARMv7-M FPU supports single-precision (32-bit) and double-precision (64-bit) floating-point operations, and it complies with the IEEE 754 standard for floating-point arithmetic. This FPU provides hardware acceleration for floating-point arithmetic operations, making it suitable for applications that require fast and efficient floating-point calculations.

To use the FPU in the STM32F767ZI with the GCC compiler, you typically specify the appropriate `-mfpu` flag when compiling your code. You would use an argument like `-mfpu=fpv5-d16`, where `fpv5-d16` indicates the specific FPU configuration of the Cortex-M7 core used in the STM32F767ZI.

Keep in mind that the exact FPU configuration may vary slightly depending on the microcontroller's specific revision or the STM32F7 series variant, so it's a good practice to refer to the reference manual or datasheet for your specific device to confirm the FPU configuration details.