This is a PHP version of the BDS C port of Willie
crowther's game Adventure - the first text adventure game
[or inter-active fiction as its called now-a-days].

I've kept the original C structure as far as possible -
even to the extent of the filenames - so as to provide	
traceability but also to demonstrate how easy C to PHP	
translation actually is. This has NOT resulted in good	
PHP code, but it works.			
		
I also took the opportunity of adding in a few more of the
original FORTRAN comments from Don Ekman's archive of	
Willie's original code. Also, I've de-noop'd the juggle	
routine for all the sado's like me who saw it had been 
removed in the BDSC version so had to go and find out
what it did in the original version!
				
This version seems pretty original - it contains all the 
original features (i.e. bugs!) and the dirty solution	
to the cave [see file walkthru.adv which also came from	
Don's archive]. The main difference is that when the score 
is calculated, a sub-total is output for various sections. 

If you find any bugs in the code, don't mail me - why not
try and fix them yourself as a challenge?

Usage Overview
adventc.php3?install=1		creates MYSQL database 
            ?debug=1		turns on debug output
            ?nodebug=1		turns off debug
            ?reset=1		resets to start of game
            ?forgetme=1 	remove userid cookie cache 
adventoc.php3 			re-indexes advent?.txt files 
				to create advtexth.php3 file 

Requirements
PHP3 or later
MYSQL database with table create privileges

Installation
Extract all the files to a directory on your server, we'll
assume its called /cave for the sake of simplicity.

1. Edit lines 18..21 of the file adventc.php3 to specify
the name of your MYSQL host [or IP address], the account
username and password, and finally the name of the database
to be used.
2. Execute /cave/adventc.php3?install=1 which will create
the MYSQL table entries [or give helpfull(?) error messages
if this fails].
3. Execute /cave/adventc.php3 to play the game.

The programme makes use of the built-in CRC32 hasing algorithm
to create a unique index in the database for each player to
store their game state. To reset your game state back to the
beginning issue the command /cave/adventc.php3?reset=1

To delete your user entry from the database execute
/cave/adventc.php3?forgetme=1

To turn on and turn off debug output enter the following respectively:
/cave/adventc.php3?nodebug=1
/cave/adventc.php3?debug=1

If you alter the text in any of the ADVENT?.TXT files then you
will need to re-index them to get the correct on-screen display. To
do this execute /cave/adventoc.php3 which will re-create the file
/cave/advtexth.php3

HAVE FUN!
Matt
