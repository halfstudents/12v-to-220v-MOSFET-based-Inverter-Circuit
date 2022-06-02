# 12v-to-220v-MOSFET-based-Inverter-Circuit
A small but powerful inverter circuit can power up your small devices. A Inverter with square wave Ac on output.
Get more info from here:   https://www.instructables.com/12v-to-220v-MOSFET-Based-Inverter-Circuit/
JLCPCB- get $30 free coupon sign-up now:    https://jlcpcb.com/SSR

Inverters are widely used devices in electronics and electrical circuits. An inverter converts corresponding DC voltage into AC. We are very familiar with linear dc power supplies, which is used to convert 220v Ac into low voltage high ampere DC. In the same way, A high ampere battery or supply is required to step up voltage to required value. Transformers are very helpful in all of these cases. Induced EMF is based on number of turns and wire gauge.
Note** High voltage/ Square wave on high AC/ Circuit can handle 100w maximum with this driver stage. Overheating may occur if there is any further push in power limits.

To power up the load safely, we will make a PCB design and order it from best PCB manufacturer JLCPCB. You can order 5pcs of high quality 2-layer PCB in just $2. JLCPCB is one stop solution for all of my projects providing 3D printing, Stencil and SMT assembly service along with simple pcb prototypes in best prices. So, order you PCB now from JLCPCB and get free coupons on first sign-up.  https://jlcpcb.com/SSR

Type of Transformer required:
Step-down transformer is used to convert high voltage AC into DC. AC is supplied to the primary winding has a greater number of turns as compared to secondary and thus induced emf generate voltage in secondary winding. In the same way if we reverse the procedure, it can generate high voltage. For small loads (less than 100W) these transformers are great but we need more powerful and dedicated center tapped transformer. Which will cost more and need heavy driver circuitry with separate microcontroller unit.
Circuit Description:
The circuit is simple, IC CD4047 drives the two MOSFETs which are in push-pull configuration. As, the usual transformer cannot work on DC, so we have to make voltage and current changing circuit w.r.t time. So, the flux will induce in the core which will induce a voltage on the secondary winding. You can adjust the potentiometer to get the desired frequency. Usually, the frequency is 50 or 60 Hz.
The rating of the transformer should be enough to bear the output power. Battery should be greater than 10Ah so that battery voltage should not drop, and it should work for a long time. The LED here indicates that the power inverter is ON. So, whenever it is ON, don’t touch the inverter otherwise you will get harmed. https://jlcpcb.com/SSR

Working:
CD4047 works in the astable mode it continuously changes output at pin no 10 and 11 and thus giving a square wave output they are opposite to each other.
These two output pins are connected to the gate of the two MOSFETs which are arranged in push-pull configuration. So at a time, only one transistor is on. These transistors can handle a very high current through them.
The source of both the MOSFETs is connected to the ground and the drain is connected to the two ends of the secondary winding of the transformer. The centre taped wire is connected to +12VCC.
when the first MOSFET Q1 is on the current path is { +ve terminal => transformer => transistor Q1 => -ve terminal of battery}, and when MOSFET Q2 is on the current path is { +ve terminal => transformer => transistor Q2 => -ve terminal of battery}.
By this method, an alternating current(AC) is produced in the secondary winding (having a smaller number of turns) of the transformer. This alternating current induces a High Voltage AC in the primary(having more number of turns) winding of the transformer. This induced current is not sinusoidal, it is an alternating square wave. this current can easily run 100W bulb a small table fan and some other non-sensitive electronic devices.
