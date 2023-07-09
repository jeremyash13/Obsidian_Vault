# Features 
---

#### General:
- all blocking to be carried out by a service to be running in the background
	- the GUI will instruct the service to activate/deactivate 

#### App Blocking:
- Block .exe's (block all in a folder, such as steam library, or select 1 by 1)
	- recursively search a selected folder for .exe's, write the filenames to an encrypted (encrypted so blocks can't be edited to bypass active block) block list on hard drive
		- re-do the recursive search on block activation, incase file names have changed
		- somehow find a way to cause the folder to "be in use" so the folder cannot be renamed or moved while the block is active
			- alternatively, add the folder itself to some sort of list to be tracked, hook into system events and watch for changes to this folder, try to intercept actions.

#### Daily / Weekly Limits:
- Monitor usage of certain processes and websites, allowing access until the allotted amount of time has been used.

#### Browser Extension / Website Blocking:
- Create a browser extension that blocks sites
- renders a custom page when visiting a blocked site
- have a few prepared lists of well known distracting and harmful sites to choose from
- can create your own custom block list and/or extend a premade list
- option to enable *Distraction Free* YouTube
	- instead of blocking YT, block all suggested video feeds. so YT *search* can still be used as a learning resource, but the user cant get sucked down rabbit holes
- Option to enable A.I. detection of Adult/Racy/Gory content present on a web page (Maybe/maybe not, due to API costs)

#### Blocking Policies:
- block for a timed duration ✔
- block on a schedule
- block until restart ✔
- block until a password is entered
- ==MAYBE== add an option to *pay a ransom* to release the block! 🤯🤯🤑🤑
	- customers might complain poor app UI/UX caused them into an aggressive block, forcing them to pay a fee to release.

#### Remote Blocking Controls (parental controls):
- a device using an "Admin" account can dictate blocking policy for all devices on the local network
- Indefinite blocks where permission to access a blocked item has to be granted by an admin.
	- slave device requests permission, a notification is sent to parent, access is approved/denied. 

#### List of warnings to users who try to bypass block:
- DO NOT uninstall browser extensions while block is active
	- All browsers will be blocked for the duration of the block

#### Installation:
- auto detect all browsers on machine
- walk user through installing the browser extension, 1 browser at a time.

#### Support:
- Allow a way to force end all blocks via a backdoor
	- (? option 1) generate a unique password for each customer at account creation. Software will store a copy in the computer's registry (so it knows what password it will allow). Customer support can remote into user's computer and enter password to release blocks. Bundle some lightweight/portable (open source hopefully) remote access software with the app, so that browsers and websites being blocked wont get in the way of remoting in.

#### Licensing:
- $29.99 for a single lifetime license,  +$9.99 to extend the license to each additional device.
- app will run a separate service for monitoring license status (that way if the user attempts to block internet traffic to/from the app, the licensing can still be validated). 
- upon purchase, will be granted a serial # to enter into the software
- licensing can be managed through website (adding new licenses, activating/deactivating serials tied to devices)

#### Blocker Defense System:

###### Defending browser extension uninstalls:
- Method 1: Keep a *secret* backup of browser extension folder, watch browser extension folder for changes, automatically restore missing files from secret backup. 

---
==TODO:==
- [ ] Research and test Browser Extension Defense Method 1