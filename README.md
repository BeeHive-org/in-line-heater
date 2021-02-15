# in-line-heater


A lot of the experiments performed under microscopes, require the maintenance of biological tissue under conditions suitable for the tissue. This is normally accomplished by the preparation of solutions that deliver required nutrients, keep Ph stable, prevent metabolites from accumulating on the tissue and of a system to perfuse this solution on/around the tissue, so that the tissue is bathed in the solution. Another need is the maintenance of a constant and correct temperature. 

This repository contains files and instructions for the construction of an inline heater. 

This system is basically a glass tube that sits in line with the tubing used to deliver the solution to the tissue. Around the glass tubem we use ni-chrome wire, which is in short temperature resistant and keeps regular resistance over a wide temperature range. This wire than receives a voltage accross (12V in this case), which will heat up the wire, the glass, and in sequence the solution passing through the glass. 

The temperature control is made by using a couple of temperature sensors on the glass tube and closer to where the solution is actually used. Sending information from the sensor to a microcontroller allows us to dynamically change the voltage being sent to the ni-chrome wire. 

With this closed loop, and using a microcontroller, we can keep a log of the temperature (and even send it periodically to the software recording experimental data). This allows for fine temperature control, but also for other neat things as:
- systematic changes of solution temperature, to observe tissue response
- pairing tissue response with recorded data, for a full control of experimental conditions.


provisional BOM:
|item |qty|link|obs|
|--|--|--|--|
|hi-temp masking tape|01|https://www.ebay.co.uk/itm/1-Blue-Polyester-Tape-25mm-x-66m-Powder-Coating-High-Temp-Masking-Tape/223507353071| about 3cm wide is easier to manipulate - used to isolate the wire from the metal tubing, as well as attaching the wire to the tube|
|3mm stainless stell tube 25cm |01|https://www.ebay.co.uk/itm/192736215338|thickness will depend on the rest of the tube line|
|12V 5A power supply|01|https://www.ebay.co.uk/itm/12V-1-2-3-4-5-6-8-10A-Power-Supply-AC-to-DC-Adapter-5050-3528-LED-Strip-Light-UK/293137585107|this will be used to pwoer the entire system (heating plus electronics)|
|nichrome (resistive wire) 0.2mm thick|1 metre|https://uk.rs-online.com/web/p/multicore-industrial-cable/7496335/|this will heat up when current is passed through it. the longer it is the more resistance it will have, so possibily more heat, but also more power will be needed datasheet:https://docs.rs-online.com/bebf/0900766b815fcf12.pdf|
|||||
|||||



