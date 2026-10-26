# MIDI-Keyboard
MIDI Keyboard is a small piano-like PCB made with a Waveshare ESP32-S3-ZERO. It uses switches, touch sensors, a rotary encoder, LEDs, and a Bourns Potentiometer.

I designed the schematic and PCB in KiCad, routed the traces, and exported the fabrication files. This is my Week 3 PCB project for Hack Club Half Life.


![MIDI Schematic](Screenshot%202026-10-23%20100507.png)
![MIDI PCB](Screenshot%202026-10-25%20204928.png)

## What it is

MIDI is designed to be like a piano, with capacitive touch sensores, switches, and a rotary encoder. It responds to touch, and plays sound from the response.

## How?

I started by following the guided MIDI Keypad project as this was really similar to my design.
After, I set up the schematic with the Waveshare ESP32-S3-ZERO, the rotary encoder, switches, bourns potentiometers, and the touch keys.
After this, I routed the traces, and checked it using designs rules checker to make sure that it was ok.
I finally exported the fabrication files and created a BOM based on it.

## Why?
I made it for the week 3 Half Life hackclub challenge, to learn about how to use KiCad and build a PCB and Schematic.

## BOM.csv
I looked towards Aliexpress for my parts, and used JLCPCB for my PCB vendor. For my Bourns Potentiometers, I first thought of aliexpress, but then I realized it was only really found in Digikey.
| Part | What it is used for | Quantity | Price | Vendor |
|---|---|---:|---:|---|
| [Waveshare ESP32-S3-ZERO]| Main microcontroller | 1 |$1.46| Aliexpress|
| [Rotary Encoder]|Knob on PCB | 1 | $1.52 |Amazon|
| [Bourns Potentiometers]| Sliders | 1 | $3.68 | Digikey |
| [SK6812 MINI-E]| LEDs for switches| 1 | $3.61 | Aliexpress |
| [Choc Switches]| Switches | 1 | $3.67 | Aliexpress |
| [PCB Fabrication]| Custom circuit board manufacturing | 1 | $8.61 | JLCPCB |

- **Parts Subtotal:** 22.55
- **Tax & Shipping:** $9.76
- **Total Project Cost:** **$32.31**


## Repository contents

- KiCad source files and fabrication exports
- PCB and Schematic renders
- BOM
- Gerber files
