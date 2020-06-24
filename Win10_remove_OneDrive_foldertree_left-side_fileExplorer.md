# how to remove OneDrive folder tree in left-side windows file explorer - windows 10
# registry edit requiring administrator privileges

1- Registry Editor - type regedit.msc in windows search bar and choose Registry Editor
2- expand HKEY_CURRENT_USER
3- expand SOFTWARE > Microsoft > Windows > CurrentVersion > Explorer > Desktop > NameSpace
4- there will be a number of entries in this location, each one relates to a cloud service that shows up in your file explorer left catalog tree
	- highlight one of these: you will see Name, Type, Data
	- the information in the Data field determines which cloud service, eg. OneDrive, or Dropbox etc
	- export the entry which corresponds to the cloud service you no longer wish to see and save as .reg in a temp location, just in case
	- then delete the entry 