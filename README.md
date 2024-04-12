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
- Splunk, a Security Information and Event Management (SIEM) system for log ingestion and analysis.
- System Monitor, a system service created to enhance logging and monitoring capabilities
- Metasploit framework, open-source penetration testing and exploitation toolkit

## Steps
Installing Sysmon. <br>
<img src="https://github.com/enriquemed23/Detection-Lab/blob/main/Sysmon install.PNG"  /> 
<img src="https://github.com/enriquemed23/Detection-Lab/blob/main/Sysmon confirmed.PNG" /> <br> <br>
Installing Splunk. <br>
<img src="https://github.com/enriquemed23/Detection-Lab/blob/main/SplunkInstall.PNG"  /> 
<img src="https://github.com/enriquemed23/Detection-Lab/blob/main/SplunkConfirm.PNG" /> <br> <br>
Add our inputs.conf file to allow Splunk to ingest Sysmon. Also, add the Sysmon Add App, this allows for much more extracted fields like parent process IDs. <br>
<img src="https://github.com/enriquemed23/Detection-Lab/blob/main/INputsMoved.PNG"  /> 
<img src="https://github.com/enriquemed23/Detection-Lab/blob/main/SplunkRestart.PNG"  /> 
<img src="https://github.com/enriquemed23/Detection-Lab/blob/main/SplunkLogsReceived.PNG"  /> 
<img src="https://github.com/enriquemed23/Detection-Lab/blob/main/Sysmon Splunk Add.PNG"  /> <br> <br>
Nmap Scan to see host is up and what is on it. Could use these ports in another lab. <br>
<img src="https://github.com/enriquemed23/Detection-Lab/blob/main/Nmapscan.PNG"  /> <br> <br>
Creating a payload that victim will download and execute from our attacker python server. <br>
<img src="https://github.com/enriquemed23/Detection-Lab/blob/main/Payload.PNG"  /> 
<img src="https://github.com/enriquemed23/Detection-Lab/blob/main/Handler.PNG"  />
<img src="https://github.com/enriquemed23/Detection-Lab/blob/main/pythonserver.PNG" />
<img src="https://github.com/enriquemed23/Detection-Lab/blob/main/download.PNG" /> <br> <br>
After malware is executed, it generates a shell and I ran these commands. <br>
<img src="https://github.com/enriquemed23/Detection-Lab/blob/main/shell and commands.PNG"  /> <br><br>
Back to splunk to see what happened. First we follow the IP and then we trace it to the file. From there we check the eventcodes that go with that file. We follow the Parent Process GUID to see the commands that we ran.   <br> 
<img src="https://github.com/enriquemed23/Detection-Lab/blob/main/SearchKalibox.PNG" />
<img src="https://github.com/enriquemed23/Detection-Lab/blob/main/SearchFamilyPicture.PNG"  />
<img src="https://github.com/enriquemed23/Detection-Lab/blob/main/familyeventcode1.PNG" />
<img src="https://github.com/enriquemed23/Detection-Lab/blob/main/eventcode1.PNG"  />
<img src="https://github.com/enriquemed23/Detection-Lab/blob/main/Busted.PNG"  />
