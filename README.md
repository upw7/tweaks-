================================================================
                 made by 2afk / quse :3
               this tool for lazy people :3
================================================================
 
DESCRIPTION
-----------
Simple Multitool is a Windows utility toolkit that combines a
system optimizer and a system cleaner into one easy-to-use menu.
It requires administrator privileges to run.
 
 
FILES INCLUDED
--------------
starter.bat   - Main launcher. Requests admin rights and shows
                the main menu to choose between Optimizer or Cleaner.
 
main.py       - The Optimizer. A Python script that applies Windows
                privacy and performance tweaks via PowerShell and
                registry edits.
 
code.bat      - The Cleaner (Quse Tools v3.0). A batch script with
                19 tools for cleaning, networking, system info,
                and power management.
 
 
HOW TO USE
----------
1. Double-click starter.bat
2. Accept the UAC (admin) prompt if it appears
3. Choose from the main menu:
     1 - Optimizer (runs main.py)
     2 - Cleaner   (runs code.bat)
     0 - Exit
 
 
OPTIMIZER (main.py) - WHAT IT DOES
------------------------------------
Applies the following Windows tweaks automatically:
 
  Privacy:
    - Disables user activity publishing (Timeline)
    - Disables Windows consumer features / suggestions
    - Sets telemetry to minimum (0)
    - Disables Windows Defender sample submission
    - Disables location services
    - Disables Teredo (IPv6 tunneling)
 
  Services:
    - Disables DiagTrack (Connected User Experiences & Telemetry)
    - Disables WerMgr (Windows Error Reporting)
 
  Explorer / UI:
    - Shows file extensions in Explorer
    - Shows hidden files and folders
    - Disables Sticky Keys shortcut
    - Hides the Task View button from taskbar
 
  Cleanup:
    - Removes Windows Widgets and Web Experience Pack
    - Deletes Temp folder contents
    - Runs Disk Cleanup (cleanmgr /sagerun:1)
 
  System:
    - Disables WPBT execution
    - Creates a System Restore Point before changes
 
 
CLEANER (code.bat) - AVAILABLE TOOLS
--------------------------------------
Cleaning:
  [1]  Delete Temp files
  [2]  Delete Prefetch files
  [3]  Delete Windows Logs
  [4]  Delete Browser Caches (Chrome, Edge, Firefox)
  [5]  Empty Recycle Bin
  [6]  Full Cleanup (all of the above at once)
 
Network:
  [7]  Flush DNS Cache
  [8]  Show Network Info (IP, MAC, adapters)
  [9]  Test Internet connection (ping Google)
 
System:
  [10] Show System Info
  [11] List Running Processes
  [12] Kill a Process by name
  [13] Check Disk Usage
  [14] Run Windows Disk Cleanup tool
 
Utilities:
  [15] Restart Explorer.exe
  [16] Shutdown / Restart / Logoff
  [17] Open Task Manager
  [18] Open Control Panel
  [19] Open Device Manager
 
 
REQUIREMENTS
------------
- Windows 10 or Windows 11
- Python 3.x installed (and added to PATH) for main.py
- Must be run as Administrator (starter.bat handles this automatically)
 
 
NOTES
-----
- The optimizer changes are applied immediately with no confirmation.
  A System Restore Point is created beforehand so you can undo changes
  via Windows System Restore if needed.
- Browser cache deletion targets default profile paths only.
  Custom profile locations will not be affected.
- Killing the wrong process in option [12] may cause instability.
  Use with caution.
 
================================================================
