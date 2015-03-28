# ADC Preamp
Kicad schematic for opamp based preamp circuit used with my adc_interface project

I designed this circuit to use with interfacing with my De0 Nano's onboard analog to digital circuit. The cicuit has the following features
   * 0-50 x Gain
   * Bandwidth (didnt really calculate, but designed for use with audio)
   * Amp requires 12-20V DC supply
   * Vout level protection circuit requires 3.3V DC supply

## Setup with De0 Nano

   * 12V rail is provided by 8 1.5V batteries
   * 3.3V rail to protection clamping diodes connect to:
    * GPIO-1 - pin 29 (VCC3P3) 
    * GPIO-1 - pin 30 (GND)
   * Vout connected to:
    * GPIO-3 - pin 24 (Analog_In0)
