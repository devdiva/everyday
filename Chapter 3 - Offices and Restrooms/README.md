# A Quick Recap

## Running *

When this book talks about "simply running the script..." you are expected to know what to do based on the context of the example.  All of this is covered variously in the first chapters, but in case you aren't clear, here is what you need to know.
  
When this book talks about running scripts, it is talking about using either R or Ruby and the corresponding shell (CLI).  It should be clear what to use based on the type of file you are trying to run, check the extension if you still need a clue:
* .rb is ruby
* .r is R

### Ruby
Checkout "Running Ruby" in Chapter 1, but here's a recap. Running a Ruby script from the command line is either by executing the file as a ruby script in your terminal's shell or in the irb shell.

#### Ruby via the shell
As in the following example (where "$" is the command prompt on your system):  

	$ ruby my_script_to_run.rb

#### Ruby via irb
As in the following where you start irb session, then copy and paste the code into the irb and see it go.

	$ irb
	> 

Or, you can try to load the script file into irb.  You know you are successful when you get a response like ```=> true```.
	
	$ irb
	> load 'my_script_to_run.rb'

### R

Checkout "Using R" and "The R Console" in Chapter 2, but here's a recap.  

	$ R
	> source("my_script_to_run.r")

Okay, so... since you are reading this book to learn, just running the source command isn't going to get you to an understanding of what's happening.  Here is an example of the source command which enables verbose output, telling you what it did in each line of evaluating the file.

	source("example3-5.r", verbose = TRUE)

Lastly, a couple more R commands to keep you cruising along with your R training wheels.

The ```help()```  command is your friend. Pass in the method you want to learn more about to see the man page for that command.  For example, ```help(source)```.  
	
Not sure if you're last script worked?  Try the  ```warnings()``` command to get a list of any warnings the script encountered in it's execution.

### Disclaimer: Just because you can, doesn't mean you should...

Okay, so chances are you are reading this book to learn.  Running scripts right off the bat is not likely to be the best way to learn AND understand what you are doing.  For example, you might not have seen the R application whine when you used ```mean(data)``` like in the book example, where it has been deprecated and the code samples reflect the updated ```colMeans(data)``` usage.

