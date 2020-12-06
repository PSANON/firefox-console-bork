# Poison Fox
A little POC code for a bug that borks the firefox devtools console with javascript.  
Not for malicious use!

Just open the HTML file in a FireFox browser of your choice.


Firefox already knows about this particular cyclic object issue, but they haven't fixed it (or maybe don't intend to) and I thought this would be a cool application of it.  
As of as of 3/12/2020 this works on the latest firefox (regular, developer addition and nightly builds).


A cool observation: For most tabs, if this bug is executed all one has to do to "fix" it is close the tab.  
But on the "new tab" page, this will bug the console and then even if the new tab page is closed and then opened again,  
the console stays bugged. IDK why, maybe console instance is cached and so it's staying alive even after the new tab page is closed.
