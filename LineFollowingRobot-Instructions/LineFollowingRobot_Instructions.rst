Line Following Robot
====================

Design and instructions for a DIY line-following robot kit.

This kit is designed as a **"Learn to Solder"** kit.

*By: Matthew Little*

*Date: 27th March 2017*

*email: hello@curiouselectric.co.uk*

Overview
-------

.. image:: Photos/InUse1_sm.jpg?raw=true
   :width: 400px

This robot will follow a black line on a light coloured background.

The sensors at the front of the robot detect the change in light and control two motors to follow the line.

The circuit uses two comparator circuits and two light dependent resistor sensors to measure the reflected light.

This kit is fully analog and requires no programming.


Kit Contents
------------

.. image:: Photos/Components1_sm.jpg?raw=true
   :width: 400px

This kit contains the following parts:

Electronics:

+------+-----------------+--------------------------+
| REF  | Description     | Details                  |
+======+=================+==========================+
| C1   | Capacitor       | 100uf Electrolytic       |
+------+-----------------+--------------------------+
| C2   | Capacitor       | 100uf Electrolytic       |
+------+-----------------+--------------------------+
| D1   | LED Red         |                          |
+------+-----------------+--------------------------+
| D2   | LED Red         |                          |
+------+-----------------+--------------------------+
| D4   | LED Bright Red  |                          |
+------+-----------------+--------------------------+
| D5   | LED Bright Red  |                          |
+------+-----------------+--------------------------+
| IC1  | Voltage comparator IC |   LM393            |
+------+-----------------+--------------------------+
|      | IC socket       | 8 Pin                    |
+------+-----------------+--------------------------+
| R1   | Adjustable Resistor        |  10k          |
+------+-----------------+--------------------------+
| R2   | Adjustable Resistor        |  10k          |
+------+-----------------+--------------------------+
| R3   | Resistor        | 3.3k Ohm                   |
+------+-----------------+--------------------------+
| R4   | Resistor        | 3.3k Ohm                   |
+------+-----------------+--------------------------+
| R5   | Resistor        | 51 Ohm                   |
+------+-----------------+--------------------------+
| R6   | Resistor        | 51 Ohm                   |
+------+-----------------+--------------------------+
| R7   | Resistor        | 1k Ohm                   |
+------+-----------------+--------------------------+
| R8   | Resistor        | 1k Ohm                   |
+------+-----------------+--------------------------+
| R9   | Resistor        | 10 Ohm                   |
+------+-----------------+--------------------------+
| R10  | Resistor        | 10 Ohm                   |
+------+-----------------+--------------------------+
| R11  | Resistor        | 51 Ohm                   |
+------+-----------------+--------------------------+
| R12  | Resistor        | 51 Ohm                   |
+------+-----------------+--------------------------+
| R13  | LDR Resistor    | CDS5                     |
+------+-----------------+--------------------------+
| R14  | LDR Resistor    | CDS5                     |
+------+-----------------+--------------------------+
| Q1   |  Transistor     | 8550                     |
+------+-----------------+--------------------------+
| Q2   |  Transistor     | 8550                     |
+------+-----------------+--------------------------+
| SW1  |  Switch         |                          |
+------+-----------------+--------------------------+
| PCB  |  Circuit board  |                          |
+------+-----------------+--------------------------+

Hardware:

+------+-----------------+--------------------------+
| Quantity | Description  | Details                  |
+======+=================+==========================+
| 2     | Geared motor   | JD3-100                  |
+------+-----------------+--------------------------+
| 2    |  Wheel piece 1  |                          |
+------+-----------------+--------------------------+
| 2    |  Wheel piece 2  |                          |
+------+-----------------+--------------------------+
| 2    |  Wheel piece 3  |                          |
+------+-----------------+--------------------------+
| 2    |  Silicone Tyre  | 25x25mm                  |
+------+-----------------+--------------------------+
| 4    |  Wheel screw    |  M3x10                   |
+------+-----------------+--------------------------+
| 4    |  Wheel nut      |  M3                      |
+------+-----------------+--------------------------+
| 2    |  Wheel shell screw  |                      |
+------+-----------------+--------------------------+
| 1    |  Castor screw   |   M5x30                  |
+------+-----------------+--------------------------+
| 1    |  Nut            |   M5                     |
+------+-----------------+--------------------------+
| 1    |  Caster nut     |   M5 Ball nut            |
+------+-----------------+--------------------------+

Tools Required
--------------
The following tools will be required:

