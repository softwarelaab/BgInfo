# BgInfo

[![BgInfo](gett-stateed.png)](https://github.com/softwarelaab/BgInfo)

BGInfo is a tool that is part of Sysinternals. It allows you to display the machine’s configuration info on the desktop wallpaper. Hospitals, schools, and large enterprises with lots of endpoints often use BGInfo to make it easy for sysadmins to see details like IP address, OS version, and hostname when they log in:

## What is BGInfo used for?

It automatically displays relevant information about a Windows computer on the desktop's background, such as the computer name, IP address, service pack version, and more.

## How can you exploit BGInfo?

The OS will automatically associate the BGInfo application with the .bgi extension when it’s first executed. Any .bgi files that a user double clicks will automatically run using the BGInfo executable without prompting the user.

Researchers have already shown that BGInfo can run script files from a remote location. A great example is this article on bypassing application whitelisting with BGInfo.

What we’ll show you here is how BGInfo can be an excellent way for an attacker to avoid detection by anti-phishing and anti-virus.

## How do I fix BGInfo?

* Go to the Startup folder and look and see if there is a shortcut to BGInfo there. If not then go look in Task Scheduler instead.
* Look in the file system. There is most likely a BGInfo folder.
* Adjust the shortcut (or task) to use the correct bgi file.
* If neither file exists then start BGInfo as an admin.
