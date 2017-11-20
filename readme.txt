
The zip file contains a virtual machine with Ubuntu 14.04 LTS operating system. It comes pre-installed with SAGE, Z3, KLEE, Java, JPF and Junit. Most importantly, it includes DIG or SymInfer - a state of the art tool for generating numerical invariants using symbolic states extracted from a symbolic execution tool (please visit https://bitbucket.org/nguyenthanhvuh/symtraces/wiki/Home to know more). To use the virtual machine, first download and unzip the file "Ubuntu 14 DIG". After unzipping, please open the configuration file "Ubuntu 14 DIG.vmx" using either "VMware Workstation Player" (available for free for personal use) or "VMware Workstation" (license required). VMware workstation player allows you to run virtual machine for free. Please visit the following link to download the player: https://my.vmware.com/en/web/vmware/free#desktop_end_user_computing/vmware_workstation_player/12_0.

Virtual machine password as well as the root password is "s".

DIG or SymInfer Website:
https://bitbucket.org/nguyenthanhvuh/symtraces/wiki/Home

Quick reference to install locations:
Z3=/home/balaij/Documents/z3
SAGE_PATH=$Z3/src/api/python
KLEE=/home/balaij/Documents/KLEE
JPF_HOME=/home/balaij/Documents

Please note that these locations are already added to bashrc, so no need to export it again if you are running inside the bash terminal, but you may want to include these if you are using any other shell or embed in other programming.

DIG or SymInfer usage:
For C programs:
balaij@ubuntu:~/Documents/symtraces$ sage -python -O dig.py programs/nla/cohendiv.c -log 3

For java programs:
balaij@ubuntu:~/Documents/symtraces$ sage -python -O dig.py programs/nla/CohenDiv.java 

