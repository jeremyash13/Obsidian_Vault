##### .NET
- upon selecting a folder/.exe to block, recursively search the for all .exe files, add them to a *"blacklist"*
- listen for a new process event to fire, check the newly started process against the blacklist, terminate and display a notification when a match is found.
- hook into system events, watch for processes starting, watch for changes to blocked folders such as moving/renaming folder and contents
- use WMI (Windows Management Instrumentation)
	- It provides the `Win32_ProcessStartTrace` and `Win32_ProcessStopTrace` events for detecting when a process has been started/terminated.

https://stackoverflow.com/questions/50999210/how-to-detect-when-a-new-process-is-started

[Win32_ProcessTrace class](https://docs.microsoft.com/en-us/previous-versions/windows/desktop/krnlprov/win32-processtrace)

---
==TODO:==
- [x] research viability of blocking websites at the system level as opposed to using a web extension. (altering HOSTS file?) (C:/Windows/System32/drivers/etc)
	- ==***not a good idea since admin privileges are needed==