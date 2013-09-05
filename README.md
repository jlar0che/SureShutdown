SureShutdown
============

Version 1.0.3
September 5th, 2013
Jacques Laroche

----------------------------------------------------
CONTENTS:
----------------------------------------------------

I. FEATURES
II. RELEASE NOTES
III. CONTACT INFORMATION


----------------------------------------------------
I. FEATURES
----------------------------------------------------

*	Immediate Forced Shutdown of computer.

*	Option to select time to Force Shutdown computer.
 
*	Immediate Forced Restart of computer.

*	Option to select time to Force Restart computer. 

*	Force Shutdown computer when Shift+Ctrl+Alt+S is pressed.


----------------------------------------------------
II. RELEASE NOTES
----------------------------------------------------

* Added Feedback mechanism.

* Added Minimize to Tray mechanism.

* Settings Page Added with three options:
  
  1) Run Minimized on application startup.

  2) Initialize Shift+Ctrl+Alt+S shortcut for immediate Forced Shutdown of computer.
  
  3) Start application on Windows startup.

Important Note:

* UAC in Windows 7 seems to always come up when Sure.Shutdown is run. This can be quite annoying, especially if
  you chose to run Sure.Shutdown when Windows starts up. Fortunately there is a solution to this.

  Disable the UAC for Sure.Shutdown:
  1. Right-click the Sure.Shutdown exe file to assign it an administrative token.
  2. Click Properties, and then select the Compatibility tab.
  3. Under Privilege Level, select “Run this program as an administrator”, and then click OK.

  Your other option if to turn off UAC.

  Elevate without prompt:

  1. Click Start and in the Search mechanism type "Local Security Policy". When it appears in the search result, press Enter to run it.
     (Note: You can also press  + R and when the Run dialog appears type: "secpol.msc" and press Enter).
  2. Expand the Local Policies tree and click on the Security Options.
  3. On the right-side a list of security settings will appear, search for "User Account Control: Behavior of the elevation prompt for administrators in Admin Approval Mode".
  4. Right-click on it and choose Properties. A dialog will appear.
  5. In the middle of the dialog you'll see a comboBox with the default value = "Prompt for consent for non-Windows binaries".
  6. Click on that comboBox and choose "Elevate without prompting", click Apply and OK.
     (Note: This does NOT require a PC reboot)
  7. Double click on the program to verify if it works. 


Technical Notes:

This program was written in Visual Basic.Net


----------------------------------------------------
III. CONTACT INFORMATION
----------------------------------------------------

Jacques Laroche
https://currentperspectives.org
DigitalDoctorsRx@gmail.com
