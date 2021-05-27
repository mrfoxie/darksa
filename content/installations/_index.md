+++
title = "Installations"
date = 2021-05-26T14:03:15Z
weight = 10
chapter = true
pre = "<b>B. </b>"
+++

### Installation
![ROS.org](http://wiki.ros.org/custom/images/ros_org.png)

There are many options available to install `ROS` on ur system, it also has multiple availability of Operating System to install. I know that maximum users are using windows 10 few people uses Ubuntu, Linux, Debian etc. on there devices. 

Now a question myself have been arrived in your mind that now I'm telling you to install `Ubuntu`, `Vmware`, or `Virtualbox` on your system but don't worry I have an alternative solution for you for windows user which you will love it as well as other OS users too. 

Now if your Windows 10 then press **Windows + r** and write the following commands to check ur version of Windows.

```
winver
```

If your After that will be using **powershell** in administrator to run the following commands.

```
dism.exe /online /enable-feature /featurename:Microsoft-Windows-Subsystem-Linux /all /norestart
dism.exe /online /enable-feature /featurename:VirtualMachinePlatform /all /norestart
```
After running this 2 commands successfully we can use **Windows Subsystem Linux** or **WSL** on our Windows 10. After completion of the above commands type bellow command.


```
wsl --version
```
This command shall return you with a number but if its give an error then follow the following steps.

## How to become a Windows Insider?

To get enrolled in the Windows Insider Program, head over to the program's [website](https://insider.windows.com/en-us/). Click the Registration button.
You'll need to log in using a Microsoft account; if you don't have a Microsoft account, you can create one using a valid email address. Once you're finished, the Windows Insider registration process will continue.
After creating your Microsoft account or logging in with an existing account, you'll see the Register page. Review the material, check the box, and click Submit.
You'll see the Welcome screen, which indicates registration is complete. You should receive an email with more details about the Windows Insider Program.
With the registration out of the way, it's time to get your Windows 10 PC updated to the latest test builds. Open the Settings app on the PC you want to use as a Windows 10 test machine, and then click Update & Security.
Scroll down to the bottom of the left-hand menu on the Update & Security screen and click Windows Insider Program.
You should be greeted with the screen, which asks you to Get Started enrolling your device. Click Get Started, and follow the prompts to log in with the Microsoft account you used to enroll in the Windows Insider Program.
Once you've linked your Microsoft Account, you'll have to choose from a few different options for how to get Windows Insider builds. The best option is the one Microsoft recommends: Active Development Of Windows--you'll get the latest builds and be able to preview the new features.
Next, choose whether you want to be in the Fast or Slow rings for updates. If you've enrolled only to get your hands on new features, choose Slow so that you're only getting updates that are already tested and stable.
After you finish enrolling, you'll need to restart your PC. Log back into Windows 10 after your computer has restarted and go to Settings | Update & Security | Windows Insider Program and check to be sure the options you chose during device enrollment are showing up properly on the screen. Now that you're enrolled.
