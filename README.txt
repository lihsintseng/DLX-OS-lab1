As mentioned in the project-1 instruction website:
1.  $ cd ~/ece595/lab1/os
    $ make
    to build the ~/ece595/lab1/os/work/os.dlx.obj
2.  $ cd ~/ece595/lab1/apps
    $ make 
    to build the ~/ece595/lab1/apps/work/userprog.dlx.obj
3.  $ dlxsim -x ~/ece595/lab1/os/work/os.dlx.obj -a -u ~/ece595/lab1/apps/work/userprog.dlx.obj
    to run the program.
    The output will be:
	Stack=0x1fffa8, pc starting at 0x9ddc
	Got 2 arguments.
	Available memory: 0x1319c -> 0x200000.
	Argument count is 2.
	Argument 0 is -u.
	Argument 1 is /home/min/a/tseng24/ece595/lab1/apps/work/userprog.dlx.obj.
	Hello World!
	PID = 31
    Which tells us the PID value is 31.

The resource helping me through this project is the concept the professor mentioned in the class stating that the PID number is the subsraction between current PID and the head of the stack.
