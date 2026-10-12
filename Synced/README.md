<img width="353" height="139" alt="Synced" src="https://github.com/user-attachments/assets/52a146f7-443a-4c47-8074-5017a227ca88" />

About

Synced is a very easy Linux machine that explores the Rsync protocol, how to interact with it and the dangers of improper configuration allowing anonymous authentication.

Task 1
What is the default port for rsync?

sudo nmap -p- -sV -sS <target_IP>

<img width="817" height="253" alt="Synced-scan" src="https://github.com/user-attachments/assets/98843e2e-ff8e-4055-b269-aa15a307fbd5" />

Answer: 873

----------------------------------------------
Task 2
How many TCP ports are open on the remote host?

sudo nmap -p- -sV -sS <target_IP>

<img width="817" height="253" alt="Synced-scan" src="https://github.com/user-attachments/assets/98843e2e-ff8e-4055-b269-aa15a307fbd5" />

Answer: 1

----------------------------------------------
Task 3
What is the protocol version used by rsync on the remote machine?

sudo nmap -p- -sV -sS <target_IP>

<img width="817" height="253" alt="Synced-scan" src="https://github.com/user-attachments/assets/98843e2e-ff8e-4055-b269-aa15a307fbd5" />

Answer: 31

----------------------------------------------
Task 4
What is the most common command name on Linux to interact with rsync?


Answer: rsync

----------------------------------------------
Task 5
What credentials do you have to pass to rsync in order to use anonymous authentication? anonymous:anonymous, anonymous, None, rsync:rsync 

Answer: None

----------------------------------------------
Task 6
What is the option to only list shares and files on rsync? (No need to include the leading -- characters)

rsync --list-only <target_IP>::
<img width="737" height="53" alt="Screenshot From 2026-10-12 14-32-01" src="https://github.com/user-attachments/assets/795d38a6-a1e6-452a-9a9c-1691c0216c7a" />


Answer: --list-only

----------------------------------------------
Submit the flag located on the share.

rsync --list-only 10.129.18.113::public

<img width="735" height="75" alt="Screenshot From 2026-10-12 14-34-19" src="https://github.com/user-attachments/assets/dc793469-e781-415b-be48-0d1ebed7bbca" />

rsync 10.129.18.113::public/flag.txt flag.txt

<img width="729" height="45" alt="Screenshot From 2026-10-12 14-35-20" src="https://github.com/user-attachments/assets/676f6671-ffa6-4db8-8758-fbdf14bfc59f" />

Copy flag to local machine

<img width="794" height="49" alt="Get-flag" src="https://github.com/user-attachments/assets/d94c4ddc-9ba7-4ea0-acf5-782903b0840c" />

cat flag.txt

<img width="642" height="546" alt="Synced-solved" src="https://github.com/user-attachments/assets/1b77f2dd-95bc-4b7a-aa7d-3ac44129e561" />

