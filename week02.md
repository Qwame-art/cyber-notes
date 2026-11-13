#Week 2 Note

##Day 1

Week 2: Binary and Data

Difference Between a Bit and a Byte

A bit is the smallest unit of data in a computer. It can have only two values: 0 or 1.

A byte is a group of 8 bits. Computers use bytes to represent and store information such as text, numbers and other data.

Why One Byte Can Only Count Up to 255

One byte contains 8 bits, and each bit has two possible values (0 or 1). Therefore, 8 bits can produce 256 different combinations (2⁸ = 256).

Since counting starts from zero, the highest number one byte can represent is 255.

The smallest value is 0 (00000000), while the largest value is 255 (11111111).




ss

##Day 2 : Binary by Hand

1. Decimal to Binary Conversions

(a) Convert 13 to binary

13 = 8 + 4 + 1

Binary = "00001101"

(b) Convert 200 to binary

200 = 128 + 64 + 8

Binary = "11001000"

(c) Convert 255 to binary

255 = 128 + 64 + 32 + 16 + 8 + 4 + 2 + 1

Binary = "11111111"

2. Binary to Decimal Conversions

(d) Convert 10101010 to decimal

= 128 + 32 + 8 + 2

= 170

Answer: 170

(e) Convert 01100100 to decimal

= 64 + 32 + 4

= 100

Answer: 100

(f) Convert 11000000 to decimal

= 128 + 64

= 192

Answer: 192

3. Bits vs Bytes: Download Time

(g) How many seconds will a 50 MB file take to download at 10 Mbps?

Given:

File size = 50 MB

Download speed = 10 Mbps

1 byte = 8 bits

Convert megabytes to megabits:

50 × 8 = 400 megabits

Download time = File size ÷ Download speed

= 400 ÷ 10

= 40 seconds

Answer: 40 seconds.

(h) Download time using my own internet connection

Website used: https://fast.com

Download speed: [Enter the speed measured by Fast.com] Mbps

File size = 50 MB

50 × 8 = 400 megabits

Download time = 400 ÷ 230

Answer: [1.74] seconds.



(h) Download time using my own internet connection

Website used: Fast.com

Download speed: 230 Mbps

File size = 50 MB

50 × 8 = 400 megabits

Download time = 400 ÷ 230

= 1.74 seconds

Answer: Approximately 1.74 seconds.



## Day 3: IP Address and Networking
Three things about my Wi-Fi connection

IPv4 Address..........10.46.181.251
Subnet Mask...........255.255.255.0
Default Gateway.......10.46.181.6


Addresses in binary
11000000.10101000.0000001.00000001


Private or Public IP address
IP address            classification
192.168.0.10          private
8.8.8.8               public
10.1.2.3              private
172.20.5.4            private
172.32.0.1            public
41.66.10.20           public


How to identify private IP address:
There are three main private IPv4 ranges:
.10.0.0.0 - 10.255.255.255
.172.16.0.0 - 172.31.255.255
.192.168.0.0 - 192.168.255.255

Ping Lab
First test:8.8.8.8
Time :54ms
TTL : 115
packets lost : 0% loss

Second test: ping google.com
Time : 168ms
TTL : 109
packets lost: 0% loss





## Day 4:  How the internet works: bits, IP addresses, DNS and packets

1. Spot the Fake (Look-alike Domains)

Scammers may create fake domain names that look similar to the official MTN Ghana website ("mtn.com.gh") to trick users.

Three examples and how to spot them:

1. mtnn.com.gh
   
   - How to spot it: Notice the extra letter "n" in the name. The official name has only one "n" at the end of MTN.

2. mtn-ghana.com.gh
   
   - How to spot it: Notice the additional word "ghana" and the hyphen. Always verify the official domain.

3. mtn-support.com.gh
   
   - How to spot it: The word "support" has been added to make the domain appear trustworthy. Verify it through MTN's official communication channels.

Conclusion:
Always check website addresses carefully before entering personal information or passwords. Never trust a website simply because its name looks familiar.

Note: These are illustrative examples, not verified registered domains. They should not be visited.


#Day 4:How the internet works: bits, IP addresses, DNS and packets

 TCP vs UDP

1. TCP (Transmission Control Protocol)

TCP is a communication protocol that ensures data is delivered accurately and in the correct order between devices. It checks whether data has arrived successfully and retransmits missing data.

Example: Web browsing (HTTPS).

Why: TCP helps ensure that website information, such as text and files, arrives correctly.

2. UDP (User Datagram Protocol)

UDP is a communication protocol that sends data quickly without establishing a connection or guaranteeing that every packet will arrive.

Example: Online video calls.

Why: UDP is useful for video calls because speed and low delay are important. Losing a small amount of data is often better than experiencing delays.

3. Differences between TCP and UDP

TCP| UDP
Reliable delivery| No guaranteed delivery
Connection-oriented| Connectionless
Generally slower| Generally faster
Checks delivery and order| Does not guarantee order

Conclusion: TCP focuses on reliable data delivery, while UDP focuses on speed and low delay.


 Follow Your Packets

1. Traceroute Lab

Command used: "tracert -d 8.8.8.8"

- Total number of hops: 14
- Hop 1 IP address: 10.239.195.80
- Default Gateway from Day 2: [10.239.195.80]
- Does Hop 1 match my Default Gateway? Yes

Observation: The packets passed through four hops before reaching Google's DNS server.


2. Near and Far

Destination 1: Google DNS (8.8.8.8)

- Hop count: [14]
- Three response times: [1905 ms  247 ms    198 ms]

Destination 2: Wikipedia (wikipedia.org)

- Hop count: [28]
- Three response times: [3073 ms 267 ms   231 ms]

Comparison:

The server with the higher hop count has more routing steps along the path. The response times help show how long communication takes.


3. Packet Loss Lab

Command used: "ping -n 20 8.8.8.8"

- Packets sent: [20]
- Packets received: [0]
- Packet loss: [20](100% loss),
- Minimum time: [44ms] 
- Maximum time: [180ms]
- Average time: [72ms] 

Observation:

The ping test helps determine whether packets are successfully reaching their destination and measures the time taken for responses to return.