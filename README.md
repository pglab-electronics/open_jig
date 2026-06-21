# Open JIG Test for FreeCAD

<img alt="Open JIG Test" src="https://github.com/pglab-electronics/open_jig_test/blob/main/img/open_jig_test.png" />

## Overview

This project is a FreeCAD design for a PCB test jig used for functional testing of small electronic boards.

The jig is designed to accommodate PCBs up to 90 × 80 mm, making it suitable for compact development boards and prototype electronics. All components used in the design are widely available online through major resellers such as Amazon and other electronics suppliers.

This project specifically is specifically for testing and validating [E-VLXESP32](https://www.pglab.dev/shop/p/e-vlxesp32). 
However, it can also be adapted for other similarly sized PCB designs.

## Status & Usage

The project is almost ready to use. However, some customization is required before fabrication.

You need to adapt the FreeCAD model according to your specific PCB dimensions, test points, and mounting hole positions to ensure proper alignment and reliable contact during testing.

Assembling the jig requires a certain level of skill and experience. The process can be time-consuming and may involve some trial and error to achieve proper alignment and reliable operation. For this reason, in some cases it may be more practical to purchase a 33 professionally manufactured jig from a specialized supplier.

However, if you like challenges and DIY projects, the Open Jig Test project is for you.

## Tools Required

To build and assemble this PCB test jig, the following tools are required:

- Soldering iron (for pogo pins electrical connections)
- 3D printer (for printing structural and supporting parts)
- Small drill press (mandatory for precise and accurate hole drilling)

## 3D Printing Notes

All structural parts should be 3D printed using PETG filament only. Do not use PLA, as it is not suitable for mechanical stress and long-term stability in this application.

Use a 0.3 mm layer height with 40% infill for all printed parts to ensure a good balance between strength and print time.

The majority of screws used in the design are M5. However, some holes in the Open JIG are sized at 6 mm. In these cases, you must install threaded brass heat-set inserts to ensure proper mechanical strength and durability.

## Pogo Pins & Alignment Pins

The pogo pins and alignment pins must be securely held by the 3D-printed support structure. Ensure that the printed parts provide a firm and stable press-fit or guided fit for all pins.

Use an appropriate drill bit size when finishing the holes to achieve accurate alignment and proper seating of the pins. After fitting, apply a small amount of super glue to secure the pogo pins and alignment pins in place.

In the model, two different types of pogo pins are supported. These pogo pins have been selected and modeled according to components commonly available on the market for purchase. The reference parts used in the design are:

- https://www.amazon.it/dp/B07SKD8Q42
- https://www.amazon.it/dp/B0CC2FR9VW

This ensures compatibility with readily available hardware and simplifies sourcing for assembly.


## How to Proceed

To correctly use and adapt this jig design, follow these steps:

Your PCB must include dedicated test points and at least two alignment pins. The test points can be placed on either the top or bottom side of the PCB, depending on your design requirements.

Make sure to use relatively large-diameter test pads to compensate for small misalignments of the pogo pins and to ensure reliable electrical contact.

As reference, here a top/bottom view of the E-VLXESP32 PCB.

<img alt="Open JIG Test" src="https://github.com/pglab-electronics/open_jig_test/blob/main/img/testing_points.png" />

- **Light Blue**: 3 mm alignment pins
- **Yellow**: pogo pins on the front side of the device, this ensure correct electrical contact and precise alignment of the 5 pogo pins located on the front side of the E-VLXESP32 board.
- **Red**: test points on the back side of the PCB

From your PCB design software, export the 3D model of your PCB and import it into the FreeCAD project of the Open JIG.

Place the PCB 3D model exactly on top of the body named PCB_Holder_Body inside the FreeCAD assembly. Modify the corner supports to exactly match your PCB dimensions.

In FreeCAD, you must also create guide holes in the body geometry to hold the pogo pins. These holes must be slightly smaller than the pogo pin diameter. At this stage, they are only used as positioning guides for later drilling and refinement to achieve precise final dimensions.

Once positioned, align the pogo pins precisely with the PCB test points.

Finally, ensure that the two alignment pins are correctly placed and aligned to guarantee repeatable and stable positioning of the PCB during testing.


## License
This work is licensed under the Creative Commons Attribution 4.0 International License.

To view a copy of this license, visit http://creativecommons.org/licenses/by/4.0/ or send a letter to Creative Commons, PO Box 1866, Mountain View, CA 94042, USA.

You are free to:
- Share
- Adapt
- Use commercially

Under the following terms:
- Attribution: You must give appropriate credit to the original project.



## Disclaimer
This is an independent design inspired by commercially available PCB test fixtures.
It is not affiliated with or endorsed by ELOPRINT.
