# Windows Optimization Guide

## Overview

1. Change resolution **125% to 100%**
2. **Turn off all Privacy settings**
3. Turn off **Background App** setting
4. Make the **Taskbar Small**
5. Install **Software**
6. **Pin Favorite Apps in the Taskbar**
7. **Uninstall** unnecessary apps
8. Install **Mem Reduct** app

---

## 1. Startup Apps (Enabled)

- Windows Security Notification Icon
- Realtek HD Audio Universal Service

---

## 2. Services (Disabled)

1. Assigned Access Manager Service
2. Background Intelligent Transfer Service
3. BitLocker Drive Encryption Service
4. Bluetooth Audio Gateway Service
5. Bluetooth Support Service
6. Computer Browser
7. Connected Devices Platform Service
8. Connected User Experience and Telemetry
9. Diagnostic Execution Service
10. Diagnostic Policy Service
11. Diagnostic Service Host
12. Diagnostic System Host
13. Downloaded Maps Manager
14. Fax
15. Geolocation Service
16. IP Helper
17. Map Manager
18. Netlogon
19. Parental Control
20. Phone Service
21. Print Spooler
22. Program Compatibility Assistant Service
23. Remote Desktop Configuration
24. Remote Desktop Service
25. Remote Desktop Service UserMode Port Redirector
26. Remote Registry
27. Retail Demo Service
28. Secondary Logon
29. Sensor Service
30. Smart Card
31. SysMain
32. Touch Keyboard and Handwriting Panel Service
33. WalletService
34. Windows Biometric Service
35. Windows Error Reporting Service
36. Windows Image Acquisition (WIA)
37. Windows Insider Service
38. Windows Media Player Network Sharing Service
39. Windows Mobile Hotspot Service
40. Windows Search
41. Work Folders
42. Xbox Accessory Management Service

---

## 3. Virtual RAM Settings

1. Press **Win + S**
2. Open **Advanced System Settings**
3. Navigate to **Advanced** > **Performance** > **Settings**
4. Under **Advanced**, go to **Virtual Memory**
5. Click **Change**
6. Uncheck the **Automatically manage paging file size for all drives** box
7. Select **C: drive**
8. Choose **Custom Size**
9. Enter desired values
10. Click **Set** > **OK**

---

## 4. Memory Integrity

1. Open **Windows Security**
2. Go to **Device Security** > **Core Isolation**
3. Locate **Memory Integrity**
4. Turn off the toggle

---

## 5. Windows Defender Exclusions (Dev Folders)

1. Go to **Windows Security** > **Virus & threat protection**
2. Click **Manage settings** > **Exclusions**
3. Add **Exclusions** for:
   - Your Project Folder (where your code lives)
   - `node_modules` folders
   - `node.exe` process

---

## 6. Performance Settings

1. Press **Win + S**
2. Search for **Adjust the appearance and performance of Windows**
3. Select **Visual Effects**
4. Choose **Custom**
5. Adjust the following settings:
    - Animate controls and elements inside windows
    - Animate windows when minimizing & maximizing
    - Enable Peek
    - Fade or slide menus into view
    - Show thumbnails instead of icons
    - Show window contents while dragging
    - Smooth edges of screen fonts
    - Smooth-scroll list boxes
6. Click **OK**

---

## 7. Msconfig Setup

1. Press **Win + S**
2. Open **System Configuration**
3. Navigate to **Boot** > **Advanced Options**
4. Check **Number of processors**
5. Select the highest number
6. Click **OK**
7. Navigate to **Services**
8. Check **Hide all Microsoft services**
9. Click **Disable all**
10. Manually enable the following:
    - Google Update Service
    - MongoDB Server
    - MySQL80
    - VirtualBox System Service

---

## 8. Registry Editor Settings

### AutoEndTasks

1. Navigate to:
    - `HKEY_CURRENT_USER\Control Panel\Desktop`
2. Right-click in the right pane → **New** → **String Value**
3. Name it `AutoEndTasks`
4. Set its value to **1** (enabled) or **0** (disabled)

### ClearPageFileAtShutdown

1. Navigate to:
    - `HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\Session Manager\Memory Management`
2. Modify `ClearPageFileAtShutdown` to **1**

### Disable Bing Search

1. Navigate to:
    - `HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\Search`
2. Modify `BingSearchEnabled` to **0**

### Disable Power Throttling

1. Navigate to:
    - `HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\Power`
2. Create a new **Key** named `PowerThrottling`
3. Inside the `PowerThrottling` key, create a **DWORD (32-bit) Value** named `PowerThrottlingOff`
4. Set its value to **1**

