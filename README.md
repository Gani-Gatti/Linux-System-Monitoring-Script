# Linux System Monitoring Script

A simple Bash script that monitors basic Linux system health metrics such as:

- CPU usage
- Memory usage
- Disk usage
- Running processes
- System uptime

This project was created to practice Linux administration and Bash scripting concepts commonly used in DevOps environments.

## Features

- Displays CPU usage
- Checks memory usage
- Checks disk usage
- Lists top CPU-consuming processes
- Shows system uptime
- Simple Bash scripting project


## Commands Used

### 1. CPU Monitoring

top -b -n 1

- "-b" → Runs in batch mode (non-interactive)
- "-n 1" → Executes once and exits

Used to capture CPU and system statistics without opening interactive mode.

### 2. Disk Usage

df -h

- Displays filesystem disk space usage
- "-h" shows output in human-readable format

### 3. Memory Usage

free -h

- Displays RAM and swap memory usage
- "-h" shows values in human-readable format

### 4. Running Processes

ps -ef --sort=-%cpu | head

- Lists top CPU-consuming processes


### 5. System Uptime

uptime

- Shows how long the system has been running
- Displays system load averages
- 

## How to Run

chmod +x system_monitor.txt
bash system_monitor.txt

## Sample Output

CPU Usage: 23%
Memory Usage: 3.1GB / 8GB
Disk Usage: 58%
Top Processes:

## Future Improvements

- Add alert system for high CPU or disk usage
- Log output to a file
- Send email notifications
- Automate monitoring using cron jobs


## Skills Demonstrated

- Linux administration
- Bash scripting
- System monitoring
- Process management
- Command-line tools
