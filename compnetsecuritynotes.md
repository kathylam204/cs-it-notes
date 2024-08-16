# Computer Networks Security Notes

## Board Info: Sending Message Order
- Sender
- Receiver
- Message
- Medium
- Protocol

## Transmission Modes
- Simplex: One way
- Half Duplex: One person gets priority on the path; you can’t use it if they are.
- Full Duplex: Two people (or data paths) may use it.

## Network Criteria
- Performance: Sending time & receiving times
- Reliability
- Security: Protecting data

## Types of Connection
- Point-to-point
- Multipoint

## Topologies
- Star: 4 devices connected to a hub
- Bus: Devices connected in a line
- Ring: Devices connected in a ring/circle
- Mesh: All devices are connected to each other

## Calculations: S=((n(n−1))/(2))
​
## Organizations
- IEEE: Institute of Electrical and Electronics Engineers
- ISOC: Internet Society
- IAB: Internet Architecture Board
- IRTF: Internet Research Task Force
- IANA: Internet Assigned Numbers Authority
- ICANN: Internet Corporation for Assigned Names and Numbers
- NIC: National Informatics Centre

## Network Layers Models
- LAN: Local Area Network

## TCP/IP Model (5 layers)
- Application Layer: Message
- Transport Layer: Segment/User datagram (port numbers)
- Network Layer: Datagram (logical address)
- Data-Link Layer: Frame (link-layer addresses)
- Physical Layer: Bits

## OSI Model (7 layers)
- Physical
- Data Link
- Network
- Transport
- Session
- Presentation
- Application

## Signal Impairment
- Loss of energy/power/signal
- 𝑑𝐵=10log10 ( P2/P1), where P2 < P1

## Frequency and Bandwidth
- Time Domain: (x = time, y = amplitude)
- Frequency Domain: (x = frequency, y = amplitude)
- Bandwidth: Range of frequencies contained in a composite signal
- Capacity (C): C = B log2 (1+SNR)

## Bit Rate Calculation
- Nyquist Formula for bitrate: Bitrate=2B log2L

## Addressing
- IP Address: 0.0.0.0 - 255.255.255.255
- Port Address: 0 - 65535
- Physical Address: 00-00-00-00-00-00 to FF-FF-FF-FF-FF-FF
- ARPANET: The first public packet-switched computer network.

## Data Link Layer
- Broadcast: Megaphone
- Unicast: Just a few specific people
- ARP: Address Resolution Protocol
- MAC Address: 48 bits

## IP Addressing
- IPv4: 32 bits
- IPv6: 128 bits
- Classful Addressing:
- Class A: Network/8 bits, Host/24 bits
- Class B: Network/16 bits, Host/16 bits
- Class C: Network/24 bits, Host/8 bits

## Subnetting
### Subnet Mask Calculation
- Find the number of subnets needed.
- Subtract host bits from total bits to get subnet bits.
- Example: For /26, subnet mask = 255.255.255.192

## Routing
- Forwarding Table: Directs data to another router or destination.
- Indirect Delivery: Uses the next hop method.

## Protocols
- UDP: User Datagram Protocol
- TCP: Transmission Control Protocol

## IPv6
- Address format: Hexadecimal (8 columns)
- Loopback: ::1/128

## Encryption
- RSA: Public-key encryption

## Formula:
- n=p×q
- m=(p−1)×(q−1)
- Public key: (e, n)
- Private key: (d, n)

## Error Reporting
- Type
- Code
- Checksum
- Rest of the header
- Data section

### Signal-to-Noise Ratio (SNR): SNR = 1023 B = 6000Hz

### Line Coding

### Multiplexing: Combining signals

## Layers of Data:
- Application
- Transport (port)
- Network (IP address)
- Data link (physical address)
- Physical

### Port Number: 16 bits, 2^16 = 65536 ports

## IPv4 Header:
- Ver: 4 bits
- HLEN: 4 bits
- Service Type: 8 bits
- Total Length: 16 bits
- Identification: 16 bits
- Flags: 3 bits
- Fragmentation Offset: 13 bits
- Time-to-live: 8 bits
- Protocol: 8 bits
- Header Checksum: 16 bits
- Source IP: 32 bits
- Destination IP: 32 bits
- Options + Padding: 0-40 bytes