+-----------------+--------------------------+
| Tool            | Description              |
+=================+==========================+
| Soldering Iron  | 25W+ is best             |
+-----------------+--------------------------+
| Solder          | I use lead-free solder   |
+-----------------+--------------------------+
| Side-cutter     | For cutting excess leads |
+-----------------+--------------------------+

.. image:: Photos/tools1_sm.png?raw=true
   :width: 400px

A useful guide for learning to solder is available here:

https://cdn.shopify.com/s/files/1/0943/8168/files/soldercomic.pdf

And a more detailed guide is available here:

https://cdn.shopify.com/s/files/1/0943/8168/files/FullSolderComic_EN.pdf

Step 1: Solder Fixed-Value Resistors
------------------------------------
There are 10 fixed value resistors used in this circuit. These are labelled R3-R12.

Solder these into the respective marked places on the PCB.

+------+-----------------+--------------------------+
| REF  | Value     | Details                        |
+======+=================+==========================+
| R3   | 3.3k Ohm        |  Orange-Orange-Black-Brown-Brown  |
+------+-----------------+--------------------------+
| R4   | 3.3k Ohm        | Orange-Orange-Black-Brown-Brown  |
+------+-----------------+--------------------------+
| R5   | 51 Ohm          | Green-Brown-Black-Gold-Brown     |
+------+-----------------+--------------------------+
| R6   | 51 Ohm          |  Green-Brown-Black-Gold-Brown     |
+------+-----------------+--------------------------+
| R7   | 1k Ohm          |  Brown-Black-Black-Brown-Brown  |
+------+-----------------+--------------------------+
| R8   | 1k Ohm          |  Brown-Black-Black-Brown-Brown  |
+------+-----------------+--------------------------+
| R9   | 10 Ohm          |  Brown-Black-Black-Gold-Brown  |
+------+-----------------+--------------------------+
| R10  | 10 Ohm          |  Brown-Black-Black-Gold-Brown  |
+------+-----------------+--------------------------+
| R11  | 51 Ohm          |  Green-Brown-Black-Gold-Brown     |
+------+-----------------+--------------------------+
| R12  | 51 Ohm          |  Green-Brown-Black-Gold-Brown     |
+------+-----------------+--------------------------+

.. image:: Photos/PCB1_sm.jpg?raw=true
   :width: 400px

.. image:: Photos/PCB2_sm.jpg?raw=true
  :width: 400px

Step 2: Solder IC Socket
------------------------

Solder the IC socket into the holes marked IC1. Ensure the notch on the IC socket aligns with the notch on the silk-screen.

.. image:: Photos/PCB3_sm.jpg?raw=true
   :width: 400px

Info: The data sheet for the IC is here: https://www.onsemi.com/pub/Collateral/LM393-D.PDF

Step 3: Solder the Red LEDs
---------------------------
There are two RED LEDs to solder in locations D1 and D2.
You must ensure correct polarity of these LEDs.

The positive lead will be the longer lead. The negative lead has a slightly flat side to the LED case. These should align with the markings "+" on the PCB.

Please see photos for clarification.

.. image:: Photos/PCB4_sm.jpg?raw=true
   :width: 400px

Step 4: Solder Adjustable Resistors
------------------------
There are two 10k adjustable resistors to solder into holes marked R1 and R2.

.. image:: Photos/PCB5_sm.jpg?raw=true
   :width: 400px

Step 5: Solder Switch
------------------------
There is one on/off switch to be soldered into the holes marked S1.

   .. image:: Photos/PCB6_sm.jpg?raw=true
      :width: 400px

Step 6: Solder Capacitors
------------------------
The capacitors are 100uf capacitors and are soldered into holes marked C1 and C2.

These are electrolytic capacitors and you **must ensure the correct polarity**.

There is a white line marked on the capacitor which indicate the negative pin. This pin must align with the large white area of C1 on the PCB silk screen.

Another way to find the pin polarity is that the positive (+) pin is on the bottom of the capacitor and the negative is on the top.
Please see photos for clarification.

.. image:: Photos/PCB7_sm.jpg?raw=true
   :width: 400px


Step 7: Solder the Transistors
------------------------
There are two transistors to solder in to the holes marked Q1 and Q2.

The transistors have three pins and must be placed into the holes so that the flat side on the transistor aligns with the flat side on the silk screen.

.. image:: Photos/PCB8_sm.jpg?raw=true
   :width: 400px


Step 8: Attach Battery Holder
-----------------------------

The battery holder is stuck onto the top of the PCB. The wires from the holder go through the hole at the back edge of the PCB and are soldered on the underside of the PCB.
You must ensure correct polarity with the RED lead going to the BT1 pad marked + and the BLACK wire going to the other pad.

