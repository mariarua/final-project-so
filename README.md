# final-project-so

This project comprises a driver for Raspberry Pi that enables the control of a buzzer through the general-purpose ports of the Rpi. The aim is to manipulate the buzzer's PWM to create interesting sounds.

Commands to run the project:

First, execute the following command:

```
  make
```

This command will generate a series of files, including a .ko file.

Next, you should run:

```
  sudo insmod driver.ko
```  

To vary the rhythms produced by our buzzer, you can choose a range between 'a' and 'j' and execute the following command:

```
  sudo echo j > /deb/my_device_nr 
```

If you wish to stop the buzzer, you can use the following command:

```  
  sudo echo a > /deb/my_device_nr
```  

To remove the driver, execute:

```
  sudo rmmod driver
  ```  
  