### Disable Prefetcher

1. Navigate to:
    - `HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\Session Manager\Memory Management\PrefetchParameters`
2. Modify `EnablePrefetcher` to **0**

### GPU Priority & Priority

1. Navigate to:
    - `HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows NT\CurrentVersion\Multimedia\SystemProfile\Tasks\Games`
2. Modify `GPU Priority` to **8**
3. Modify `Priority` to **6**
4. Modify `Scheduling Category` to **High**
5. Modify `SFIO Priority` to **High**

### MenuShowDelay

1. Navigate to:
    - `HKEY_CURRENT_USER\Control Panel\Desktop`
2. Modify `MenuShowDelay` to **10**

### MouseHoverTime

1. Navigate to:
    - `HKEY_CURRENT_USER\Control Panel\Mouse`
2. Modify `MouseHoverTime` to **10**

### Ndu

1. Open **Registry Editor** and navigate to:
    - `HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Services\Ndu`
2. Modify `Start` to **4**

### Startup Delay

1. Navigate to:
    - `HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\Explorer\Serialize`
2. Create the `Serialize` key if it doesn't exist
3. Create a **DWORD (32-bit) Value** named `StartupDelayInMSec`
4. Set its value to **0**

### SvcHostSplitThresholdInKB

1. Navigate to:
	- `Computer\HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control`
2. Modify `SvcHostSplitThresholdInKB` to **1000000**

### System Responsiveness

1. Navigate to:
    - `HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows NT\CurrentVersion\Multimedia\SystemProfile`
2. Modify `SystemResponsiveness` to **0**

### Verbose Status

1. Navigate to:
    - `HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\Policies\System`
2. Create a new **DWORD (32-bit) Value** named `VerboseStatus`
3. Set its value to **1**

### WaitToKillServiceTimeout

1. Navigate to:

    - `HKEY_LOCAL_MACHINE\SYSTEM\ControlSet001\Control`
2. Modify `WaitToKillServiceTimeout` to **500**

3. Navigate to:

    - `HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control`
4. Modify `WaitToKillServiceTimeout` to **100**

### Win32PrioritySeparation

1. Navigate to:
    - `HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\PriorityControl`
2. Modify `Win32PrioritySeparation` to **26**

---

## 9. Task Scheduler (Disable Tasks)

### Application Experience
**Path:** `Task Scheduler Library > Microsoft > Windows > Application Experience`
- Microsoft Compatibility Appraiser
- ProgramDataUpdater
- StartupAppTask

### Customer Experience Improvement Program
**Path:** `Task Scheduler Library > Microsoft > Windows > Customer Experience Improvement Program`
- Consolidator
- UsbCeip
- KernelCeipTask

### Defrag
**Path:** `Task Scheduler Library > Microsoft > Windows > Defrag`
- ScheduledDefrag

### DiskDiagnostic
**Path:** `Task Scheduler Library > Microsoft > Windows > DiskDiagnostic`
- Microsoft-Windows-DiskDiagnosticDataCollector

### DiskFootprint
**Path:** `Task Scheduler Library > Microsoft > Windows > DiskFootprint`
- Diagnostics

### Maintenance
**Path:** `Task Scheduler Library > Microsoft > Windows > Maintenance`
- WinSAT

### Maps
**Path:** `Task Scheduler Library > Microsoft > Windows > Maps`
- MapsToastTask
- MapsUpdateTask

### Mobile Broadband Accounts
**Path:** `Task Scheduler Library > Microsoft > Windows > Mobile Broadband Accounts`
- MNO Metadata Parser

### Speech
**Path:** `Task Scheduler Library > Microsoft > Windows > Speech`
- SpeechModelDownloadTask

---

## 10. Cleanup C: Drive

### Disk Cleanup

1. Press **Win + E**
2. Right-click on **C: Drive**
3. Select **Properties**
4. Click **Disk Cleanup**
5. Click **Clean up system files**
6. Check all boxes
7. Click **OK**

### Delete Temp Files

1. Press **Win + R**
2. Type `temp`, `%temp%`, or `prefetch`
3. Select all files (**Ctrl + A**)
4. Delete permanently (**Shift + Delete**)

### Optimize & Defragment Drive

1. Press **Win + E**
2. Right-click on **C: Drive**
3. Select **Properties** > **Tools** > **Optimize**

---

## 11. Fix Corrupt Files

### Restore Missing or Corrupt System Files

Run this command in **Command Prompt (Admin)**:

```cmd
DISM /Online /Cleanup-Image /RestoreHealth
```

### Check and Fix System Files

Run the following command:

```cmd
sfc /scannow
```