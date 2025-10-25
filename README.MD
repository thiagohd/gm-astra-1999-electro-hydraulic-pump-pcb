# PCB for the Electro-hydraulic pump - CHEVROLET ASTRA 1999

This repository aims to help anyone who need more information regarding the circuit or PCB components, with some images and references which may not be possible to find elsewhere.

I took some pictures whilst fixing this board with my colleague. We were able to fix the electronic board and make the pump work again properly.

## Damaged Dual Inverting MOSFET Driver

The board has 2 [ONSEMI Dual Inverting MOSFET Drivers MC33151](<Onsemi MC34151 MC33151.pdf>) on SOIC-8 package.

On this case, one of them was damaged, and had to be replaced. We couldn't find an exact replacement, so we went with the following alternative: [ONSEMI Dual Inverting MOSFET Drivers MC33151](<Microchip MIC4426YM.pdf>).

## Damaged Zener

The board had one damaged zener on an input line (probably the central command line), which was all burnt out. We figured that it should rectify the voltage accross a voltage divider that reaches the main driver, to around 3V3 signal level.

## Relay Transistor

The [NPN transistor](<NPN FMMT491A.PDF>) responsible for actuating the relay was not damaged.

## MOSFETS

The board has 4 [N-Channel MOSFETS](<N-MOSFET BUZ71.pdf>) for driving the rotor. None of them was damaged.

## 5V LDO

The [5V Regulator](<5V LDO TLE4265.pdf>) responsible for powering the processors was ok.