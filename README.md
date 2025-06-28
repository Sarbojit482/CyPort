## README for Simple Nmap Scanning Tool
This is a simple command-line tool using Python3 and nmap library to perform network scanning. The user can enter
an IP address, select from three types of scans (SYN Scan, UDP Scan, Comprehensive Scan) as input, then the
program uses nmap's functions to execute the scan and display the results.

## How to Use
1. Run this script in a terminal or command prompt with Python3 installed.
2. When prompted for an IP address, enter any valid IP address (ipv4).
3. You will then be given three options:
    - '1' for SYN Scan
    - '2' for UDP Scan
    - '3' for Comprehensive Scan
   Select one of the above by entering its corresponding number.
4. The program will start the scan and display the results after it completes. If a port is open, the service that
runs on that port and its state (open/closed) will be displayed along with the port number.
5. You can then repeat the process as many times as you like by simply running this script again.

## Dependencies
This program requires nmap library which should already installed if you are using Linux, or else install it via
pip: `pip3 install python-nmap`

The code is pretty straightforward and does not require any additional dependencies outside of the Python standard
library and the nmap package.

## Limitations & Known Issues
There could be an issue with running this script if you have more than one network interface on your machine, as
it might choose the wrong network to scan from. You can also run into issues if ports are not open or the IP
address is invalid. The nmap library doesn't handle these errors very gracefully and will throw a lot of warnings
and exception messages in such cases.
