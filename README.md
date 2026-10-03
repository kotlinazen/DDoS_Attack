# DDoS_Attack
learnign about DDoS attack(for internet security learning)
## testing by VM(simple way,not true DDoS attack)
first, you need a virtual machine and install debian-based distro like kali
then active ssh service
```bash
sudo apt update
sudo apt install openssh-server
sudo systemctl start ssh
sudo systemctl enable ssh
```
second,check the ip address
```bash
ip addr
```
third, connect to your VM
```bash
ssh username@192.168.1.100
```
last,excute
```bash
ssh username@192.168.1.100 "DISPLAY=:0 gnome-terminal -- bash -c 'echo hello world; sleep 10'"
```
then in the VM it will pop out a termianl and says "hello world"
