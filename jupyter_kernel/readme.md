# MicroPython kernel

Works with hardware device over serial port and unixport as a subprocess.

## Installation:

Dependencies:

```
pip3 install pexpect pyserial jupyter
```

Kernel:

```
python3 -m jupyter kernelspec install f469kernel
```

Add module to python (development mode):

```
pip3 install -e .
```

## Connection

Use lsmagic string. 

To connect to micropython unixport provide path to a binary:

```
%spawn path/to/micropython_unix
```

To connect to the device provide port and optinally baudrate

```
%connect /dev/tty.usbmodemblahblah 115200
```
