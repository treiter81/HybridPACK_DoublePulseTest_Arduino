# WARNING: HIGH VOLTAGE HAZARD
* DANGER: This equipment involves lethal voltages. For use by qualified, trained personnel only in a controlled laboratory environment with appropriate safety measures.
* USER RESPONSIBILITY: The user assumes all risk and sole responsibility for operation.
* LIMITATION OF LIABILITY: No claims shall be made for any injury to persons or damage to equipment/property.
* MANDATORY STARTUP: Regardless of experience, start with a 12V supply only to verify operation and familiarize yourself with the system before applying high voltage.
* USE AT YOUR OWN RISK.

This Arduino project is not supported by Infineon Technologies AG. Motivation of this platform was to support open research activities. <br> If you need support with Infineon products like the power modules, gate drivers, do not hesitate to contact your local sales representative and/or the official support.

# HybridPACK_DoublePulseTest_Arduino
Double Pulse GUI. Project is very early DRAFT
* Pulse Resolution 10ns
* 1st Pulse; Wait; 2nd Pulse
* Support Short Circuit Testing


# Motivation and why Arduino:
Motivation of this platform was to support open research activities. <br>


# Get Started (fast track without MATLAB/Simulink):
* install the precompiled GUI (only Windows) from folder "CompiledWIN_noMATLAB"
* start the GUI
* ensure that firewalls not blocking WiFi access
* connect Arduino NANO IoT 33 via USB and click the "FlashTool Arduino" button in GUI. Just follow the instructions.
* disonnect USB cable after flash process!
* establish a WIFI hotspot with SSID: FUSION; PW: ffffffff
* connect the PC (running the GUI) to the WIFI. Click reset button on Arduino.
* after about 5..10s both PC and Arduino should be in WIFI. You can now click Connect button in GUI and start
* Start double pulses
  


# Multiple Arduinos running in same WIFI net:
* After connect click LockComChannel. A special command sequence is sent to Arduino and the communicatoin will be locked to this Key. Only a reset will release the Key.
* After 1st Arduino is operated in locked mode the next one can be started and should be also locked.


# Needed Toolchain SW:
Can be used without MATLAB/Simulink => use precomiled GUI. This GUI includes also precompiled bin file, which can be flashed. <br>
But recommended with MATLAB/Simulink:
  
* Matlab/Simulink R2022b (tested version) <br>

requires installed <br>
* MATLAB Support Package for Arduino Hardware <br> 
* Simulink Support Package for Arduino Hardware <br>



# Toolchain HW:
* Arduino Nano IoT 33 <br>
* WIFI Network <br>
* Infineon Arduino Interface PCB: EV PCB INT; SP006038346 <br>

Compatible Gate Driver Boards (just some examples): <br>
* <a href="https://www.infineon.com/evaluation-board/EV-GB-HPD2-FU" target="_blank">EV GB HPD2 FU; SP006070794 (for Si/SiC Fusion Power Modules)</a>  <br>
* <a href="https://www.infineon.com/evaluation-board/EV-GB-HPD2-SIC" target="_blank">EV GB HPD2 SIC;	SP006056143 (for SiC Power Modules)</a>  <br>
* <a href="https://www.infineon.com/evaluation-board/EV-GB-HPD2-SI-08" target="_blank">EV GB HPD2 SI 08; SP006038350 (for 750V IGBT Power Modules)</a>  <br>
* <a href="https://www.infineon.com/evaluation-board/EV-GB-HPD2-SI-12" target="_blank">EV GB HPD2 SI 12; SP006038348 (for 1200V IGBT Power Modules)</a>  <br> 



Compatible Power Modules (just some examples): <br>
* FS980R08A7F32B (Si/SiC Fusion Power Module 780V/980A) <br>
* <a href="https://www.infineon.com/part/FS01MR08A8MA2LBC" target="_blank">FS01MR08A8MA2LBC (SiC MOSFET Power Module 750V/1mOhm)</a>  <br>
* <a href="https://www.infineon.com/part/FS02MR12A8MA2B" target="_blank">FS02MR12A8MA2B (SiC MOSFET Power Module 1200V/2mOhm)</a>  <br>
* <a href="https://www.infineon.com/part/FS1150R08A8P3LBC" target="_blank">FS1150R08A8P3B (IGBT Power Module 750V/1150A) </a>  <br> 
* <a href="https://www.infineon.com/part/FS520R12A8P1LB" target="_blank">FS520R12A8P1LB (IGBT Power Module 1200V/520A)</a>  <br>
* many more

Information to the Gate Drivers: <br>
*  <a href="https://www.infineon.com/part/1EDI3035AS" target="_blank">SiC MOSFET and Si/SiC Fusion optimized Gate Driver 1EDI3035AS</a>  <br> 
*  <a href="https://www.infineon.com/part/1EDI3025AS" target="_blank">IGBT optimized Gate Driver 1EDI3025AS</a>  <br>




