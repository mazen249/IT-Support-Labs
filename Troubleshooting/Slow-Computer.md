# 🛠 Windows Troubleshooting Lab — Slow Computer

## 📌 Scenario

A user reported that their Windows computer was running slowly. Applications were taking longer than usual to respond.

The objective was to investigate the issue, identify the likely cause, communicate the findings to the user, and document the troubleshooting process.

---

## 🎫 Support Ticket

**Issue:** Computer is running very slowly  
**Type:** Incident  
**Priority:** Medium  
**Request Type:** Report a system problem

![Jira Support Ticket](./screenshots/07-jira-ticket.png)

The user reported that applications were taking a long time to open and that switching between programs was delayed.

---

## 🔍 Investigation

### 1. Check Windows Update

Windows Update showed two failed updates, including a .NET Framework Security Update and a Windows Security Update.

![Windows Update](./screenshots/01-windows-update.png)

This indicated that Windows update activity could be a possible contributor to the reported performance issue.

---

### 2. Check Running Processes

Task Manager was used to review CPU, memory, and disk usage and identify processes consuming system resources.

![Task Manager Processes](./screenshots/02-task-manager-processes.png)

`Windows Modules Installer Worker` was one of the processes consuming noticeable CPU and memory resources during the investigation.

---

### 3. Check CPU Performance

CPU performance was reviewed using Task Manager.

![CPU Performance](./screenshots/03-cpu-performance.png)

CPU utilization was approximately 17% at the time of the check, indicating that the CPU was not under heavy load at that moment.

---

### 4. Check Memory Usage

Memory utilization was reviewed to determine whether insufficient RAM could be contributing to the slowdown.

![Memory Performance](./screenshots/04-memory-performance.png)

Memory usage was approximately 62% (9.6 / 15.6 GB), indicating moderate memory utilization.

---

### 5. Check Disk Usage

Disk activity was reviewed using Task Manager.

![Disk Performance](./screenshots/05-disk-performance.png)

Disk utilization was approximately 10%, indicating that the disk was not under heavy load at the time of the investigation.

---

### 6. Check Startup Applications

Startup applications were reviewed to determine whether unnecessary applications were launching automatically.

![Startup Apps](./screenshots/06-startup-apps.png)

Most applications were disabled, with only a small number enabled.

---

## 🧠 Findings

Based on the investigation:

- CPU utilization was not under heavy load at the time of checking.
- Memory utilization was moderate.
- Disk utilization was low.
- Most startup applications were disabled.
- Windows Update showed two failed updates.
- `Windows Modules Installer Worker` was consuming noticeable resources during the investigation.

The failed Windows updates and update-related activity were identified as a possible contributor to the reported performance issue.

---

## 💬 Customer Communication

The findings were communicated to the user through Jira Service Management.

The user was advised to install the pending Windows updates and restart the computer. The user was also asked to report back if the performance issue continued.

![Jira Troubleshooting Update](./screenshots/08-jira-troubleshooting-update.png)

---

## 📋 Ticket Status

**Status:** Work in Progress

The ticket remains open while waiting for the user to complete the recommended updates and confirm whether the performance issue has improved.

---

## 🎯 Skills Practiced

- Windows Troubleshooting
- Task Manager
- Process Analysis
- CPU / RAM / Disk Analysis
- Windows Update Troubleshooting
- Startup Application Analysis
- Problem Diagnosis
- Customer Communication
- Ticket Documentation
- IT Support Workflow

---

## 🛠 Tools Used

- Windows 11
- Task Manager
- Windows Update
- Jira Service Management

---

## 🔄 IT Support Workflow

```text
User Report
    ↓
Create Ticket
    ↓
Investigate
    ↓
Collect Evidence
    ↓
Identify Possible Cause
    ↓
Communicate With User
    ↓
Wait for User Confirmation
    ↓
Verify Resolution
    ↓
Resolve Ticket
```