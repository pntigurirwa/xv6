##### CS450: Operating System
##### Programming assignment #2 part 2

Implementation of new system call in xv6: date() will return the current UTC time to run this xv6 

##### Obtaining the repository

###### 1. Assuming you have Git installed on your machine,and  simply run the following command to clone the repository into a directory named xv6 on your machine.
 
 ####   $ git clone  https://github.com/pntigurirwa/xv6.git
      
##### 2. Start up your platform's command line interpreter (a terminal emulator on Linux/OS X, or Windows command prompt), change into the cloned "xv6" directory, then type the following command:

$ cd xv6

##### 3. now that you are in the repository you are going to build xv6 and run it using "QEMU" emulator. The following commands will do this: 
 $ make 
 $ makeqemu-nox
##### 4. The first make command should've resulted in a (successful) build process, while the second should've resulted in the following output:

 :~/xv6-public$ make qemu-nox

qemu-system-i386 -nographic -drive file=fs.img,index=1,media=disk,format=raw -drive file=xv6.img,index=0,media=disk,format=raw -smp 2 -m 512 
xv6...
cpu1: starting 1
cpu0: starting 0
sb: size 1000 nblocks 941 ninodes 200 nlog 30 logstart 2 inodestart 32 bmap start 58 
init: starting sh
$ 
##### 5. Finally type date after a dollar sign that is displayed on your result should look like the following: 
$ date
2019-10-4 2:12:37 UTC
$ 

##### Note: the new added system call of date() was to display the current UTC time  

