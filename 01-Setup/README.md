# 🛠️ SQL Server Setup Guide

This section documents the complete setup process for learning Microsoft SQL Server as a Database Administrator.

---

## ✅ 1. Installed Tools

| Tool Name            | Version | Purpose                        |
|---------------------|---------|--------------------------------|
| SQL Server          | 2022    | Main Database Engine           |
| SQL Server Management Studio (SSMS) | 19.x     | GUI Tool for DB Access         |

---

## 🖥️ 2. Installation Steps

### 🔹 SQL Server Installation
1. Download from official Microsoft site.
2. Choose **Developer Edition** (Free).
3. Select basic or custom installation as per need.
4. Use **Mixed Mode Authentication** (Username: `sa`, Password: `yourpassword`).

> 📸 Screenshot: (Add setup wizard screenshot)

---

### 🔹 SSMS Installation
1. Download SSMS from official site.
2. Install with default settings.
3. Connect to server using:
   - Server Name: `localhost` or `.\SQLEXPRESS`
   - Authentication: SQL Server Auth
   - Login: `sa`, Password: `yourpassword`

> 📸 Screenshot: (Add SSMS login screenshot)

---

## ⚙️ 3. Configuration Done

- [x] Enable TCP/IP protocol via SQL Server Configuration Manager
- [x] Open SSMS and successfully connect
- [x] Created default database `SchoolDB`

---

## 🧯 4. Errors Faced & Fixes

| Error Message | Cause | Solution |
|---------------|-------|----------|
| Cannot connect to server | SQL Server services not running | Start services from `services.msc` |
| Login failed for user 'sa' | Wrong password or disabled login | Enable `sa` from SSMS and reset password |

---

## 📂 Folder Structure

```bash
01-Setup/
├── README.md
├── screenshots/
│   ├── sql-install-1.png
│   ├── ssms-login.png
└── setup-notes.txt

