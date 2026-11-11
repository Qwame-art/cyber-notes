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

Day 1: Binary by Hand

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



## Day 2: IP Address and Networking
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








