Command Line Interface

- **Router >** **User EXEC mode** -- This mode is very limited, User can look at some things, but can't make any changes to the configuration. This mode is also called as User mode.
- **Router#**   If we enter enable command then we will be going into **Privileged EXEC mode**, Provides complete access to view device's configuration, restart the device etc.. In this mode can not change the configuration but can change the time on the device and save the configuration file 
- use ? to view the commands 
- Router(config)> ---- This mode is global configuration mode. To enter into this mode type conf t from the user privilege mode.
- To enable password..... enable password password ... eg:  enable password CCNA
- We will be having 2 configuration files kept on the device at once. 
1. running-config ---- The current, active configuration file on the device.As we enter commands in the CLI, we edit the active configuration.
      ---- Command--- show running-config in user privilege mode, here we can even see enable password along with the password in the running-config file.
      - To level up security use below commands,
      - **service password-encryption.** (will encrypt the current password) now, we can see jumbled encryption code for the password in the running-config. here **7** is type of encryption to encrypt the password, but we can easily crack using internet. (type 7 password cracker)
      - For more security use below commands,
      - **<span style="color:rgb(0, 176, 80)">enable secret Cisco</span>** (C should be capital) -- it will encrypt the password using MD5 encryption.
      - now in the running config enable password with 7 encryption will be ignored.
2. startup-config --- The startup-config file will be loaded upon the restart of the device.
	  ----- Command--- show startup-config in user privilege mode
	- whenever we restart the device it will load the default config not the startup config
	How to save config file ?
	from privilege-exec mode -- 
	1. <span style="color:rgb(0, 176, 80)">write</span>
	2. <span style="color:rgb(0, 176, 80)">write</span> <span style="color:rgb(0, 176, 80)">memory</span>
	3. <span style="color:rgb(0, 176, 80)">copy</span><span style="color:rgb(0, 176, 80)"> running-</span><span style="color:rgb(0, 176, 80)">config</span> <span style="color:rgb(0, 176, 80)">startup</span>-<span style="color:rgb(0, 176, 80)">config</span>
3. service password encryption: 
		If we enable service password encryption
		- current passwords will be encrypted
		- future passwords will be encrypted
		- the enable secret will not be effected
		If we disable service password encryption
		- current passwords will be encrypted
		- future passwords will not be encrypted
		- the enable secret will not be effected
		