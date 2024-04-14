## first of all list all wifi adapter or wifi cards
## using one of the following commands 
```sh
iwconfig
```
## or
```sh
ifconfig
```
## when you find the name of the device copy it
## then down it ( like shutting it down )
```sh
sudo ip link set dev device_name down
```
## then you can rename it ( without shut it down you can't rename it )
```sh
sudo ip link set dev old_devicename name new_devicename 
```
## after renaming it you have to start it or ( up it )
```sh
sudo ip link set dev new_devicename up
```

