# IP Addresses, Network Tools & Wireshark

As part of my journey, I've learned about the different types of IP addresses, some basic network troubleshooting commands, and how to look at network traffic!

## IPv4 vs IPv6
Every device on the internet needs an address, just like a house.
- **IPv4 (Internet Protocol version 4):** The older, standard way to give addresses. It uses numbers like `192.168.1.15`. The problem is that there are only about 4 billion of these, and we ran out!
- **IPv6 (Internet Protocol version 6):** The new version created to solve the shortage. It uses much longer addresses with letters and numbers (like `2001:0db8:85a3:0000:0000:8a2e:0370:7334`). This provides enough addresses for every device on Earth forever.

## Essential Network Commands
When using my Linux machine, I use these tools in the terminal:

- **`ping`:** This command acts like a sonar to see if a website or computer is online. Even cooler, I learned I can use it to find the IP address of a company! If I type `ping company.com` (like google or tryhackme), the terminal will show me the exact IP address behind that company's website.
- **`ifconfig`:** (Interface Configuration). I use this command to see my own computer's IP address and check if my network adapter is working properly. 

## Wireshark & The TCP 3-Way Handshake
**Wireshark** is a tool that lets me "sniff" or capture data packets flying through the network. 

I used Wireshark to watch a **TCP 3-Way Handshake** happen in real time. TCP is a reliable protocol, meaning it double-checks that connections are made properly. Here is what I saw:
1. **SYN (Synchronize):** My computer says "Hello, can we talk?"
2. **SYN-ACK (Synchronize-Acknowledge):** The server replies "Yes, I hear you! Let's talk."
3. **ACK (Acknowledge):** My computer replies "Great, I'm sending data now."

Only after those three steps does the actual data start transferring!
