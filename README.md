Simple REXX Exec to generate timing statistics for any TSO command

Syntax:  %TIMER command / count

Where:  command  name of any TSO command, clist, or rexx exec
        /        delimiter
        count  number of iterations 

Example from ISPF command line to run a exec that gets the users home directory and echos using the `say` instruction:

`TSO %TIMER TESTGID / 10`

```
Starting the time test of TESTGID  for  10 times                             
/u/lbdyck                                                                    
/u/lbdyck                                                                    
/u/lbdyck                                                                    
/u/lbdyck                                                                    
/u/lbdyck                                                                    
/u/lbdyck                                                                    
/u/lbdyck                                                                    
/u/lbdyck                                                                    
/u/lbdyck                                                                    
/u/lbdyck                                                                    
REXX Procedure TESTGID  executed  10 times with average service units of 23.3
and a total cpu time of: 0                                                   
with total wall time of: 0
```
