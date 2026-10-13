# Variable DC Power Supply (1.25V - 13.5V, 2A)
The project illustrates the implementation of analog circuit design and fabrication from the concepts learned in class.

+ ## Key Parameters
  + ### Input: 14V DC Supply (4 x 3.7V Lithium-ion batteries wired in series)
  + ### Output Voltage: 1.25V to 13.5V (variable)
  + ### Output Current: up to 2A


+ ## Analog Circuit Design & System Architecture
  The heart of the power supply consists of LM317 linear voltage regulator, used to reduce the input 14V DC unregulated voltage to a regulated and variable output.
  + ### Voltage Regulator: The circuit includes LM317 regulator configured with 560 ohms fixed resistor (R1).
  + ### Resolution: The feedback network consists of two potentiometers (RV1) in series: 10k ohms and 1k ohms (RV2) to provide precision voltage control.
  + ### Noise Filtering: A 0.1uF capacitor (C1) is added to the input of the circuit to remove the high frequency noise. Also, 1uF capacitor (C2) is added to the output to provide transient stability of the output voltage and prevent oscillations.

+ ## Custom PCB Layout Design (KiCad)
  The schematic has been converted into a custom Printed Circuit Board (PCB) in KiCad.
  The key aspect in this case was to provide proper placement of the components to eliminate noise and provide proper cooling for the TO-220 packaged LM317 regulator.
The circuit board included two potentiometers (RV1, RV2), regulator, capacitors (C1, C2), and input/output terminal headers.

+ ## Prototyping & Fabrication
  Based on the design rules of KiCad the final prototype has been manually assembled and soldered onto the perfboard.
  + ### Enclosure: All electronic parts are placed inside a custom enclosure with a control panel in front.
  + ### Interface: The front panel includes two knobs for potentiometers and a built-in digital panel meter with voltage/current readings.
    
