# Task 5: Capture and Analyze Network Traffic Using Wireshark

## 🎯 Objective
Capture live network packets using Wireshark and identify basic protocols and traffic types.

## 🛠️ Tools Used
- [Wireshark](https://www.wireshark.org/) (Free and Open Source)

## 📝 Steps Followed

1. Installed Wireshark on my system.
2. Launched Wireshark and selected the **wlan0** for capturing packets.
3. Performed the following actions to generate traffic:
   - Opened a web browser and visited [vulnweb.php](http://testphp.vulnweb.com/).
   - Pinged `google.com` using the terminal.
4. Stopped the capture after approximately one minute.
5. Applied filters to inspect specific protocols such as:
   - `http`
   - `dns`
   - `tcp`
6. Identified and documented at least **three different protocols** found in the traffic.
7. Exported the capture as a `.pcap` file (`network_capture.pcap`).

## 📦 Deliverables

- `network_capture.pcap`: The raw packet capture file.
- `protocol_summary.md`: A short report listing and explaining identified protocols and example packets.

## 📊 Protocols Identified

| Protocol | Description                            | Example Usage                           |
|----------|----------------------------------------|-----------------------------------------|
| HTTP     | HyperText Transfer Protocol            | Browsing web pages                      |
| DNS      | Domain Name System                     | Resolving domain names to IPs           | 
| TCP      | Transmission Control Protocol          | Reliable transmission of packets        |
| ARP      | Address Resolution Protocol            | Resolving IP addresses to MAC addresses |
## ✅ Outcome

Gained hands-on experience in:
- Capturing live traffic using Wireshark.
- Filtering packets using protocol-based filters.
- Understanding the role of each protocol in network communication.
## Here are some screen shots of the above
![Screenshot 2025-06-06 200640](https://github.com/user-attachments/assets/5ed25911-05e2-4ee4-89b0-f511f2b5bd85)
![Screenshot 2025-06-06 200656](https://github.com/user-attachments/assets/b646f0b7-ec86-437a-8c6f-c0544746503c)
![Screenshot 2025-06-07 004506](https://github.com/user-attachments/assets/1d3aa39b-84a5-42cd-a4ed-460070375a8f)




