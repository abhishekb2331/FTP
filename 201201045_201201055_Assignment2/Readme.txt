IMPLEMENTED ftpt by Abhishek Bhat (201201045)  and Bhumik Shah (201201055)




1) "IndexGet" to get list of file on server.
	a) IndexGet ShortList starting-date starting-time-stamp end-date ending-time-stamp.
		ex. "IndexGet ShortList 02-03-2014 19:11:11 24-03-2014 19:11:11"

	b) IndexGet LongList to get list of all files along with file type and Last Modified time
	   ex. "IndexGet LongList"

	c) A "RegEx" request indicating that the requesting client wants to know the list of files that contain the regular expression pattern in their file names.
		ex. " IndexGet regEx *mp3"

2) A "FileHash" request indicates that the client to enable the client to check if any file's content has changed.
   
   a) A "Verify" request which gives the name of the file that the client wants the hash for.
   		ex "fileHash Verify temp.c"

   b) A "Check All" request which is used to periodically check for modifications in the file.
        ex. "fileHash checkAll".

3) Downloading file from server

   a) ex. "Download Coldplay.mp4"

4) Uploading file from client to server.
	
   a) ex. "upload Coldplay.mp4"

5) To know your earlier commands.
   a) ex "history"

6) To know servers earlier commands
   a) ex. "server-history"
