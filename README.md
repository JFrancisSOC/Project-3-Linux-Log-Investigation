# Project 3 – Linux Log Investigation

## Objective

* Develop practical Linux log analysis skills used by Security Operations Center (SOC) analysts by viewing, searching, and interpreting Linux authentication logs within an Ubuntu virtual machine.

---

## Environment

* Ubuntu Desktop LTS
* Oracle VirtualBox
* Bash Terminal

---

## Skills Practiced

* Navigating Linux log directories
* Viewing Linux authentication logs
* Reading log files using `head`
* Reading log files using `tail`
* Viewing large log files using `less`
* Searching log files using `grep`
* Identifying authentication events
* Performing basic Linux log analysis

---

## Linux Commands Used

| Command                             | Purpose                                         |
| ----------------------------------- | ----------------------------------------------- |
| `ls /var/log`                       | Display available Linux log files               |
| `head /var/log/auth.log`            | View the beginning of the authentication log    |
| `tail /var/log/auth.log`            | View the most recent authentication log entries |
| `tail -n 20 /var/log/auth.log`      | Display the last 20 authentication log entries  |
| `less /var/log/auth.log`            | Scroll through large log files                  |
| `grep "session" /var/log/auth.log`  | Search for authentication session activity      |
| `grep "Accepted" /var/log/auth.log` | Search for successful login events              |

---

## Lab Activities

* Explored the Linux `/var/log` directory.
* Located the `auth.log` authentication log.
* Used `head` to examine the beginning of the log.
* Used `tail` to review the newest authentication events.
* Used `less` to scroll through a large log file.
* Used `grep` to search for authentication-related events.
* Reviewed Linux authentication messages to determine whether they represented normal system activity or events requiring additional investigation.

---

## Screenshots

* P3 01 Linux Log Setup
* P3 02 Viewing Auth Log with Head
* P3 03 Viewing Auth Log with Tail
* P3 04 Searching Auth Log with Grep
* P3 05 Identifying Successful Logins
* P3 06 Authentication Activity

---

## Lessons Learned

* I learned how Linux stores authentication events inside the `auth.log` file.
* I practiced using `head`, `tail`, `less`, and `grep` to investigate authentication activity.
* I learned that not every authentication-related log entry indicates malicious activity and that each event should be reviewed within its proper context.

---

## SOC Analyst Takeaways

* Authentication logs are one of the first places SOC analysts look during an investigation.
* Linux command-line tools make it possible to quickly search and analyze large log files.
* Reviewing both successful and failed authentication events helps determine whether unauthorized access may have occurred.
