# SOC Automation Lab

## Objective

The SOC Automation lab aims to automate a Security Operations Center (SOC) that streamlines event monitoring, alerting, and incident response. By leveraging powerful tools such as Wazuh, TheHive, and Shuggle, you can create an efficient and resilient SOC. This lab was inspired by the Youtube Channel <a href="https://www.youtube.com/MyDFIR">MyDFIR</a>. 

![Wazuh](https://github.com/user-attachments/assets/50e06c6b-8ca4-4d46-b630-faf67cfe7df7)


## Tools Used

- Wazuh: An open-source cyber security platform that integrates SIEM and XDR capablities in a unique solution.
- Shuffle: An open-source automation platform designed to streamline and automate workflows within SOCs.
- TheHive: An open-source incident response and case management platform.
- VirusTotal: An online service that provides tools for analyzing files, URLs, domains, and IP addresses for potential security threats.


## Step-by-Step Guide:

## Windows Client Set Up

1. Install <a href="https://www.microsoft.com/en-ca/software-download/windows10ISO">Windows 10</a> on VirtualBox
- If you haven't already, download <a href="https://www.virtualbox.org/">VirtualBox</a> or your preferred Virtual Machine
2. Install <a href="https://learn.microsoft.com/en-us/sysinternals/downloads/sysmon">Sysmon</a> as well as <a href="https://github.com/olafhartong/sysmon-modular/blob/master/sysmonconfig.xml">Sysmon's Configuration File</a>

![sysmon git](https://github.com/user-attachments/assets/b9d900d1-ad9a-4a4e-8e64-83191e12ee15)

- Extract Sysmon zip file
- Open PowerShell as administrator
   - Change directory into the file path 
      - Run: cd (Paste the file path of the extracted directory here)
      - ex. cd C:\Users\hacki\Downloads\Sysmon 
   - Run: .\Sysmon64.exe -i ..\sysmonconfig.xml
      - -i flag indicates that we want to specify a configuration file
      - ../ allows us to go back one directory 
         - sysmon config file is locaed under downloads directory so ../ will allow us to do that
   - Hit "Enter"
   - Select "Agree" to install Sysmon
   - Screen will display "Sysmon64 started"
   - Close PowerShell


## Install & Configure Wazuh

## SetUp TheHive

## Configure Wazuh Dashboard

## Integrate SOAR


## References & Resources:

- <a href="https://www.youtube.com/@mydfir">MyDFIR</a>
- <a href="https://learn.microsoft.com/en-us/sysinternals/downloads/sysmon">Sysmon Documentation</a>
