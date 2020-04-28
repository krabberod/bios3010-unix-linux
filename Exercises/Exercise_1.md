# Ex. 1 - Accessing Saga

The first exercise takes you through the necessary steps to log on to Saga.
You should already have registered and activated your account.

### 1. Start you terminal (or shell)
- **Windows** users start _gitbash_ application
- **Mac** and **Linux** users start the _terminal_ application

The shell is a user interface giving access to  interpreter for your key-strokes

### 2. Use _ssh_ to log on
**SSH**, (Secure Shell) is a network protocol that gives users a secure way to access a computer over an unsecured network typically used to log into a remote machine and execute commands. To access Saga you need your username, password and the location of the login nodes. The address to saga is _saga.sigma2.no_, you also need to tell saga who you are by stating your username.

``` bash
ssh username@saga.sigma2.no
```
This is how it should look when you log on:

![ssh saga](/images/01_ssh_saga.png)

The first thing you see is a link to the documentation page for the cluster, followed by the support email. Next is the latest news from [the operational log](https://opslog.sigma2.no/) for the cluster. This is were you will find important news about saga and related infrastructure, things like scheduled maintenance, unexpected behavior, node downtime etc will be posted here.  
At the last line you have the command prompt were you can write your commands. Every command you write here _after logging on_ will be executed by the cpus on saga, not on your computer. To see where in the file structure on saga you are you can use the command _pwd_ (print working directory)
```
pwd
```
You should get something similar to this:
>/cluster/home/anderkkr  

Which tells me that I'm currently located in the folder _anderkkr_ which is my username and it is located in the folder _home_, which in again is in the folder _cluster_. You should be in a folder with your own user name. In the next exercise ([Excercise 2](Exercises/Exercise_2.md)) we will have a closer look at the folder structure in linux.

But let's check a few things first:
### Check version
Linux and Unix comes in many different versions and distributions:
Which version of linux is running on saga? Here are to ways of checking (there are probably more):
- Print system information:  
``` uname -mrs ```  
-Print LSB (Linux Standard Base) and Distribution information. (Probably doesn't work on UNIX/MAC)  
``` lsb_release -a ```
