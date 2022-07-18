#### Methods
- CreateBlockList(): BlockListModel
- SaveBlockList(): void
- DeleteBlockList(): void
- EnableBlocking(): void
- DisableBlocking(): void
- GetExecutables(): List
	- recursively searches a folder and all subfolders for ALL executable files, returns a list of either: executable paths, executable names, process names/ID's (depending on how blocking will be implemented)