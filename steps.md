Comppling the code using the cross compiler.

arm-none-eabi-gcc -mcpu=cortex-m7 main.c -c

Viewing the contents on the file generated.

arm-none-eabi-objdump -h main.o


Sections:
Idx Name          Size      VMA       LMA       File off  Algn
  0 .text         00000050  00000000  00000000  00000034  2**2
                  CONTENTS, ALLOC, LOAD, RELOC, READONLY, CODE
  1 .data         00000000  00000000  00000000  00000084  2**0
                  CONTENTS, ALLOC, LOAD, DATA
  2 .bss          00000000  00000000  00000000  00000084  2**0
                  ALLOC
  3 .vectors      000001ac  00000000  00000000  00000084  2**2
                  CONTENTS, ALLOC, LOAD, RELOC, READONLY, DATA
  4 .comment      00000046  00000000  00000000  00000230  2**0
                  CONTENTS, READONLY
  5 .ARM.attributes 0000002e  00000000  00000000  00000276  2**0
                  CONTENTS, READONLY


The VMA and LMA are 0 as we have not linked the code yet.

