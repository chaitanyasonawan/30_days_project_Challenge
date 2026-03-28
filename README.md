# 🚀 30 Days DevOps Challenge

## 📌 Overview

This repository contains my **30 Days DevOps Challenge**, where I build hands-on projects daily to strengthen my skills in Linux, Git, Docker, CI/CD, and automation.

Each day focuses on solving a real-world problem using DevOps tools and practices.

---

# 📅 Day 1: Log Analyzer Tool

## 🎯 Objective

Build a simple tool to analyze log files and extract useful insights.

## 🛠️ Tech Stack

* Python
* Linux
* Git

## 📂 Project Structure

log-analyzer-project/
│
├── app.log
├── log_analyzer.py
├── report.txt (auto-generated)
├── README.md

## ▶️ How to Run

git clone https://github.com/chaitanyasonawan/30_days_project_Challenge.git
cd project-Day-01
python3 log_analyzer.py

## 📊 Output

INFO    : 3
WARNING : 2
ERROR   : 2

## 💡 Use Case

Helps DevOps engineers quickly analyze logs and detect issues.

---

# 📅 Day 2: Dockerized URL Status Checker

## 🎯 Objective

Build a containerized tool to check the availability of multiple URLs.

## 🛠️ Tech Stack

* Docker
* Linux
* Bash

## 📂 Project Structure

project-Day-02/
│
├── check.sh
├── urls.txt
├── Dockerfile

## ▶️ How to Run

docker build -t url-checker .
docker run url-checker

## 📊 Output

https://google.com -> 301
https://github.com -> 200
https://invalidsite.com -> 000

---

## ⚠️ Major Challenges Faced

### 🔴 1. Docker Build Network Issue

Error:
Temporary failure resolving 'archive.ubuntu.com'

👉 Cause:
Docker container was unable to access internet (DNS issue)

👉 Solution:

* Configured Docker DNS in `/etc/docker/daemon.json`
* Used:
  docker build --network=host -t url-checker .

---

### 🔴 2. Image Naming Error

Error:
repository name must be lowercase

👉 Solution:
Used lowercase naming:
docker build -t project-day-02 .

---

## 💡 Use Case

Useful for monitoring website availability and detecting downtime.

---

# 🧠 Key Learnings

* Git conflict handling (rebase, push issues)
* Docker image build and run
* Debugging real-world DevOps errors
* Linux file and directory management

---

# 📌 Author

Chaitanya Sonawane
