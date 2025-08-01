# DevOps Home Lab - Episode 6: Shell Scripting Essentials

In this episode, you’ll learn to write your first shell script to automate routine tasks on your virtual machine server.

## What You'll Learn
- Importance of scripting for DevOps engineers
- Writing basic bash scripts using shebang
- Running updates and installing packages via scripts
- Making scripts executable and debugging common errors
- Using echo for logging

## Files Included
- `challenges.txt`: Practice tasks after watching the episode
- `shell-scripting-checklist.txt`: Detailed checklist to follow while writing the script
- `README.md`: Episode overview and usage instructions
- `folder-structure.png`: Visual reference for file setup

## Tools Used
- Vim or Nano text editors
- Bash shell
- apt package manager
- SSH for VM connection

## Final Script Example
```bash
#!/bin/bash
echo "Updating system"
sudo apt update && sudo apt upgrade -y
echo "Installing nginx"
sudo apt install nginx -y
echo "All done"
```

Save it as `setup.sh`, make it executable using `chmod +x setup.sh`, and run it with `./setup.sh`.

## Reminder
Shell scripting is a foundation skill for every DevOps engineer. Automate small tasks, avoid mistakes, and save time.

Watch the full video to follow along step by step.
