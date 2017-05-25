(All we need are - IE, Notepad and DownloadMaster)
1. 
Open URL
http://services.mtps.microsoft.com/serviceapi/catalogs/dev14/
In IE (you can choose your own locale e.g. ru-ru, fr-fr, pt-br...)

2.
After page was loaded -> right mouse click -> "View HTML Code".
HTML editor window will appear. Choose menu option "Save file" -> just name it "HelpContentSetup.msha" and save it (in utf-8) into local
folder e.g. "C:\Visual Studio 2015". Close "HTML editor".

3. 
Again, right mouse click on the same page -> "Download all by DownloadMaster". (DownloadMaster should be instaled befor, it's freeware)

4. 
You'll see DM-window. Apply filter only for CAB-files. (Links on Folder DocumentsENG\ )
So you should see only cab-files are selected. 
Start downloading into same local folder "C:\Visual Studio 2015".
Approximately all files from Catalog for one locale about 3,5 Gb.

5. 
Now, while downloading, lets make setup file "C:\Visual Studio 2015\HelpContentSetup.msha" as portable. 
Open it in Notepad and Comment lines:
	
	<meta name="ROBOTS" content="NOINDEX, NOFOLLOW" />
    <meta http-equiv="Content-Location" content="http://services.mtps.microsoft.com/serviceapi/catalogs/dev14/en-us" />
    <link type="text/css" rel="stylesheet" href="../../../serviceapi/styles/global.css" /> 



Replace all 
"../../../serviceapi/catalogs/dev14"       by "DocumentsENG/"
"http://packages.mtps.microsoft.com/"      by "DocumentsENG/"
"../../../serviceapi/packages/"            by "DocumentsENG/"
"https://offlinebook.mtps.microsoft.com/"  by "DocumentsENG/"

Save HelpContentSetup.msha - it's ready.


6.
Wait until all CABs were downloaded. (Links on Folder DocumentsENG\ )
So at the end you should have a "C:\Visual Studio 2015" folder contained
HelpContentSetup.msha and DocumentsENG\*.CAB - files.


7. 
Portable instalation of Help Viewer 2.2 for Visual Studio 2015 Library is ready.
PS. If you wish - you can create an ISO - image or burn it to the DVD. Enjoy!