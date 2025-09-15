# Homelab-Attack-Detection

## Objective

This Homelab Attack Detection lab project enabled me to establish an environment for simulating and detecting attacks. This project was primarily focused on generating and analyzing logs within the Security Information and Event Management (SIEM) to mimic scenarios that could happen during real attacks. This Experience allowed me to design, implement, and gain an advanced understanding of how attackers exploit unsecure networks and what strategies can be used to defend against them.

### Skills Learned


- Implementation and deployment of a SIEM for practical use
- Proficiency in analyzing and interpreting network logs.
- Strengthened understanding of attacks and defending a machine to provide security
- Enhanced knowledge of network protocols and security vulnerabilities.
- Development of critical thinking and problem-solving skills in cybersecurity.

### Tools Used

- Security Information and Event Management (SIEM), like Splunk, for log analysis and incident response building.
- Reconnaissance tools like NMAP to find open ports and vulnerabilities to exploit and experiment on.
- Telemetry generation tools like Sysmon to create network traffic that is similar to real-world scenarios.

## Steps
<img width="1920" height="966" alt="Kali-NMAP" src="https://github.com/user-attachments/assets/d28172aa-7da2-432b-bc24-23bfb8a1c18d" />
Kali Linux: Ran NMAP to find vulnerabilities within the defender system.

<img width="1920" height="966" alt="Kali-Metasploit" src="https://github.com/user-attachments/assets/e6cf8416-9ed7-4eb6-9650-d4f64c5591e8" />
Kali Linux: Created the file that will have the payload within it.

<img width="1920" height="966" alt="Kali-Payload" src="https://github.com/user-attachments/assets/57f4ad21-ca07-4860-8559-ac82213eca13" />
Kali Linux: Configured the Payload in Metasploit to the correct selected payload. We created the file with Metasploit

<img width="1920" height="966" alt="Kali-Exploit" src="https://github.com/user-attachments/assets/25f9e843-4c8b-4adf-8360-02e5eea9a4f7" />
Kali Linux: Once we set the local host, we launched the attack using the command 'exploit'

<img width="1920" height="966" alt="KALI-PythonServer" src="https://github.com/user-attachments/assets/3cea3df7-b825-45e7-aab2-8245d69ca3b7" />
Kali Linux: However, since it's a downloadable file, we needed a Python server, so I created one so the defender machine could download the file.


<img width="1024" height="768" alt="Windows-virus" src="https://github.com/user-attachments/assets/30ac146c-5d60-4c15-9869-7fecc35ae21a" />
Windows: After configuring the Python server, on the defender server, we head to the server we set up and downloaded the file.
<img width="1920" height="966" alt="Kali-Connectionestablished" src="https://github.com/user-attachments/assets/5c5ec46d-d505-495c-a79a-9d0aea33c148" />
Kali Linux: After running the file on the defender machine, we connected to the machine and were able to run commands like Shell, and then utilize commands to exploit the system.
<img width="1024" height="768" alt="endpoint" src="https://github.com/user-attachments/assets/38f13c98-efc6-4c33-becb-04e4bced8a4c" />
Windows: After the connection is confirmed, we went into Splunk and ensured we created an index named endpoint. This allows us to view the log traffic on our system.
<img width="1024" height="768" alt="WINDOWS-LOGS" src="https://github.com/user-attachments/assets/cf8de96b-ed3b-4820-a957-f5b86089939a" />
Windows: After creating the index, we were able to go to Search and Reporting and enter 'index = endpoint'. This will show you the logs from your system. 
<img width="1024" height="768" alt="EventID1" src="https://github.com/user-attachments/assets/49d2becb-3eba-46f1-8c63-00c16323bc75" />
<img width="1024" height="768" alt="more logs" src="https://github.com/user-attachments/assets/68f2c820-98f6-47fd-9d18-9d18e36d8714" />
Windows: We are able to view event IDs and logs of what happened on our system, and we can search by which file did what. In this case, the resume.pdf.exe led to Shell being used.

