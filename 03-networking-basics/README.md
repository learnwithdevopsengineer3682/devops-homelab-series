# Networking Basics Lab

Welcome to Lab 03: Networking Basics. In the last episode, we set up our first Linux virtual machine. Now it’s time to connect it to the world.

Networking might seem intimidating, but understanding the difference between NAT and Bridged mode will make a huge difference in your home lab confidence — and your interview answers.

## What You'll Learn

- How NAT and Bridge networking work in VirtualBox
- How to test if your VM can reach the internet
- How to connect from your host machine to the VM
- How to find your VM’s IP address
- What to check if networking doesn't work

## Key Concepts

| Mode        | Can VM Access Internet? | Can Host Access VM? | Use Case                    |
|-------------|-------------------------|----------------------|-----------------------------|
| NAT         | ✅ Yes                  | ❌ No                | Safe default for learning   |
| Bridge Mode | ✅ Yes                  | ✅ Yes               | Required for SSH and testing tools like curl or web servers |

## Files in this Lab

- `challenges.txt`: Networking exercises to try out.
- `networking-checklist.txt`: Guided checklist to go step by step.

## Tools Used

- `ping`, `ip a`, `curl`, `ssh`, `VirtualBox Settings`

## Pro Tip

Networking issues are a real-world DevOps scenario. Knowing how to debug them makes you stand out.
