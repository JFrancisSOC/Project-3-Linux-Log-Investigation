# Project 3 – Linux Log Investigation

## Objective

Develop practical Linux log analysis skills used by Security Operations Center (SOC) analysts by viewing, searching, and interpreting authentication logs within an Ubuntu virtual machine.

---

## Environment

* Ubuntu Desktop LTS
* Oracle VirtualBox
* Bash Terminal

---

## Skills Practiced

* Navigating Linux log directories
* Viewing authentication log files
* Reading the beginning and end of log files
* Searching log files using `grep`
* Identifying authentication events
* Understanding Linux authentication logs
* Recognizing normal authentication messages
* Basic log analysis during a security investigation

---

## Linux Commands Used

| Command                             | Purpose                                         |
| ----------------------------------- | ----------------------------------------------- |
| `ls /var/log`                       | Display available Linux log files               |
| `head /var/log/auth.log`            | View the beginning of the authentication log    |
| `tail /var/log/auth.log`            | View the most recent authentication log entries |
| `tail -n 20 /var/log/auth.log`      | Display the last 20 authentication log entries  |
| `grep "session" /var/log/auth.log`  | Search the log for authentication sessions      |
| `grep "Accepted" /var/log/auth.log` | Search for successful login events              |

---

## Lab Activities

During this project, I explored the Linux **/var/log** directory and analyzed the **auth.log** authentication log. I practiced viewing log files using **head** and **tail**, searched for authentication events using **grep**, and examined recent authentication messages to determine whether they represented normal system activity or events requiring additional investigation. This project introduced the basic log analysis techniques commonly used by SOC analysts during security investigations.

---

## Screenshots

* 01 Linux Log Setup
* 02 Viewing Auth Log with Head
* 03 Viewing Auth Log with Tail
* 04 Searching Auth Log with Grep
* 05 Identifying Successful Logins

---

## Lessons Learned

During this project, I learned how Linux stores authentication events in **auth.log** and how SOC analysts can quickly investigate those events using command-line tools. I practiced using **head**, **tail**, and **grep** to locate important authentication activity without manually reading an entire log file. I also learned that not every authentication-related message indicates malicious activity and that analysts should always investigate log entries within their proper context.

---

## SOC Analyst Takeaways

This project strengthened my understanding of Linux authentication logs and how they support security investigations. I learned how to locate important log files, review authentication events, search for specific login activity, and distinguish between normal operating system messages and events that may require additional investigation.


