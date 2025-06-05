# Active-Directory-Project

This project establishes a comprehensive virtual cybersecurity lab using Oracle VM VirtualBox, featuring Windows 10, Kali Linux, Windows Server 2022, and Ubuntu Server virtual machines. The lab environment is configured with NAT networking to ensure seamless IP-based communication among all systems.

## daigram
![image](https://github.com/user-attachments/assets/7e2c7421-4a0c-4645-baa3-26782e4427d7)


## Skills Learned
- Setting up VMs (Windows 10, Kali Linux, Windows Server, Ubuntu Server) in Oracle VM VirtualBox.
- Configuring IP addresses, NAT Networks for VMs.
- Troubleshooting network connectivity (ping, DNS settings).
- Installing Splunk Server and Universal Forwarder.
- Installing Sysmon for endpoint monitoring.
- Using Crowbar for brute force attacks.
- Using Atomic Red Team (ART) to simulate tests.
- Analyzing security logs (event codes 4625, 4624) in Splunk.
- Joining Windows machines to a domain.
- Enabling Remote Desktop on Windows.
- PowerShell scripting for tasks (Invoke-WebRequest, Set-ExecutionPolicy).

## Tools Used
- Oracle VM VirtualBox Manager: For creating and managing virtual machines (VMs).
- Splunk Server: For log analysis and monitoring.
- Splunk Universal Forwarder: For data forwarding to Splunk.
- Sysmon: Endpoint monitoring on Windows machines.
- Crowbar: Used to simulate brute force attacks.
- Atomic Red Team (ART): Used for security testing and validation.
- PowerShell: For scripting and automation tasks.
- Microsoft Windows Event Logs: Analyzed in Splunk for security monitoring.
- Windows Server 2022: Operating system used for Active Directory Domain Services setup.
- Ubuntu Server: Used as a Splunk server in the lab setup.
- Microsoft Windows 10: Operating system for target machine in the lab.
- Kali Linux: Used as an attacker machine in the lab setup.

# Steps
## Lab Components

| Component       | Description                              |
|----------------|------------------------------------------|
| Windows Server | Domain Controller (`demodomain.local`)  |
| Windows 10     | Target PC joined to domain               |
| Kali Linux     | Attacker machine (Crowbar)              |
| Ubuntu Server  | Splunk Enterprise for log analysis      |

## Network Configuration

- NAT Network: `192.168.10.0/24`
- Ubuntu (Splunk): `192.168.10.10`
- Windows Server: `192.168.10.7`
- Windows 10: `192.168.10.100`
- Kali Linux: `192.168.10.250`

  ## Usage

1. Set up and install all VMs with specified IPs.
2. Configure Splunk and forwarders.
3. Join Windows 10 to the domain.
4. Simulate attacks via Kali (Crowbar) and ART.
5. Analyze logs and detection patterns in Splunk.

## Conclusion
With the conclusion of the last part of this walk-through, you should have a successful setup and communication between 4 Virtual Machines: Windows 10 Target Machine, Kali Linux Attacker Machine, Splunk, and Windows Servers. You should be able to view events with Splunk, test Splunk functionality and defense using Crowbar brute force password cracker, and more.
  
