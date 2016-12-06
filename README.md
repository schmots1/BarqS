# BarqS
Breakout Automation and Replication for QtreeS

## Change Log
v.2.0
  * Option 5 will now properly end the tdp relationship if an option 3 wasn't used first.  If an option 3 was used first, system will log the inability to re-break-off the tdp
  * Main menu updated to switch positions of options 3 and 4 to make the progressive steps make more sense.
  * 'Back' option added to credential add to allow exiting step instead of having to force kill application.
  * Multi-threaded mirrors now available
  * Group status includes the last runs total time
  * Vfiler sources supported.  Mirrors run over the vfiler0 interface

v.1.2
  * NFS export rules now copy over properly.
  * Added ability to exit from group select if entered accidently.
  * Error checking added for accessing systems that don't have credentials added

Next major update: 
  * Parallel snapmirrors.

v.1.1
  * Bug causing testing volumes to not cutover fixed.  – was actually an error with multiple 7-mode filers.
  * Hidden main menu option ‘dump’ added.  This outputs the database table ‘qtree’ which holds all the info to a csv file called db_dump.csv.  This file is overwritten each time you run the option.
  * Groups that have not been initialized, now can’t be updated, so it won’t just generate a ton of errors if you try.
  * After cutover step finished status changed to completed for reporting on finished qtrees
  * Version of application now listed at the top of the main menu.
 
Next issue to be fixed:
  * Nfs export rules not copying over properly.


