##### .NET
- upon selecting a folder/.exe to block, recursively search the for all .exe files, add them to a *"blacklist"*
- listen for a new process event to fire, check the newly started process against the blacklist, terminate when a match is found.
- use WMI (Windows Management Instrumentation)
	- It provides the `Win32_ProcessStartTrace` and `Win32_ProcessStopTrace` events for detecting when a process has been started/terminated.

https://stackoverflow.com/questions/50999210/how-to-detect-when-a-new-process-is-started

[Win32_ProcessTrace class](https://docs.microsoft.com/en-us/previous-versions/windows/desktop/krnlprov/win32-processtrace)