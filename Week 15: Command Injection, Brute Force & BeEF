## Week 15: Command Injection, Brute Force & BeEF

### Command Injection

For this activity I used a command injection to run commands against the operating system. Using the dot-dot-slash method I was able to access the /etc/passwd and /etc/hosts files from the web page and terminal.

![Command_Injection_From_Terminal](Images/Week_15/Command_Injection_From_Terminal.png)

8.8.8.8 && cat ../../../../../../etc/passwd
![Command_Injection_Passwd](Images/Week_15/Command_Injection_Passwd.png)

8.8.8.8 && cat ../../../../../../etc/hosts
![Command_Injection_Hosts](Images/Week_15/Command_Injection_Hosts.png)

#### Mitigation
Admins need to properly set permissions on web files.  By default, permissions are inherited from the file they are in. They could also implement input validation logic to create parameters so that an input outside of the parameters would be rejected. 


### Brute Force Attack

In this activity the "client" is concerned that a web application has been accessed with a compromised password. Given a list of user names and passwords, I was able to use Burp Suite Intruder to determine the compromised user name/password combination.

![Brute_Force_With_Burp_Suite](Images/Week_15/Brute_Force_With_Burp_Suite.png)

#### Mitigation
When the breach was discovered all of the passwords should have been changed.  Additionally, a password policy should be implemented to change passwords on a frequent basis.  Passwords should also be long and contain numbers, letters, and characters.  Such policies would make it extremely difficult for a hacker to conduct a brute force attack with success.

### BeEF

For this activity I demonstrate how BeEF can be used to "hook" unsuspecting victims.

BeEF can be used to capture Facebook login credentials using the Social Engineering >> Pretty Theft tool:
![BeEF_Facebook](Images/Week_15/BeEF_Facebook.png)

A malicious actor may also use fake notifications. This example shows the Social Engineering >> Fake Notification Bar tool.
![BeEF_Fake_Notification_Bar](Images/Week_15/BeEF_Fake_Notification_Bar.png)

This is how it appears on the malicious actor's end when the victim clicks the fake notification.
![BeEF_Hook_Fake_Notification](Images/Week_15/BeEF_Hook_Fake_Notification.png)

Who knew Clippy was still hanging around ready to help?! (Social Engineering >> Clippy)
![BeEF_Clippy](Images/Week_15/BeEF_Clippy.png)

As you can see, Clippy is not so helpful after all.
![BeEF_Hook_Clippy](Images/Week_15/BeEF_Hook_Clippy.png)

For those who do not want to give up Flash... (Social Engineering >> Fake Flash Update)
![BeEF_Fake_Flash_Upddate](Images/Week_15/BeEF_Fake_Flash_Upddate.png)

Hooked ya!  Guess they didn't attend Flash's funeral. RIP Flash.
![BeEF_Hook_Flash](Images/Week_15/BeEF_Hook_Flash.png)

Finally, this is the view from the command line:
![BeEF_From_Terminal](Images/Week_15/BeEF_From_Terminal.png)

#### Mitigation
Training is probably most important when it comes to mitigation.  Many of the BeEF hooks were obviously old or unexpectedly requesting information.  Never login to accounts you are not expecting to login to and do not click on popups. Additionally, browsers and operating systems should be kept up to date. If one believes they may be the victim of a BeEF hook they should clear their history and cache. Furthermore, to protect the machine, every machine and network should have a firewall; and every machine should also have anti-virus/anti-malware software.
