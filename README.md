# Windows_Sysmon_IDs

This repository contains a series of notebooks designed to develop my understanding of Windows Event IDs and Sysmon IDs and their use in detecting suspicious activity. As part of my self-directed learning journey in cybersecurity, these notebooks focus on key aspects of event log analysis; including identification, visualisation, and alerting, to help develop detection skills using native Windows logging data.

<b>Event ID Identification and Short Explanation</b><br>
    - Parses a log file to extract unique Windows Event IDs<br>
    - Uses the `BeautifulSoup` library to scrape event definitions from the <a href="https://www.ultimatewindowssecurity.com/securitylog/encyclopedia/">Ultimate IT Security Encyclopedia</a><br>
    - Presents a list of the Event IDs found, along with their corresponding meanings<br>
    - Helps build foundational understanding of what each Event ID represents in the context of security monitoring<br>

<b>Event Volume Visualisation</b><br>
    - Visualises overall event hit volume in 15-minute intervals using `matplotlib`<br>
    - Enables interactive exploration with `ipywidgets` to drill down and inspect specific Event IDs<br>
    - Example output highlights the count of Event IDs 8 (Create Remote Thread), 29 (File Executable Detected), 4648 (Explicit Credential Logon), and 4732 (A member was added to a security-enabled group)<br>

<b>Suspicious Event Alert</b><br>
    - Analyses Windows Event and Sysmon logs to detect and alert on potential security incidents<br>
    - Parses a log file and flag suspicious events<br>
    - Example alerts includes Privilege escalation attempts, Command line execution for network discovery and file transfer, Executable file creation, and Possible process injection
