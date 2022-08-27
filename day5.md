# Communication Protocols

## UART (Universal Asynchronous Reciever-Transmitter)
The "alpha protocol" for machine-to-machine communication could be referred to as UART. This input is converted by the chip into serial data f
or transmission over a single transmit (Tx) line. Data receiving from an additional UART device is possible with a single receive (Rx) line.
Data transmission occurs between two devices and can be simplex (single direction), half-duplex (one direction at a time), 
or full-duplex (both directions concurrently).Simple UART wiring just requires connectors for Rx and Tx.It was earlier used in telegraphs.
## I2C (Inter Integrated Circuit)
Data is transferred via a bus consisting of two wires (SDA – serial data and SCL – serial clock) in half-duplex mode. Typically, 
a single master device is used to signal one or more slave devices. Each has a unique address to allow them to share the same bus.
This bus technology is generally faster than UART. Standard speeds run from 100kbit/s to as high as 5Mbit/s in ultra-fast mode. However, 
only half-duplex operation is available, and only one slave can be addressed at a time.
## SPI (Serial Peripheral Interface)
A single master device may send and receive data from one or more slaves. SPI is also the most complicated wiring-wise, requiring lines 
from the master device.SPI is generally the fastest of these three protocols. It's capable of sending and receiving simultaneously for 
full-duplex operation. SPI is often the best choice if speed is essential for a peripheral -- for example, in the case of an SD card reader,
or a quickly refreshing display.
