# AquaSense — Arduino Smart Water Dispenser

A project guide and interactive browser simulation for an automatic, touch-free water dispenser concept.

## Run
Open `index.html` in a modern browser. No build tools required.

## What's included
- Component overview and illustrated part cards.
- System flow and conceptual connection table.
- Six-stage build guide.
- Starter Arduino sketch (`script.js` is only the website simulation; the Arduino sketch is in the page under Sample Arduino Sketch).
- Copy-code button.
- Interactive distance/threshold simulation.

## Suggested pin plan
- HC-SR04 VCC → Arduino 5V
- HC-SR04 GND → Arduino GND
- HC-SR04 TRIG → D9
- HC-SR04 ECHO → D10
- Driver signal input → D3
- Pump power → separate correctly rated DC supply through a suitable driver

## Critical safety information
The pump must NOT be powered from an Arduino I/O pin. Use a properly rated MOSFET/relay driver and a separate DC supply. Follow the exact driver module wiring diagram and verify voltage/current ratings and polarity. Keep the water path physically separated from electronics; use a fuse, switch, splash protection, drip loops, leak checks, and suitable food-contact materials. Never use mains wiring near the wet area.

This is a student project guide and browser simulation. The concept artwork and wiring plan are illustrative, not proof of a physically assembled or tested unit. Test each stage safely and verify all component datasheets before building. A prototype is not automatically safe for drinking water.