.. image:: Photos/PCB9_sm.jpg?raw=true
   :width: 400px

   .. image:: Photos/PCB10_sm.jpg?raw=true
      :width: 400px

 Step 9: Attach Motors
 -----------------------------
The motors are stuck onto the underside of the PCB. With the wire included make 2 cables with 2 wires in each.
Solder these wires to the motor pads (sticking out from the back of the motors).

These are soldered to the M1 and M2 pads on the underside of the PCB.

The wire attached to the motor the furthest away from the PCB will go to the pad closest to the red LED. The wire connecting to the motor closest to the PCB will go on the other pad.
Please see photos for clarification.

.. image:: Photos/PCB11_sm.jpg?raw=true
  :width: 400px

.. image:: Photos/PCB12_sm.jpg?raw=true
   :width: 400px

.. image:: Photos/PCB13_sm.jpg?raw=true
 :width: 400px

.. image:: Photos/PCB14_sm.jpg?raw=true
  :width: 400px

.. image:: Photos/PCB15_sm.jpg?raw=true
  :width: 400px


Step 10: Attach front caster
-----------------------------

The front caster is built using an M5 bolt, along with a nut and a ball nut on the end.
The bolt goes through the PCB and is held in place with the M5 nut. The M5 ball nut is screwed on to the end.
As the ball nut is round it will glide along the ground.

.. image:: Photos/PCB16_sm.jpg?raw=true
  :width: 400px

Step 11: Solder Light Dependent Resistors
-----------------------------
The light dependent resistors (LDR) are soldered onto the underside of the PCB (see photo). These go into the holes marked R13 and R14 (on the underside of the PCB).
They need to be inserted and solder so that the head of the LDR is around 5mm from the ground.
The LDRs do not have a polarity.

.. image:: Photos/PCB17_sm.jpg?raw=true
   :width: 400px


Step 12: Solder LEDs
-----------------------------
The last two LEDs are super-bright LEDs. They provide the light which is reflected back from a white surface, but not from a black surface.

You must ensure correct polarity of these LEDs.

The positive lead will be the longer lead. The negative lead has a slightly flat side to the LED case. These should align with the markings "+" on the PCB.

Please see photos for clarification.

.. image:: Photos/PCB18_sm.jpg?raw=true
  :width: 400px


Step 13: Add Wheels
-----------------------------

The wheels fit onto the motor shaft and are held in place with the two small self-tapping screws.

The silicone tyres fit over the wheels to provide grip.

.. image:: Photos/PCB19.jpg?raw=true
  :width: 400px

Step 14: Finished!
------------------------

Add some AA batteries into the battery holder (double check their polarity!). Press switch S1 and the unit should start to move.

You can adjust R1 and R2 to adjust the sensitivity of each sensor. Typically around half-way on each resistor works well.

.. image:: Photos/InUse1_sm.jpg?raw=true
   :width: 400px

.. image:: Photos/InUse2_sm.jpg?raw=true
   :width: 400px


Troubleshooting
--------------------
This circuit is relatively simple and designed for the beginner. There are some items which have a polarity and the circuit will not work if any of the following are places the wrong way around:
- Diodes
- LEDs
- Capacitors
- Transistors
- IC orientation

Please double check these in case of any issues.

Also it might be that one of the motors moves in the wrong direction (the robot will be going around in circles or moving away from the line). If this is the case then we need to swap around the wires to the motor.
This is easiest to change by unsoldering the wires from the motor pads and swapping them around.

Please also double check the soldering to ensure that there are no short circuits (solder connecting two pads) or 'dry joints' (which do not have enough solder or are not clean).

Circuit Schematic
-------------------
.. image:: Photos/Schematic.png?raw=true
   :width: 400px

Suppliers Information
----------------------
We would like you to be happy with this kit. If you are not happy for any reason then please contact us and we will help to sort it out.

Please email **hello@curiouselectric.co.uk** with any questions or comments or please tweet us at **@curiouselectric**

If any parts are missing from your kit then please email **hello@curiouselectric.co.uk** with details and, if possible, where the kit was purchased.

More technical information can be found via **www.curiouselectric.co.uk**

The GITHUB repository for all these files is: **https://github.com/curiouselectric/soldersolar**

This kit has been designed and produced by:

.. image:: Photos/CuriousElectricCompany_Logo_Round_Logo_sm.png?raw=true
   :width: 400px

..

   The Curious Electric Company

   hello@curiouselectric.co.uk

   www.curiouselectric.co.uk

   Hopkinson,

   21 Station Street,

   Nottingham,

   NG2 3AJ, UK
