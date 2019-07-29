# UDP_IPv4_MAC_stack
Basic and fast UDP IPv4 MAC stack written in VHDL for communication with 1 PC through 1 direct cable connection.

Limitations:
- no MDIO
- no ARP
- no ICMP
- payloads hav to be over 46 bytes
- all addresses are hard coded
- fairly lareg design compared to its limitations, due to the high speed pipelines

Advantage:
- works at 1Gbits/sec even on Xilinx Spartan-3 (90nm process) devices
