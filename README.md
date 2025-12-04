# RadioDJ Butler
### RadioDJ Database Maintenance Utility

---

## What is RadioDJ Butler?

RadioDJ Butler is a friendly helper program designed to keep your RadioDJ database running smoothly. Think of it as a maintenance crew for your radio automation software! It helps you back up your database, optimize performance, and keep everything in tip-top shape.

---

## Getting Started

### First Time Setup

1. Run **RadioDJ_Butler.exe**
2. Click on the **"DB Config"** tab
3. Enter your database information (see below)
4. Click **"Save Config"** to remember your settings

### Database Configuration

Most RadioDJ users can use these default settings:

| Setting | Default Value |
|---------|---------------|
| **Host** | localhost |
| **Port** | 3306 |
| **Database** | radiodj20341 (or your database name) |
| **Username** | root |
| **Password** | *(leave blank if you haven't set one)* |

> **Tip:** If you're not sure about your database name, check your RadioDJ settings!

### Test Your Connection

1. Go to the **"Main"** tab
2. Click **"Test Connection"**
3. If successful, you're ready to go!

---

## What Does Each Button Do?

On the Main tab, you'll find these helpful tools:

### 🔌 TEST CONNECTION
Verifies that RadioDJ Butler can talk to your database. Always run this first before using other features!

### ✅ CHECK
Examines your songs table to make sure everything is healthy. Like a doctor's checkup for your music database!

### 📊 ANALYZE
Updates statistics about your database to help it run faster. Think of it as tuning up your engine.

### 💾 BACKUP
Creates a complete snapshot of your database and saves it in the **"Backups"** folder. This is your safety net! Backups are automatically named with the date and time so you'll never lose track.

### ⚡ OPTIMIZE
Cleans up and reorganizes all your database tables for better performance. Like defragmenting your hard drive, but for your database!

---

## Making Regular Backups

The most important feature is **BACKUP**! Here's how to stay safe:

### Manual Backup
1. Open RadioDJ Butler
2. Click **"Test Connection"** to make sure everything's working
3. Click **"Backup"**
4. Wait for the green success message
5. Your backup is saved in the **"Backups"** folder!

### Automatic Backup (Advanced)
You can schedule automatic backups using Windows Task Scheduler or RadioDJ's event system:

```
RadioDJ_Butler.exe -backup
```

This runs a backup without opening the main window. Great for overnight or weekly maintenance!

---

## Command Line Options (For Advanced Users)

If you want to automate tasks, you can run RadioDJ Butler from the command line or a batch file:

```batch
RadioDJ_Butler.exe -backup     # Creates a database backup
RadioDJ_Butler.exe -optimize   # Optimizes all database tables
```

These commands will run in the background and automatically use your saved configuration.

---

## Tips & Best Practices

✅ Always test your connection before running maintenance tasks  
✅ Make backups regularly - daily or weekly is recommended  
✅ Keep your old backups for at least a month, just in case  
✅ Run OPTIMIZE once a week to keep things running smoothly  
✅ If something goes wrong, don't panic! Your backups are in the Backups folder

> **Note:** The program automatically resizes to fit your screen, and it remembers your window size for next time. Only one copy can run at a time (so you don't accidentally run two backups at once).

---

## Where Are My Backups?

Backups are stored in a folder called **"Backups"** in the same location as RadioDJ_Butler.exe. Each backup file includes the date and time in its name, like:

```
RadioDJ_radiodj20341_Backup_2025-12-03_14-30-45.sql
```

---

## Troubleshooting

### Problem: "mysql.exe not found" error
**Solution:** RadioDJ Butler needs MySQL to be installed. It should be in your RadioDJ installation folder. Make sure RadioDJ is properly installed.

### Problem: Connection test fails
**Solution:** Double-check your database settings in the DB Config tab. Make sure RadioDJ is installed and the database name matches your setup.

### Problem: Backup file is empty
**Solution:** Check that your username and password are correct. You might need administrator permissions.

---

## Contact & Support

RadioDJ Butler was created by **MrPapaya** for the RadioDJ community.

- **GitHub:** [https://github.com/MrPapaya-JRR](https://github.com/MrPapaya-JRR)  
  Leave questions or bug reports on the release page

- **Ko-Fi:** [https://ko-fi.com/mrpapaya](https://ko-fi.com/mrpapaya)  
  If this software helps you, consider leaving a tip!

- **RadioDJ Forums:** Find MrPapaya as **'JackRabbit'** at RadioDJ.ro

*This is free software - use it however you like! Just don't modify or sell it.*

---

## About This Program

RadioDJ Butler started as a simple batch file and grew into this handy tool. It's designed to make database maintenance easy for everyone, whether you're a tech wizard or just someone who wants their radio station to run smoothly.

**RadioDJ ForEver!**

© 2025 JackRabbit Radio Software  
Released as FreeWare

---

### Thanks for using RadioDJ Butler! 🎵📻
