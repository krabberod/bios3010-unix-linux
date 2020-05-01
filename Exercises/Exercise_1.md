# Ex. 1 - Accessing Saga

The first exercise takes you through the necessary steps to log on to Saga.
You should already have registered and activated your account.

### 0. Install a shell
You need to have a shell in order to log on to Saga.   

**Mac and Linux users:**  
If you are using a mac or one of the many Linux distributions you don't need to install anything since these machines comes with a shell and terminal installed. Proceed to step 1.

**Windows user**  
If you are on a Windows PC you need to install a shell. We will use
[Gitbash](https://gitforwindows.org/). Follow this [link]((https://gitforwindows.org/)) and click Download, you will be directed to a repository were you can find the latest version of the program. Scroll down and choose the latest release, _Git-2.26.2_ as of early May 2020. You can choose between 32-bit and 64-bit version. If you have a relatively new installation of Windows on your computer the 64-bit version should work fine, but to be shure you can check which version of Windows you are running [here](https://www.howtogeek.com/howto/21726/how-do-i-know-if-im-running-32-bit-or-64-bit-windows-answers/). If you have an older computer, or have no idea what this is all about you can opt for the 32-bit version. It will work fine for the following exercises. Click and download the **.exe** file for the version you need. Wait tfor it to download and install it as you would any other program.

There are other alternatives for Windos, but they will not be covered in this course. (But if you want to check out some of the alternatives you can use this [link - advanced users](http://faculty.smu.edu/reynolds/unixtut/windows.html) )



### 1. Start you terminal
- **Windows** users start the _gitbash_ application from your start menu
- **Mac** and **Linux** users start the _terminal_ application

You should now have a terminal window with a blinking cursor awaiting your commands.

### 2. Use _ssh_ to log on to Saga

Next you will need  to open a connection to the computing cluster. **SSH**, (Secure Shell) is a network protocol that gives users a secure way to access a computer over an unsecured network typically used to log into a remote machine and execute commands. To access Saga you need your username, password and the adress to the cluster. You were asked to activate your user account a few weeks ago. If you didn't, check the message on Canvas by Jonas dated 23. April, and follow the instructions.

Saga is located at sigma2.no,but you also need to tell the server who you are by stating your username. The full command you should type after the cursor is (note: all command are in ```grey boxes```):

```ssh username@saga.sigma2.no```

The first time you log on ssh will not find the necessary encryptinon keys, and will ask you if you still want to proceed. Type 'yes', you will then be prompted about your password.

![](/Exercises/images/01_Encryption_Key.png)

When you have managed to successfully type your password (this is often harder than it sounds) You should see something like this:

![ssh saga](/Exercises/images/01_ssh_saga.png)

The first thing you see is a link to the documentation page for the cluster, followed by the support email. Next is the latest news from [the operational log](https://opslog.sigma2.no/) for the cluster. This is were you will find important news about saga and related infrastructure, things like scheduled maintenance, unexpected behaviour, node downtime etc will be posted here.  
At the last line you have the command prompt were you can write your commands. Every command you write here _after you have logged on to the server_ will be executed on Saga, not on your computer. To see where in the file structure on saga you are currently located you can use the command _pwd_ (which is short for print working directory). Type

```pwd```  
and hit enter.
You should see something similar to this:
>/cluster/home/anderkkr  

Which tells me that I'm currently located in the directory _anderkkr_ (which is the same as my username) and it is located in the directory _home_, which in again is in the directory _cluster_. You should be in a directory with your own user name, this is your home area on saga. In the next exercise you will get a closer look at the directory structure in Linux.

But let's check a few things first. Linux and Unix comes in many different versions and distributions:
Which version of linux is running on saga? Here are two ways of checking:
- Print system information:  
``` uname -mrs ```  
- Print LSB (Linux Standard Base) and Distribution information. (Does't work on UNIX/MacOS)  
``` lsb_release -a ```



Now move on to [Excercise 2](Exercises/Exercise_2.md)
