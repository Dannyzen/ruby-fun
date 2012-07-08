ruby-fun
========
This repo is for my random ruby projects

1 - File Copier

	Problem: I download zip files that create folders that contain mp3 files. I want these files to be moved automatically to my LAN file server.
	
	Solution: A script that looks in a source folder and its subdirectories, copies all matching filetypes to a destination folder. 
	
Fun Things:
	
	Uses an easy (magical) config file.

	Keeps the original base directories (in the case of mp3s, the "Artist - Album" folder) intact.
	
Usage:

	Modify the config file given yo' needs.

	ruby file_copier.rb.
	
	Done! Check your destination folder, the files should have moved over.
