The original repo has a final version of the source code that was not released as a .dll file. It made the files created go back to being a .log, readable by FF Logs Uploader, instead of a .zonelog file.
I only compiled it and made it more easily available.
All credits go to the original creator valarnin.

# ACT FFXIV Log Splitter Plugin

This plugin will automatically split FFXIV logs into `Zone_<DateTime>_<ZoneName>.log` files, in the same folder as normal FFXIV logs.

Just download the latest release DLL and load it as an ACT plugin.

Features:
- Automatically split encounters to log files per zone, the same way the FFLogs uploader does, but in real-time
- If a zone doesn't have an encounter, it will be removed when changing to a new zone. For example:
  - In E9S -> creates zone file for E9S
  - Clear fight
  - Zone out to Eulmore -> creates zone file for Eulmore
  - Zone in to E10S -> creates zone file for E10S, removes zone file for Eulmore since no encounters happened

Example of zone files created:

![image](https://user-images.githubusercontent.com/6119598/122481763-4c309700-cf9d-11eb-86e8-b5f3490ca3a8.png)
