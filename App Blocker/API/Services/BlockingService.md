.NET Core Worker Service
- SystemD NuGet package
---

- Start():
- Stop():
- TerminateProcess():
	- maybe InterceptProcess() depending on if my implementation can detect some sort of system level "Process Launched" event and prevent the executable from starting to begin with.
- BlockingStatus: String ("Block is active" or "Block is disabled")
