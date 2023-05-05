.NET Core Worker Service
- SystemD NuGet package
---

#### Methods
- Start():
- Stop():
- TerminateProcess():
	- maybe InterceptProcess() depending on if my implementation can detect some sort of system level "Process Launched" event and prevent the executable from starting to begin with.
- BlockingStatus: String ("Block is active" or "Block is disabled")
- CreateBlockList(): BlockListModel
- SaveBlockList(): void
- DeleteBlockList(): void
- EnableBlocking(): void
- DisableBlocking(): void
- GetExecutables(): List
	- recursively searches a folder and all subfolders for ALL executable files, returns a list of either: executable paths, executable names, process names/ID's (depending on how blocking will be implemented)
