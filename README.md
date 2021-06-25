# Flask & Vagrant Local Development Environment

## Requirements

* [Vagrant](https://www.vagrantup.com/downloads)

* [VirtualBox](https://www.virtualbox.org/wiki/VirtualBox)

## How to use this environment

1. Clone this repo. 
```
   git clone https://github.com/akiffeyzioglu/flask-setup.git  
```
2. cd into it. 
```
  cd flask-setup
```
3. Start Vagrant.
```
   vagrant up --provision
```

4. Go to browser and type "15.15.15.4", see result.

5.  If you want to see machine UI, you can SSH into the machine.
```
   vagrant ssh
```
6. Logout machine.
```
   logout
```