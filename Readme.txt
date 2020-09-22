DSS Server Control 1.1
======================

Thank you for your interest in DSS (Dynamic Socket Stack) Server Control.

This ZIP archive contains a RAR archive which in turn contains
full source code and executables for the applications as advertised.

If you do not have WinRAR or a compatible program to deflate RAR
archives, then visit www.rarsoft.com or www.winrar.com and
download the WinRAR application to deflate the pack contents.

Once you have extracted the project contents from the RAR archive,
you should open the project group file (DSS Control and Example 
Project.vbg). This opens the Example project with the DSS Control
project. When you want to see if the DSS Control is worth its salt,
open the Test DSS project (prjDSSTest.vbp) in the Test DSS folder.

Updated items from version 1.0
------------------------------
*The StartSocket proceedure in the DSS Server Control has been debugged*
The control reference when searching the socket stack was incorrectly
stated as Index, when it should have been the For..Next variable (findsocket).
You may have noticed that the Top Socket was not managed correctly before this
fix. This is now fixed and appears to work much better now. If you notice any
other bugs please do let me know so I can quickly fix the errors and
continue to provide a quality product! (matt@andrews-computers.com).

Register Server
---------------
Please note you must REGISTER the ActiveX file dsssrv1.ocx with the Register
Server provided by Microsoft available on all machines running Windows 95+.

To use the Register Server, click Start > Run and type the following;

REGSVR32 C:\DSS SERVER CONTROL\dssserv1.ocx

(where C:\DSS SERVER CONTROL\ is the containing folder of dssserv1.ocx)
..and click OK. You should see a message confirming the action was a success.

Projects in the RAR archive:

-DSS Server Control 1.1
-Example Multi User Server using DSS Control
-DSS Server Test Program

DSS Server Control 1.0
----------------------
This is the main element of this pack, it allows the developer to
simply insert the DSS Control on to thier application form, and
have a fully working, seamless, multiple user enabled server
framework. You can specify two main properties, which are passed
to the control at run-time when you call the StartDSSServer method.
These are the local port to listen on and the maximum connections
that are allowed. You MUST specify a whole number above the value
of 1 (one) for both of these properties. The control also has various
events that are fired when there is activity on the server framework.
You can see these in more detail by opening the Example project..

Example Multi User Server using DSS Control
-------------------------------------------
A basic demonstration on how to use the DSS Control. It highlights
all events that are key to the DSS Control, and all methods apart
from SendDataToSocket and SendDataToConnectionID. These are
basically what it says on the packet, and simply sends a data
packet to the specified packet or connection id (requestID).

DSS Server Test Program
-----------------------
So you have looked at the DSS Control and Example project and want to
test it out? Look no further, because as I am so nice, there is even a
Server Test project to see if the DSS Server Control can stand its
ground. Open the prjDSSTest.prj project file with Visual Basic located
in the 'Test DSS' folder. The project is already set up to connect to
the local computer (localhost) on port 210, which is the default port
of the Example DSS Control project. Just Run the Example project, click
the Start Multi-User ready Server command button, and then switch to the
DSS Test project and start clicking the connect buttons randomly! This
basically connects to the DSS Server Control that was started by the
Example project, sends a data packet then disconnects after two seconds.
There are six Connect buttons to play with, so you can try and break the
DSS Control. I dont think you will somehow, BUT, if you do, email me
with how it happened and I'll fix it as soon as possible!

Thanks for reading,
-Matt Hall
 
www.nexis-software-technologies.tk
www.aboutmatt.tk
matt_hall44@hotmail.com