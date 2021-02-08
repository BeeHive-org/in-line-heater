# in-line-heater


A lot of the experiments performed under microscopes, require the maintenance of biological tissue under conditions suitable for the tissue. This is normally accomplished by the preparation of solutions that deliver required nutrients, keep Ph stable, prevent metabolites from accumulating on the tissue and of a system to perfuse this solution on/around the tissue, so that the tissue is bathed in the solution. Another need is the maintenance of a constant and correct temperature. 

This repository contains files and instructions for the construction of an inline heater. 

This system is basically a glass tube that sits in line with the tubing used to deliver the solution to the tissue. Around the glass tubem we use ni-chrome wire, which is in short temperature resistant and keeps regular resistance over a wide temperature range. This wire than receives a voltage accross (12V in this case), which will heat up the wire, the glass, and in sequence the solution passing through the glass. 

The temperature control is made by using a couple of temperature sensors on the glass tube and closer to where the solution is actually used. Sending information from the sensor to a microcontroller allows us to dynamically change the voltage being sent to the ni-chrome wire. 

With this closed loop, and using a microcontroller, we can keep a log of the temperature (and even send it periodically to the software recording experimental data). This allows for fine temperature control, but also for other neat things as:
- systematic changes of solution temperature, to observe tissue response
- pairing tissue response with recorded data, for a full control of experimental conditions.





