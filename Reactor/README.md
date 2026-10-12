UNSOLVED!

<img width="358" height="145" alt="Screenshot From 2026-10-12 19-23-07" src="https://github.com/user-attachments/assets/9dec7356-0ae1-427e-9d8b-96542da85bf2" />

About

Reactor is an easy-difficulty Linux machine built around a ReactorWatch nuclear-monitoring dashboard, a Next.js 15.0.3 / React 19.0.0 application exposed on port 3000. The stack is vulnerable to CVE-2025-55182, better known as React2Shell, an unsafe-deserialization flaw in React Server Components that grants unauthenticated remote code execution. Using a public proof-of-concept, we obtain a foothold as the low-privileged node service account. From there, we enumerate the application directory, recover a SQLite database containing user records, and crack an MD5 password hash to obtain valid SSH credentials for the engineer user. Privilege escalation abuses a root-owned monitoring service that was launched with the Node.js --inspect debugger flag bound to a local port. By tunnelling to that debug port and driving it through the V8 inspector protocol, we execute code as root and escalate to a full root shell.


Task 1
How many TCP ports are open on Reactor?

<img width="637" height="196" alt="Screenshot From 2026-10-12 19-24-20" src="https://github.com/user-attachments/assets/19b9f6b5-b877-4da1-bbaa-0bd1fcb756e6" />

Answer: 2

------------------------------------------
Task 2
Which JavaScript framework powers the web application running on port 3000?

Answer: Next.js

------------------------------------------
Task 3
Which critical CVE affecting React Server Components can be used to gain remote code execution?

Answer: CVE-2025-55182

------------------------------------------
