# UARTC

FT232RL-based UART to USB Type-C adapter with support of 5V/3V3/2V5/1V8

[![board front mini](https://raw.githubusercontent.com/streamx3/uartc/master/images/UARTC-revA01-front-mini.png)](https://raw.githubusercontent.com/streamx3/uartc/master/images/UARTC-revA01-front.png)
[![board back mini](https://raw.githubusercontent.com/streamx3/uartc/master/images/UARTC-revA01-back-mini.png)](https://raw.githubusercontent.com/streamx3/uartc/master/images/UARTC-revA01-back.png)

This is an advanced tool for rare usecases. It might come in handy if your scope includes:

- Low voltage targets

- Targets, that expect power to be supplied

- Targets with altering voltage, like battery-powered systems that discharge


## INSTRUCTION

Either use **ONE** voltage on switch or use none and connect VIO to board's voltage source. Doing otherwise will most like damage a board.


## Thing you can do with this board

- Solder 2.54mm header or XH-2.54-6P-SMD compatible connector like this: [CAX 2.54-6P-WT @ LCSC](https://lcsc.com/product-detail/Wire-To-Board-Wire-To-Wire-Connector_CAX-2-54-6P-WT_C722706.html)

- Make a cable with separate pins, or a specific cable for a specific board, and connect it in one move.

- Supply pover to target via XH-2.54-2P connector or several VIO+GND pairs

- Monitor target's voltage over VIO+GND pairs

- Use all of the I/O pins of FT232RL chip

- Add of remove solderbridges from LEDs to control power consumption

- Program raw ESP32 modules without wiring extra transistors and resistors


## Q&A:

- Why should I use this board if there's a $1.5 FT232 knock-off on Ali?
  
  Honestly, you probably should have that product just because it's a great value. Yet, it does not allow you to do a lot of thing, which this boards allows, like operate at 1.8V or comfortably supply an external power.

- XH-2.54-6P sound scary, why is it not built with good old pin headers?
  Typical 2.54 pin headers where really and afterthought for this board, although I realize some people might really be inclined to use those. The thing is, if you work on one board for an extended period of time -- you will most likely will be irritated by the need to reconnect UART to the specific pins and pay attention every time. With this board, you at the very least can have known & stable connection on one side, and an ability to make a custom cable on the other. You can a) just buy a one side pre-assembled XH-2.54-6P cable, and connect some typical connector on the other or b)  get yourself a tool like [Crimping pliers SN 04BM](https://www.aliexpress.com/item/4000005467806.html) and actually build whatever the hell you want in a couple of minutes.
