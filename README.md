serialport-config
==========================

**configure linux serialports on startup via systemd and stty**

## Installation ##

```
apt-get install serialport-config
```

## Configuration ##

File: `/etc/serialports.conf`

```bash
## scheme: <devicename> <baud>

# rs232 baud 9600
ttyS0 9600

# rs232 baud 9600
ttyS1 115200

# rs232 baud 9600
ttyS2 38400
```


## Enable ##

```bash
systemctl enable serialport-setup
systemctl start serialport-setup
```

## Contribution ##

The **.deb** package is automatically generated via a **Continuous Delivery Pipeline** - please do not build packages manually!
