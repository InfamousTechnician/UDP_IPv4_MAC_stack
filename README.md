# UDP_IPv4_MAC_stack
Basic and fast UDP IPv4 MAC stack written in VHDL for communication with 1 PC through 1 direct cable connection.

Limitations:
- no MDIO
- no ARP
- no ICMP
- payloads have to be over 46 bytes
- all addresses are hard coded
- fairly large footprint compared to its limitations, due to the high speed pipelines

Advantage:
- works at 1Gbits/sec even on Xilinx Spartan-3 (90nm process) devices

State of development:
- the transmitter has been proven to work on an Artix FPGA and freezes my Windows laptop with a clear 1Gbit/s steady UDP stream when I turn it on
- after that the receiver I tested against the code of the transmitter in simulation

Use case:
- well you can still DoS your PC with the transmitter very cheaply
- even 10Gb/s with an Artix would be possible if only it had 10Gb/s transceivers, yet with XAUI it is still an option
