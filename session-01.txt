AWS Account
------------
https://portal.aws.amazon.com/billing/signup

#### How to create AWS account
https://www.youtube.com/watch?v=F4jF88UkxV4

1. CC/DB --> give details like
firstname
lastname
address
email

Computer --> computation with in local or wide network
-----------
Laptop
Desktop
Server
Mobile
TV --> smart tv
	android
	wifi/network
	storage
	RAM --> 2GB
Refrigirator --> they can order food items on their own
Washing machine
AC

OS
CPU
Ram
Storage

IP Address

Mobile
----------
OS --> Android
RAM --> 8GB
Storage --> 128/512
CPU --> Snapdragon

WiFi/Mobile net --> Ip address

facebook.com --> computer/server/laptop/mobile

based on purpose
mobile --> calling
laptop/desktop --> surf internet, browsing, watching movies
TV -> watching braodcast channels

server --> install application and serve users/clients

client server
-------------
server --> mobile
client --> laptop

mobile --> files/images

IT --> communication between clients and servers


Operating Systems --> Linux
---------------------------
Windows --> bridge b/w user and hardware --> UI
windows --> user instrcutions --> commands --> 0/1 --> hardware
OS will take care of how to convert instructions into 0/1

Windows vs Linux
----------------
graphics --> load increase on RAM, CPU

servers world --> linux

Fast, less cost

linux is free
stability --> run 10 years also non stop
performance --> very high
security --> comes from unix principles

How to connect linux server
----------------------------
box
lock --> public
key --> private

Auth mechanism
--------------------
1. what you know --> username/password
2. what you have --> tokens
3. what you are --> fingerprints, palms, retina, etc.

what you have

ssh --> secured shell

pub/private key --> generate this pair

Linux server = node = box

ssh-keygen -f <file-name>

Git bash --> https://git-scm.com/downloads
windows --> mini linux
/c/Users/user
/c/Users/sivakumar

ssh-keygen -f daws-76s

ssh-keygen -f ravi

daws-76s.pub --> public key
daws-76s --> private key

ssh-rsa <code> <laptop-name>

cheapest region --> us-east-1 --> somewhat slow than mumbai --> negligible

every region --> min 2 AZ --> HA

AWS --> everything is called as resource

EC2 --> creation of servers

0.0.0.0/0 --> representation of internet / public

Linux is not operating system --> it is kernel

OS vs Kernel
--------------
Kernel --> connecting to Hardware --> no utilities, no shell

Linus Torvalds --> Linux

Unix --> very costly, tightly coupled to hardware

Laptop --> IBM Dos

Linux Kernel --> based on unix principles but code is from the scratch --> C Language

Open source

Kernel + package + shell == OS
Android is flavour of linux
Kernel + package + shell + UI

ubuntu
-------
Desktop --> Kernel + Shell + UI
Server --> Kernel + Shell
centos
RHEL
Fedore
Suse
Arch Linux
99% same --> few commands only will differ

RHEL --> Open source --> but not free
Code open source -> take the code

Support --> immidiate call
community 
RHEL = Centos = Fedora = almalinux = AWS Linux

RHEL --> Code --> OS --> CentOS --> internet community

IP=54.226.152.150
username = ec2-user
private-key

ssh -i <path-to-private-key> username@IP

ssh -i daws-76s.pem ec2-user@54.226.152.150

GitBash/putty --> SSH client
EC2 Server --> SSH server
protocol = SSH
port=22

https://www.facebook.com:443

PROTOCOL IP Address Port-no

username and password

absolute path / relative path

/c/Users/user/daws-76s.pem --> absolute

$ --> normal user
# --> root
pwd --> /home/ec2-user
uname --> kernel name

<command-name> <options> <inputs>
options and inputs are ocassionally optional

<command-name> --help = will get info

1 server --> free 30/31 days
2 servers --> 15 days
3 servers --> 10 days

AWS account
public key and private key
create ec2 server and connect to it
client-server
git bash

ec2 t2-micro charges --> assignment --> INR
t3.medium charges --> assignment

#### DevOps overview sessions

https://www.youtube.com/watch?v=iO8qpPeiph0&list=PLbeIORXauosjypPNHf4YGeEKN3KlSjzOj