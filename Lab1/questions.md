# Questions lab 1

### Question 1 
*Research the frequencies of the ISM bands, and describe where you would expect
to find the signal, given the properties of radio waves at these particular and 
the typical use case of garage door opener. At which frequencies do you not 
expect to find the signal? Explain why.*

[wiki ISM bands](https://en.wikipedia.org/wiki/ISM_band)

[wiki short range devices](https://en.wikipedia.org/wiki/Short_Range_Devices)

[wiki garage door opener](https://en.wikipedia.org/wiki/Garage_door_opener)

The wiki says that garage door openers are between 300-400 MHz, so the ISM band
closest to that is the 433.05-434.79 MHz. The frequency of the signal should
not be to high to limit power usage, and to allow the signal to go through
walls. On the other hand, a signal with a very low frequency can be picked up
from afar, so the signal should be high enough to limit the range.


### Question 2
*Analyze the signal in the time and frequency domain, and describe your 
observations. What can you conclude about the signal’s modulation? Record the 
frequency and bandwidth of the signal for later processing.*

There are power intensity changes at 433 MHz when pressing a button on the 
garage door opener. This implies that Amplitude Modulation is used. In the 
time domain this is very well visible


### Question 3 
*Demodulate the signal based on the modulation type
you identified earlier and study the signal. What information is
transmitted by the garage door remote?*

> Bitsequence: 1011001111001010000010000, or inverted. Depending on whether
a 'long' is a one or a zero.


### Question 4 
*Compare each of the transmissions, describe how
does the protocol of the wireless remote works. What triggers the
garage door to open and close?*

> Send predefined bitsequence for opening and closing the garage door

### Question 5 
*Assemble a signal that is able to open the garage
door and transmit it. Ensure that the “garage door” opens.*

> TODO

### Question 6
*Describe the weakness of the garage door opener
protocol. How would you change the communication protocol
so that the basic signal injection you have just done would no
longer be successful? What would be necessary for the designers
to accomplish this. Aside from the cryptographic and network-
security related aspects, also comment on usability aspects of
your proposed solution.*

> both have a key, garage door asks to encrypt a certain sequence

### Question 7 
*Given the chart, estimate the beamwidth of the antenna. What range extension 
would you expect in boresight?*

> ?

### Question 8
*Plot a chart of distance versus signal strength ob-
served by the SDR. Mark when the garage door stops to react
to the signals sent by the remote. When can the SDR no longer
receive and decode the transmission? Mark this threshold in the
chart as well.*


### Question 9 
*Based on the approximate receiver sensitivity of the
garage door, estimate from how far away an adversary could
successfully observe and inject a signal only based on antenna
gain.*


