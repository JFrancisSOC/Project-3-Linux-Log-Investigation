Objective

Develop foundational Linux log analysis skills by viewing, searching, and interpreting authentication logs commonly used during Security Operations Center (SOC) investigations.

Environment
Ubuntu Desktop LTS
Oracle VirtualBox
Bash Terminal
Skills Practiced
Navigating Linux log directories
Viewing log files
Reading the beginning and end of log files
Searching logs for specific keywords
Identifying authentication events
Understanding basic Linux log analysis
Linux Commands Used
Command	Purpose
ls /var/log	List available log files
head /var/log/auth.log	View the first lines of the authentication log
tail /var/log/auth.log	View the most recent log entries
grep "Session" /var/log/auth.log	Search the authentication log for matching text
Lab Activities

During this mission, I explored the Linux /var/log directory and examined the auth.log file. I used the head command to review the beginning of the authentication log and the tail command to inspect the most recent login activity. I also used grep to search the log for specific authentication events, demonstrating how Linux log files can be filtered during a security investigation.

Screenshots
P3 01 Linux Log Setup
P3 02 Viewing Auth Log with Head
P3 03 Viewing Auth Log with Tail
P3 04 Searching Auth Log with Grep
SOC Analyst Takeaways

This project introduced me to one of the most important responsibilities of a SOC analyst: reviewing authentication logs. I learned how to quickly locate and examine log files, identify login activity, and search large log files for specific events using grep. These skills are essential for investigating failed login attempts, unauthorized access, and other security-related events on Linux systems.

Next Mission

Mission 4 – Linux File Permissions & User Management

Topics:

chmod
chown
whoami
id
groups
File ownership
Linux permissions
