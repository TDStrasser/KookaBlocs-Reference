----
Pins
----


The **Pins** category, shown in :numref:`pinpalette`, provides the means to control what the **Pins** do.

.. _pinpalette:
.. figure:: images/pins-palette.png
   :scale: 50%
   :align: center
   
   The palette of **KookaBlocs** **Pins** blocks

**Pins** are electrical connectors on the **Kookaberry**.  

The **Kookaberry** circuit board has five plugs on the rear numbered ``P1`` to ``P5``.  

``P3`` has four electrical pins and the rest have 3 pins.  

On each connector two of the pins are used for positive and negative power connections.  The remaining pin(s) have 
multiple uses as digital or analogue inputs or outputs.

In some of the **Pins** blocks it is possible to replace the drop-down selection block with a **String** block.   
This is useful when using **Pins** other than those exposed on the rear of the **Kookaberry**, 
or when other microprocessor boards that are compatible with **Kookaberry** firmware are being used.  
In those cases type in the Pin's identifier into the **String** block, as shown in :numref:`pinstring`.



.. _pinstring:
.. figure:: images/pins-string-nomination.png
   :scale: 50%
   :align: center
   
   Using a **String** value block instead of a **Pins** drop-down selection.

There are break-out (expander) circuit boards for the **Kookaberry** and the **Pi Pico** that make more of the **GPIO Pins** available for
connection and therefore practical use within **KookaBlocs** scripts.

Pin Turn ON
-----------

The Pin Turn ON block causes the selected pin to behave as a digital output and to be turned on with an output voltage of +3.3 volts DC.


.. image:: images/pins-turn-on.png
   :scale: 50%
   :align: center
   :alt: Turn Pin On Block


Pin Turn OFF
------------

The Pin OFF block causes the selected pin to behave as a digital output and to be turned off with an output voltage of 0 volts DC.

.. image:: images/pins-turn-off.png
   :scale: 50%
   :align: center
   :alt: Turn Pin Off Block


Pin Toggle
----------

The Pin Toggle  block causes the selected pin to behave as a digital output and to change state from ``OFF`` to ``ON``, 
or from ``ON`` to ``OFF``, depending on its existing state.

.. image:: images/pins-toggle.png
   :scale: 50%
   :align: center
   :alt: Toggle Pin Block


``OFF`` sets the Pin to 0 volts DC, and ``ON`` sets the Pin to +3.3 volts DC.

Set Pin to Digital Value
------------------------

The Pin Set Pin Digital Value block causes the selected pin to be set to according to the integer value of the input block.

.. image:: images/pins-set-digital.png
   :scale: 50%
   :align: center
   :alt: Set Pin Block

If the input value is ``0``, the output of the Pin will be set to ``OFF`` which is 0 volts DC.

If the input value is not ``0``, typically ``1`` or greater, then the output of the Pin will be set to ``1`` which is +3.3 volts DC.


Get Pin Digital Value
---------------------

This value block designates the selected pin as a digital input and returns the digital value of the 
input as either ``0`` if the input voltage is close to 0 volts DC, or ``1`` if the input voltage is closer to +3.3 
volts DC.


.. image:: images/pins-get-digital.png
   :scale: 50%
   :align: center
   :alt: Get Pin Block


.. important:: 
    The allowable **Pin** input voltage range for the **Kookaberry** is 0 volts to +3.3 volts DC.  
    Applying voltages outside that range may irreparably damage the **Kookaberry**.


Get Pin Voltage
---------------

This value block designates the selected pin as an analogue input and returns a floating point value of the input in volts DC.


.. image:: images/pins-get-voltage.png
   :scale: 50%
   :align: center
   :alt: Get Pin Voltage Block

.. important:: 
    The allowable **Pin** input voltage range for the **Kookaberry** is 0 volts to +3.3 volts DC.  
    Applying voltages outside that range may irreparably damage the **Kookaberry**.


Get Pin Voltage as Percentage of Maximum
----------------------------------------
 
This value block designates the selected pin as an analogue input 
and returns an integer percentage value of the allowable **Kookaberry** input voltage range.

.. image:: images/pins-get-percentage.png
   :scale: 50%
   :align: center
   :alt: Get Pin Percentage Block


Applying 0 volts DC to the input Pin will resturn a value of ``0``.

Applying +3.3 volts DC to the input Pin will resturn a value of ``100``.

.. important:: 
    The allowable **Pin** input voltage range for the **Kookaberry** is 0 volts to +3.3 volts DC.  
    Applying voltages outside that range may irreparably damage the **Kookaberry**.


Set Pin to Voltage
------------------

Where available on the **Kookaberry** the Set Pin to Voltage block causes the selected pin to behave 
as an analogue output and to be set to the voltage specified by the input block.

.. image:: images/pins-set-voltage.png
   :scale: 50%
   :align: center
   :alt: Set Pin Voltage Block


.. note::  **Set Pin to Voltage** is not available on **Kookaberry** using the Raspberry **Pi Pico RP2040** microprocessor.

Set Pin to Percentage of Maximum
--------------------------------

Where available on the **Kookaberry** the Set Pin to Percentage of Maximum block causes the selected pin to behave 
as an analogue output and to be set to the percentage of maximum voltage specified by the input block.  

.. image:: images/pins-set-percentage.png
   :scale: 50%
   :align: center
   :alt: Set Pin Percentage Block

The output voltage will rise from 0 volts DC to +3.3 volts DC linearly with the input block rising from ``0`` to ``100``.

.. note::  **Set Pin to Percentage of Maximum** is not available on **Kookaberry** using the Raspberry **Pi Pico RP2040** microprocessor.


Pin – Pulse Width Modulation (PWM)
----------------------------------

Pulse Width Modulation (PWM) oscillates the selected Pin as a digital output between ``0`` (0 volts) 
and ``1`` (+3.3 volts DC) at a given frequency and duty cycle as specified in the input blocks.  

.. image:: images/pins-set-pwm.png
   :scale: 50%
   :align: center
   :alt: Set Pin PWM Block


The duty cycle is the proportion of each oscillation in which the output state is set to 1.  A duty cycle of 50  
means that the oscillation is ``0`` for 50% of the time and `1` for the remaining 50%.

The frequency is the number of times the output cycles per second.  Frequency can be any positive floating point value

Both frequency and duty can be derived from other value blocks or specified directly.

PWM is used to apply speed control to DC motors by varying the duty cycle from 0% (motor is 
stopped) to 100% (motor at full speed). Additional circuitry is required to deliver the electrical 
power that a motor requires.

PWM can also be used to play tones through a loudspeaker by varying the frequency according 
to the pitch required.  A frequency of 440Hz corresponds to the musical note of middle A on a 
piano, for example.  Duty cycle is usually set to 50% but other interesting harmonics may be 
produced by varying the duty cycle over a limited range around 50%.  Additional circuitry is also 
required to successfully drive a loudspeaker.

See also https://en.wikipedia.org/wiki/Pulse-width_modulation

.. important::
  Please note that motors and loudspeakers should not be directly plugged into a **Kookaberry** 
  connector.  These devices require special electronics to supply more power.  
  
  Plugging in motors or loud speakers without the necessary driving electronics may irreparably damage the **Kookaberry**.





