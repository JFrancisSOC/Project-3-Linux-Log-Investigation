Project 3 – Linux Log Investigation
Objective

Develop practical Linux log analysis skills used by Security Operations Center (SOC) (SOC) analysts by viewing, searching, and interpreting Linux authentication logs within an Ubuntu virtual machine.

Environment
Ubuntu Desktop LTS
Oracle VirtualBox
Bash Terminal
Skills Practiced
Navigating Linux log directories
Viewing Linux authentication logs
Reading log files using head
Reading log files using tail
Searching log files using grep
Reviewing authentication events
Recognizing normal authentication activity
Performing basic Linux log analysis
Linux Commands Used
Command	Purpose
ls /var/log	Display available Linux log files
head /var/log/auth.log	View the beginning of the authentication log
tail /var/log/auth.log	View the end of the authentication log
tail -n 20 /var/log/auth.log	Display the last 20 log entries
grep "session" /var/log/auth.log	Search for authentication sessions
grep "Accepted" /var/log/auth.log	Search for successful login events
less /var/log/auth.log	Scroll through large log files
Lab Activities

During this project, I explored the Linux /var/log directory and analyzed the auth.log authentication log. I practiced viewing log files using head, tail, and less, and searched for authentication events using grep. I reviewed recent authentication messages, identified normal authentication activity such as root session events, and learned how Linux log files are used during security investigations.

Screenshots
P3 01 Linux Log Setup
P3 02 Viewing Auth Log with Head
P3 03 Viewing Auth Log with Tail
P3 04 Searching Auth Log with Grep
P3 05 Identifying Successful Logins
P3 06 Authentication Activity
Lessons Learned

During this project, I learned how Linux stores authentication events inside the auth.log file and how command-line tools can be used to quickly investigate those events. I practiced using head, tail, less, and grep to review authentication activity without manually reading an entire log file. I also learned that not every authentication-related message indicates malicious activity and that analysts should always investigate log entries within their proper context before making conclusions.

SOC Analyst Takeaways

This project strengthened my understanding of Linux authentication logs and their importance during security investigations. I learned how to locate important log files, search for authentication events, review login activity, and distinguish between normal operating system messages and events that may require additional investigation. These are foundational skills used by SOC analysts during incident response and threat investigations.
