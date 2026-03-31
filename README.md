# Linux Log Monitoring Project

## 📌 Description
This project demonstrates Linux and basic DevOps concepts using AWS EC2.

## 🚀 What I did
- Created an EC2 instance in AWS
- Connected using SSH with PEM key
- Created a log file
- Added sample data
- Used grep to find errors
- Created a shell script to automate error detection

## 🛠️ Commands Used
mkdir log_project
cd log_project
touch system.log
echo "ERROR: Disk issue" >> system.log
grep "ERROR" system.log

## 🤖 Script Used
#!/bin/bash

if grep -q "ERROR" system.log
then
  echo "Error found in system log"
else
  echo "No errors found"
fi

## 📷 Output
