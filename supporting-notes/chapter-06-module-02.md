# Chapter 6, Module 2 · Network Monitoring and Traffic Analysis

[Back to index](../README.md)

## Topics Covered

- Traffic baselines and indicators of compromise
- Flow, payload, and timing analysis
- PCAP and PCAPNG
- IPv4 and IPv6 headers
- Wireshark and tcpdump

## Study Notes

Compare observed hosts, ports, protocols, and timing with an established baseline. Flow metadata describes communication patterns. Packet captures provide protocol and header detail, and encryption can limit payload visibility. IPv4 TTL and IPv6 Hop Limit constrain packet lifetime. Wireshark display filters narrow the view of a capture. tcpdump can read an existing capture with `tcpdump -nn -r capture.pcap` and filter it with an expression such as `udp port 53`.

## Key Takeaways

- Unexpected traffic is a lead that needs supporting evidence.
- Preserve original captures and filter a working copy or display.
- Use direction, time, host identity, and protocol details to interpret a conversation.

## Source

Personal course notes in `Chapter 6 M 2.docx`.
