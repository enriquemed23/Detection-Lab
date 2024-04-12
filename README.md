# Detection-Lab

## Objective
The Detection Lab project aimed to establish a controlled environment for simulating and detecting cyber attacks. The primary focus was to ingest and analyze logs within a Security Information and Event Management (SIEM) system, generating test telemetry to mimic real-world attack scenarios. This hands-on experience was designed to deepen understanding of network security, attack patterns, and defensive strategies.

### Skills Learned
- Advanced understanding of SIEM concepts and practical application.
- Proficiency in analyzing and interpreting network logs.
- Ability to generate and recognize attack signatures and patterns.
- Enhanced knowledge of network protocols and security vulnerabilities.
- Development of critical thinking and problem-solving skills in cybersecurity.

### Tools Used
- Security Information and Event Management (SIEM) system for log ingestion and analysis.
- Network analysis tools (such as Wireshark) for capturing and examining network traffic.
- Telemetry generation tools to create realistic network traffic and attack scenarios.

## Steps
Installing Sysmon. <br>
<img src="https://github.com/enriquemed23/Detection-Lab/blob/main/Sysmon install.PNG" height= 250 width =450 /> 
<img src="https://github.com/enriquemed23/Detection-Lab/blob/main/Sysmon confirmed.PNG" height= 250 width =450 /> <br> <br>
Installing Splunk. <br>
<img src="https://github.com/enriquemed23/Detection-Lab/blob/main/SplunkInstall.PNG" height= 250 width =450 /> 
<img src="https://github.com/enriquemed23/Detection-Lab/blob/main/SplunkConfirm.PNG" height= 250 width =450 /> <br> <br>
Add our inputs.conf file to allow Splunk to ingest Sysmon. Also, add the Sysmon Add App, this allows for much more extracted fields like parent process IDs. <br>
<img src="https://github.com/enriquemed23/Detection-Lab/blob/main/INputsMoved.PNG" height= 250 width =450 /> 
<img src="https://github.com/enriquemed23/Detection-Lab/blob/main/SplunkRestart.PNG" height= 250 width =450 /> 
<img src="https://github.com/enriquemed23/Detection-Lab/blob/main/SplunkLogsReceived.PNG" height= 250 width =450 /> 
<img src="https://github.com/enriquemed23/Detection-Lab/blob/main/Sysmon Splunk Add.PNG" height= 250 width =450 /> <br> <br>
Nmap Scan to see host is up and what is on it. Could use these ports in another lab. <br>
<img src="https://github.com/enriquemed23/Detection-Lab/blob/main/Nmapscan.PNG" height= 250 width =450 /> <br> <br>
Creating a payload that victim will download and execute from our attacker python server. 
