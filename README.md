# firstdriver
The objective over here is to write, compile & test our first driver

Setting up the Machine
----------------------
Follow these links, in case, Linux Machine is not being setup yet:
https://ubuntu.com/tutorials/install-ubuntu-desktop#1-overview

If you have a Windows and want to install the Linux using Virtual Box, use:
https://www.youtube.com/watch?v=x5MhydijWmc

Installing the required Packages
--------------------------------
Once you are done with the setup, let's proceed with installing the required packages. 
On Ubuntu, install the packages using:
 $ sudo apt install build-essential rsync gcc bc bison libssl-dev libncurses5-dev libelf-dev

Writing a Driver
----------------
1. The driver is already included as a part of this repo. 
   To compile, execute make
   $ make
This would generate the file by name first_driver.ko
2. Next step is to test the driver. For this we need to use the insmod command
   $ sudo insmod first_driver.ko (Root Privileges are required to load the driver)
   This should load the driver into the system. To verify, execute the 'lsmod' command & check if the driver is listed
   If loading fails for some reason, check if the secure boot is disable or enable the signing of the driver
4. To verify, execute 'dmesg' and check if the corresponding string is printed
  

