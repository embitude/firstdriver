# firstdriver
The objective over here is to write, compile & test our first driver
1. The driver is already included as a part of this repo. 
   To compile, execute make
   $ make
This would generate the file by name first_driver.ko
2. Next step is to test the driver. For this we need to use the insmod command
   $ sudo insmod first_driver.ko (Root Privileges are required to load the driver)
   This should load the driver into the system. To verify, execute the 'lsmod' command & check if the driver is listed
   If loading fails for some reason, check if the secure boot is disable or enable the signing of the driver
4. To verify, execute 'dmesg' and check if the corresponding string is printed
  
