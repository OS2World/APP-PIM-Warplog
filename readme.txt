WARPLOG version 0.99 beta
Author Mark H. Tucker
Dec 30, 2001 

1. Introduction
2. System Requirements
3. Installation/Upgrading
4. Uninstall
5. Usage
6. License
7. History
8. Possible Future Plans
9. Thanks
10. Contact Information


1.Introduction
==============
Warplog is a journal type program that allows you to record daily
events or notes in a simple PM interface.   Data is stored in a normal
(human readable) text file (with a few high-ASCII characters). It 
provides a simple search facility for your entries.   

I wrote this program because I couldn't find an acceptable application
for this purpose under OS/2, DOS or Win16.  It has was also an excuse
for me to learn REXX and DrDialog.  I was originally doing this for my
own use but decided to make it available for public consumption. 

I'm still calling this version a beta since there are still things I
haven't tested thoroughly.  The core of the program has been working
well for me and I've been using it daily for several months now
without any data loss.  I have about 18 months of data stored and it
still seems to handle things efficiently.  I've made a few relatively 
minor changes and very few new features since version 0.95. There is a 
long list of features I'd like to add to the program but I'm not
likely to add any more until I release this feature set as a "1.0"
release.  I plan to continue development after version 1.0.
 

2. System Requirements
======================
Warplog has been tested on my P200, 64MB RAM running Warp 3 with
classic REXX installed.  No additional libraries are required.  I
would expect it to work on any 32 bit version of OS/2 (2.0 -> eCS) but
I have not tested it on any other system.  If you have problems,
please let me know and I will do what I can to make things behave.  As
far as minimum hardware goes, it should run on any system capable of
running OS/2. 


3. Installation
===============
New Installation:
If you haven't done so, unzip the contents of the archive into an
empty directory.  If you want a shortcut on your desktop then make a
shortcut or use the "program" template from the Templates folder.  I
don't like programs that have convoluted installations so I've kept
this one simple.  Besides, I'm lazy. 

Upgrading:
If you already have WarpLog installed then you should make a backup of
your data before using the new version.  You're already doing this as
a normal part of your computer usage, right?  Perhaps I should repeat
this: MAKE A BACKUP OF YOUR DATA!!!  I have no reason to believe that
you will experience data loss but I _strongly_ recommend that you make
a backup just to be safe. 

Once you've made a good, reliable, tested backup of your data you
should unzip the contents of this archive to a temporary directory.
To upgrade you need only copy over three files to your current
installation directory: WarpLog.exe, README.TXT and optionally,
source.zip.  The first time you launch WarpLog you will need to set
the names for your subject titles and bookmark titles in the new
"Settings" dialog.  I should probably write a script so that there is
a nice upgrade process but that'll probably never see the light of day
(along with better documentation) for version 1.0. WarpLog will now
create it's own ini file on startup to store all program settings.
The old settings file, warplog.rc, is no longer necessary.


4. UnInstall
============
Delete the directory containing Warplog and all it's related files.


5. Usage
========
Unless you've never used OS/2 before, this program should be largely
self explanatory.  There are mouse-over hints in the bottom of the
main window which should be enough to get anyone up to speed. With the
"Settings" dialog you can now change the "subject" names or the
program's default data file. 

I've added a feature for "bookmarking" lines in an entry.  The
idea behind this is to make it easier to search for specific types of
information without dedicating an entire subject entry to it.  You
will find a new option in the "Search" dialog to specifically seach
just these lines.  Bookmark titles can be added or edited from the
"Settings" dialog. 

The "Open" button will now provide the ability to select a data file
to open other than the program default.  A new data file can be
created by using the "Open" dialog and entering the name for a new
data file. 

If things get weird, try deleting the warplog.ini file.  The program
will create a new default ini file on it's next startup.  This will
not affect your data.

6. License
==========
This REXX code that I wrote may be used and/or redistributed according
to the terms of the GNU GPL.  See the COPYING file included in the
distribution archive for more exciting details about redistribution
and the lack of warranty. 

My only request is that if you find this program to be useful to send
me an email at mark@tucker.net.  If you do not like it, I'd be
intereseted in hearing what you find to be deficient.  This program is
freeware under the GPL; you are under no obligation to contact me.
The more feedback I get the better this program is likely to become. 

The program icon came from the ticn10ic.zip archive on hobbes.nmsu.edu.

7. History
==========
Dec 30, 2001 - ver. 0.99 rereleased.
        + Fixed a problem with loading the RexxUtil libraries
	+ Fixed a bug in searches that span more than one year.
Dec 26, 2001 - ver. 0.99 released.
	+ fixed several minor date handling routines (days of week
	should be correct now).  This only affected the interface and
	not the storage of data.
	+ fixed a leap year bug in the date selection display
	routine. Again, this did no harm to the data storage.
	+ Added a few double-click shortcuts to functions
	(eg. add/edit from the date selection list).
	+ Added limited font selection support (found under
	"settings").
	+ Added window settings to automatically store the position of
	the program and it's various windows.

Aug 21, 2001 - ver. 0.95a released. (the shameful bugfix release)
	+ Fixed a bug where adding a bookmark deletes the existing text in an entry.
	+ optimised a few minor routines.

Aug 13, 2001 - ver. 0.95 released
	+ Added a button bar with more functions
	+ Added clipboard support
	+ Added a settings dialog
	+ Added the ability to open a data file other than the default
	+ Added "bookmark" support
	+ Updated the search engine.
	+ numerous minor bug fixes
	+ optimized many routines
	- WarpLog.exe now exceeds 100k (just barely). Sorry.

May 3, 2001 - ver. 0.85 released


8. Possible Future Plans
===============
- Add the ability to save color and size settings
- printing support?

9. Thanks
===============
I just wanted to thank all those who have pointed out bugs, made
feature suggestions and offered help with improving my Rexx code.  


10. Contact Info
===============
Current versions of this program can be found my page:
http://www.os2world.com/freeos2/

If you wish to email me with ideas, suggestions, information about a
possible bug, or just say to "hi" send it to: mark@tucker.net 

