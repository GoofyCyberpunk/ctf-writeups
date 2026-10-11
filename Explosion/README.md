Hackthebox Lab: Explosion

Explosion is a very easy Windows machine that showcases the Remote Desktop Protocol (RDP), how to interact with it using the xfreerdp client and how improper configurations can allow unauthenticated access.

Task 1
What does the 3-letter acronym RDP stand for?

Answer: Remote Desktop Protocol
------------------------------------------
Task 2
What is a 3-letter acronym that refers to interaction with the host through a command line interface?

Answer: CLI
------------------------------------------
Task 3
What about graphical user interface interactions?

Answer: GUI
------------------------------------------
Task 4
What is the name of an old remote access tool that came without encryption by default and listens on TCP port 23?

Answer: telnet
------------------------------------------
Task 5
What is the name of the service running on port 3389 TCP?

doing: sudo nmap -p- -sS -sV <target_IP>
<Einfügen!Explosion-task5.png>

Answer: ms-wbt-server
------------------------------------------
Task 6
What is the switch used to specify the target host's IP address when using xfreerdp?

Answer: /v:
------------------------------------------
Task 7
What username successfully returns a desktop projection to us with a blank password?

Answer: administrator
------------------------------------------
