# System_HealthCheck_Report

This report was generated using command line tools as part of the Linux Project: System Health Check Report.

Purpose of the Report:
The objective was to create a comprehensive system health report using only command line tools.

Key Commands Used and Their Purpose:
----------------------------------

1. mkdir ~/system_report
   - Purpose: **Make Directory**. Creates the 'system_report' directory in the user's home directory to store all output files.

2. date
   - Purpose: **Display/Set System Date and Time**. Used to capture the current date and time the report was run.

3. uname -a
   - Purpose: **Unix Name**. Prints detailed system information, including the kernel name, network node hostname, kernel release, kernel version, machine hardware name, and operating system.

4. free -h
   - Purpose: **Display Free and Used Memory**. Shows the total, used, and free amount of physical and swap memory in a human-readable format ('-h').

5. df -h
   - Purpose: **Disk Filesystem**. Reports disk space usage for all mounted filesystems, displayed in a human-readable format ('-h').

6. ps -eo ... | head -11
   - Purpose: **Process Status**. Used to report a snapshot of the current processes. The options capture PID, PPID, command, %memory, and %CPU. The output is sorted by CPU usage and piped to 'head -11' to get the header and the top 10 results.

7. ip a
   - Purpose: **Show IP Address and Interface Information**. Displays address information for all configured network interfaces.

8. tar -czvf system_report.tar.gz
   - Purpose: **Tape ARchiver**. Used to create an archive file. The options '-c' (create), '-z' (compress with gzip), and '-v' (verbose) compress the entire 'system_report' directory into a single archive file for sharing.

Report Files Included:
----------------------
- date_time.txt
- system_info.txt
- memory_usage.txt
- disk_usage.txt
- top_processes.txt
- network_info.txt
