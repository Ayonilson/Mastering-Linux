# Linux Fundamentals Project

This project documents practical exercises completed as part of a **Linux Fundamentals Project** using Kali Linux. It covers basic Linux system identification, resource inspection, network connectivity testing, IP address resolution, and an introduction to understanding ping results.

## Table of Contents
- [Project Overview](#project-overview)
- [Configuration Steps](#configuration-steps)
- [Results and Findings](#results-and-findings)
- [Author](#author)

## Project Overview

The purpose of this project is to develop foundational knowledge of Linux operating systems and basic networking commands through hands-on exercises in Kali Linux.

The assignment focuses on identifying system information, checking available system resources, testing network connectivity using `ping`, and examining how domain names resolve to IP addresses.

The key objectives are to:
- Identify the machine hostname, current directory, and logged-in user.
- Check available virtual machine memory and disk space.
- Identify the installed Kali Linux kernel version.
- Test network connectivity and observe packet loss and round-trip time.
- Resolve Google's domain name to an IP address.
- Understand the difference between pinging an IP address and a domain name.

## Operating System Software

The assignment was performed using **Kali Linux**, a Linux distribution commonly used for cybersecurity education and security testing.

### System Information

- **Machine Name (Hostname):** Kali
- **Current Directory:** `/home/kali`
- **Logged-in User:** `kali`
- **Operating System:** Kali Linux
- **Kernel Version:** `Linux Kali 6.19.14+kali-amd64`
- **Virtual Machine RAM:** 1.9 GB
- **Available Disk Space:** 953 MiB

### Linux Commands Used

| Command | Purpose |
|---|---|
| `hostname` | Displays the machine's hostname. |
| `pwd` | Displays the current working directory. |
| `whoami` | Identifies the currently logged-in user. |
| `free -h` | Displays memory usage in a human-readable format. |
| `df -h` | Displays filesystem disk space usage. |
| `uname -r` | Displays the running Linux kernel version. |
| `ping -c 2 8.8.8.8` | Sends two ICMP echo requests to Google's public DNS IP address. |
| `ping -c 4 google.com` | Sends four ICMP echo requests to Google's domain name. |

### Network Test Results

- **IP Address Tested:** `8.8.8.8`
- **Domain Tested:** `google.com`
- **Resolved IP Address:** `172.217.76.139`
- **Average Round-Trip Time (First Test):** 1003 ms
- **Average Round-Trip Time (Second Test):** 3005 ms
- **Packet Loss:** No packet loss reported in the first test.
- **Ping Count:** 2 packets for the IP address test and 4 packets for the domain test.

The recorded results reflect the observations documented during the assignment.

## Tools and Technologies

- **Kali Linux:** Linux operating system used for the practical exercises.
- **Linux Terminal:** Command-line interface used to execute commands and inspect system information.
- **Virtual Machine:** Virtualized environment in which Kali Linux was running.
- **Ping Utility:** Network diagnostic tool used to test connectivity and measure round-trip time.
- **ICMP:** Protocol used by the ping utility to send echo requests and receive echo replies.
- **DNS (Domain Name System):** System used to resolve domain names such as `google.com` into IP addresses.
- **Google Public DNS IP:** `8.8.8.8`, used as the destination for a connectivity test.

## Configuration Steps

1. **Identify the machine hostname.**

   Execute the following command to display the machine name:

   ```bash
   hostname
   ```

   The recorded hostname was `Kali`.

2. **Check the current working directory.**

   Run:

   ```bash
   pwd
   ```

   The recorded current directory was `/home/kali`.

3. **Identify the logged-in user.**

   Execute:

   ```bash
   whoami
   ```

   The command identified the user as `kali`.

4. **Inspect the virtual machine's memory and disk space.**

   Use the following commands to examine available system resources:

   ```bash
   free -h
   df -h
   ```

   The assignment recorded 1.9 GB of virtual machine RAM and 953 MiB of available disk space.

5. **Check the Linux kernel version.**

   Run:

   ```bash
   uname -r
   ```

   The recorded system version was `Linux Kali 6.19.14+kali-amd64`.

6. **Test network connectivity to an IP address.**

   Execute:

   ```bash
   ping -c 2 8.8.8.8
   ```

   The command sends two ICMP echo requests to `8.8.8.8`. The assignment recorded an average round-trip time of 1003 ms and no packet loss.

7. **Test connectivity to Google's domain name.**

   Run:

   ```bash
   ping -c 4 google.com
   ```

   The command sends four ICMP echo requests to the hostname `google.com`. The assignment recorded the resolved IP address as `172.217.76.139` and a round-trip time of 3005 ms.

8. **Compare the ping results.**

   Review the output from both tests to observe the differences in packet counts, response times, and destination formats.

   The first test used an IP address directly, while the second used a domain name that required DNS resolution if the result was not already cached.

9. **Document the findings.**

   Record the system information, commands executed, network test results, and relevant screenshots as evidence of the completed practical exercises.

## Results and Findings

The assignment demonstrated basic Linux system administration and introductory network troubleshooting skills.

### Key Findings

- **System Identification:** Successfully identified the Kali Linux hostname, current directory, and logged-in user.
- **Resource Inspection:** Recorded the virtual machine's RAM allocation and available disk space.
- **Kernel Identification:** Documented the Kali Linux kernel version as `6.19.14+kali-amd64`.
- **Network Connectivity:** Successfully conducted a ping test to `8.8.8.8`, with no packet loss reported in the assignment.
- **DNS Resolution:** Recorded Google's resolved IP address as `172.217.76.139`.
- **Round-Trip Time Comparison:** Observed different response-time values between the two ping tests.
- **Packet Count:** Learned that the `-c` option specifies the number of ping packets to send. For example, `-c 4` sends four requests and then stops.

### Lessons Learned

- Linux commands provide useful information about the operating system, user session, and available resources.
- The `ping` utility helps test network reachability and measure round-trip time.
- Domain names can be resolved into IP addresses through DNS.
- The `-c` option limits the number of ICMP echo requests sent by the ping utility.
- Differences in measured ping times may result from network conditions, routing, destination behavior, and the number of packets sent. The recorded results alone do not establish the cause of the difference.

This project provided practical experience with Linux command-line operations and basic networking concepts, building a foundation for further study in **networking, system administration, and cybersecurity**.

## Author

**Adeayo Aladebo**

- **Field:** Networking, IT, and Cybersecurity
- **Operating System:** Kali Linux
- **Project:** Linux Fundamentals Assignment

**GitHub:** Add your GitHub profile URL here.

**Email:** reycoba2@yahoo.com.
