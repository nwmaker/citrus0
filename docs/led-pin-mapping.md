# LED and GPIO pin mapping

There are 19 LEDs driven by GPIO directly. When the GPIO is low, the LED is turned on. 

The numbering of LED starts from the position of hour 1 clockwise. Then minute 1 to 32. And the center of second at last.

In SAMD conventions, The GPIO pins are grouped in pin group. Group 0 consists of the PA pins. Each pin group has its own Port registers. Below is the mask used for each GPIO (LED).

```
const uint32_t cLedMask0 = (1UL<<27);
const uint32_t cLedMask1 = (1UL<<1);
const uint32_t cLedMask2 = (1UL<<2);
const uint32_t cLedMask3 = (1UL<<3);
const uint32_t cLedMask4 = (1UL<<5);
const uint32_t cLedMask5 = (1UL<<6);
const uint32_t cLedMask6 = (1UL<<14);
const uint32_t cLedMask7 = (1UL<<15);
const uint32_t cLedMask8 = (1UL<<17);
const uint32_t cLedMask9 = (1UL<<18);
const uint32_t cLedMask10 = (1UL<<19);
const uint32_t cLedMask11 = (1UL<<23);
const uint32_t cLedMask12 = (1UL<<0);
const uint32_t cLedMask13 = (1UL<<4);
const uint32_t cLedMask14 = (1UL<<7);
const uint32_t cLedMask15 = (1UL<<16);
const uint32_t cLedMask16 = (1UL<<22);
const uint32_t cLedMask17 = (1UL<<28);
const uint32_t cLedMask18 = (1UL<<25);
```

