# NostCore
Continued development on the Leaked Nostalrius Core.

# How to compile:
 Download TBB from here:
 https://www.threadingbuildingblocks.org/sites/default/files/software_releases/windows/tbb2017_20170118oss_win.zip
 
 Extract the contents of the tbb2017_20161128oss folder inside the zip file to:
 C:\Program Files\Intel\TBB\
 
 Download ACE from here:
 http://download.dre.vanderbilt.edu/previous_versions/ACE-6.4.2.zip
 
 Extract the contents of the ACE_wrappers folder inside the zip file to:
 C:\Program Files\ACE\Include\
 
 Inside the ace folder, create a new file called "config.h", inside it write:
 #include “ace/config-win32.h”
 
 Then compile ACE using the ACE_wrappers_vc14 solution.
 
 Once done, copy the dll and libs files compiled into this folder:
 C:\Program Files\ACE\lib\
 
 Add a new enviroment variable called ACE_ROOT directing to the ACE folder in Program Files
 
 Generate the NostCore solution using cmake, compile and good to go!
