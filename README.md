# Project 3 – Linux Log Investigation

## Objective

- Build practical skills in Linux log analysis, focusing on reviewing and interpreting authentication logs—an essential task for SOC analysts during incident investigations.

---

## Environment

- Ubuntu Desktop LTS
- Oracle VirtualBox
- Bash Terminal

---

## Skills Practiced

- Navigating log directories in Linux
- Viewing and searching Linux authentication logs
- Using commands like head, tail, less, and grep
- Identifying normal vs. suspicious login events
- Analyzing patterns in log files for potential threats

---

## Linux Commands Used

| Command                             | Purpose                                                |
|-------------------------------------|--------------------------------------------------------|
| `ls /var/log`                       | List log files in the system directory                 |
| `head /var/log/auth.log`            | View the beginning of the authentication log           |
| `tail /var/log/auth.log`            | View the latest entries in the authentication log      |
| `tail -n 20 /var/log/auth.log`      | Show the last 20 log entries                           |
| `less /var/log/auth.log`            | Scroll through a large log file interactively          |
| `grep "session" /var/log/auth.log`  | Search for session-related log entries                 |
| `grep "Accepted" /var/log/auth.log` | Find successful login attempts                         |

---

## Lab Activities

- Navigated to the `/var/log` directory to explore system logs.
- Located and examined the `auth.log` file, which records all authentication attempts.
- Used `head` to see initial log entries.
- Used `tail` to monitor the most recent authentication attempts.
- Scrolled through large logs with `less` to spot patterns.
- Used `grep` to find specific events like successful logins and session activity.
- Differentiated between normal log entries and suspicious patterns requiring deeper investigation.

---

## Screenshots

### 01 – Log Directory Exploration
![Log Directory Exploration](01%20Linux%20Log%20Setup.png)

### 02 – Viewing Auth Log with Head
![Viewing Auth Log with Head](02%20Viewing%20Auth%20log%20with%20Head.png)

### 03 – Viewing Auth Log with Tail
![Viewing Auth Log with Tail](03%20Viewing%20Auth.log%20with%20tail.png)

### 04 – Scrolling Auth Log with Grep
![Scrolling Auth Log with Grep](04%20Searching%20Auth%20log%20With%20grep.png)

### 05 – Identifying Successful Logins
![Identifying Successful Logins](05%20Identifying%20Successful%20Logins.png)

### 06 – Authentication Activity
![Authentication Activity](06%20Authentication%20Activity.png)
---

## Lessons Learned

- I learned how authentication events are logged in Linux, providing a record of all login attempts.
- I practiced using tools like head, tail, less, and grep to efficiently sift through large log files.
- I realized that not every login attempt is suspicious—context matters, and I improved my ability to spot patterns that may indicate a threat.

---

## SOC Analyst Takeaways

- Reviewing authentication logs is one of the first steps in SOC investigations—these logs help identify unauthorized access attempts.
- Command-line tools like grep and tail allow you to quickly pinpoint important events, saving time during real incident analysis.
- Understanding the flow of log entries helps analysts distinguish between normal user behavior and potential security incidents that need further action.
