## Wine 

[Wine](https://www.winehq.org/) (originally an acronym for "Wine Is Not an Emulator") is an open-source project that provides a compatibility layer used to run Windows applications on other operating systems such as macOS and Linux

## Verifying the system architecture

Bfore installing Wine, we need to verify the system architecture as it uses different configurations tailored for 32-bit and 64-bit versions of Ubuntu to ensure optimal compatibility and performance when running Windows applications on each architecture. On our ubuntu machine, we can check this using the ```lscpu``` command.
<br>

![image](https://github.com/user-attachments/assets/7d2662b8-4f6c-486c-b267-755e91da6899)

The CPU op-mode(s) field shows which architecture you are using:

* CPU op-mode(s): 32-bit. The system has a 32-bit architecture.
* CPU op-mode(s): 64-bit. The system has a 64-bit OS.
* CPU op-mode(s): 32-bit, 64-bit. The system supports both.

## Installation

Before installing ```wine``` on our machine, let us first update the repository package.
```
apt update -y
```
<br>

For installing ```wine``` we can use both ```32-bit``` or ```64-bit``` as our system supports both based on the image above. we can use the following commands for installing:
```
apt install wine32 -y
```
or 
```
apt install wine64 -y
```
<br>

Once, done we can verify the installation by checking the running version.
```
wine --version
```
<br>

