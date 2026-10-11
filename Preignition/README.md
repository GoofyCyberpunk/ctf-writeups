<img width="502" height="150" alt="Preignition" src="https://github.com/user-attachments/assets/eab31af5-8ccd-4ade-9544-337346ac6b75" />

About

Preignition is a very easy Linux machine which explores beginner enumeration and directory fuzzing of web applications. Upon finding a vulnerable Admin login endpoint, the web app showcases the dangers of improper configuration and default credentials.

Task 1

Directory Brute-forcing is a technique used to check a lot of paths on a web server to find hidden pages. Which is another name for this? (i) Local File Inclusion, (ii) dir busting, (iii) hash cracking.

Answer: dir busting

-------------------------------------------
Task 2

What switch do we use for nmap's scan to specify that we want to perform version detection?

Answer: sV

-------------------------------------------
Task 3

What does Nmap report is the service identified as running on port 80/tcp?

Answer: http

-------------------------------------------
Task 4

What server name and version of service is running on port 80/tcp?

Answer: nginx 1.14.2

-------------------------------------------
Task 5

What switch do we use to specify to Gobuster we want to perform dir busting specifically?

Answer: dir

-------------------------------------------
Task 6
When using gobuster to dir bust, what switch do we add to make sure it finds PHP pages?

Answer: -x php

-------------------------------------------
Task 7
What page is found during our dir busting activities?

doing: gobuster dir -u <target_IP> -w /usr/share/seclists/Discovery/Web-Content/DirBuster-2007_directory-list-2.3-small.txt -x php

<img width="1236" height="454" alt="Preignition-gobuster-task-7-8" src="https://github.com/user-attachments/assets/428ed895-57bb-4837-a842-953c57d42353" />


Answer:admin.php

-------------------------------------------
Task 8
What is the HTTP status code reported by Gobuster for the discovered page?

<img width="1236" height="454" alt="Preignition-gobuster-task-7-8" src="https://github.com/user-attachments/assets/740dbb24-f4d7-47ab-a61d-57ff6c31625c" />


Answer: 200

-------------------------------------------

After logging on the webpage wirh default credentials admin:admin i got the flag!

<img width="1045" height="358" alt="Preignition-root-flag" src="https://github.com/user-attachments/assets/e72c8c4e-e5af-444c-9382-2a295ddb878d" />


Submit the flag located in the webpage.

<img width="648" height="534" alt="Preignition-solved" src="https://github.com/user-attachments/assets/5039fd39-7d4e-4c05-a4ab-a7613340077a" />

