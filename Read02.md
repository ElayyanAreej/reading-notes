# Version Control

As you know Developers works in _teams_ which requires sharing work and secure it at the same time, Version control protects secure code from ~~both~~ :
* deliberate 
* unintentional mistakes.

They are also constantly updating the old code, writing new code and dividing the work into multiple tasks. This allows developers to work on multiple things simultaneously, one of them can work on a new feature while the other fixes bugs, as well as requires sharing work and secure at the same time.

![explination](https://www.documentlocator.com/img/knowledge/version-control-diagram.png)

***Version Control*** systems allow software teams to _manage changes_ to secure code over time. Version control software _keeps track_ of every change over time in a special database. This allows developers the opportunity to _turn back time and fix mistakes_ and make comparisons with the least amount of distraction the team.

## types of VCS: 
1. Local Version Control   
  Entails one database on your hard disk that stores changes to files.
2. Centralized Version  
  Single server storing all changes and file versions, which can be accessed by various clients.
3. Distributed Version Control  
   The entire history of the code is mirrored on each system. 


![explination](https://codexitos.com/wp-content/uploads/2019/10/blog-What-is-github-and-why-you-should-use-it..png)
   
# Git
Is a free and open source distributed version control so we can save the version of our work(code) and handle it with speed and efficiency.


## How Git works ?
Git is a **DVCS** that stores data in a file system made up of **snapshots**; each *commit* Git creates a snapshot of the file and stores a reference to it.

![explination](https://vishalsubramanian.com/assets/Blog_1_Fig_2.png)

### Git Benifites:
- Allow Local Operations whiches allowing one to continue     work on a project even when not online or on a VPN.
- Tracked every single change applied whiches save            information in transit from losting.
- Makes it extremely difficult for a snapshot of your file    that is committed to be lost.
- Files in Git can reside in three main states:
   -  committed
   -  modified 
   -  staged.

### How to Getting Start
* First of all **Download Git** *make sure you have the latest version*.
 
### install Git system
You must select the installation way from the three ways below:
+ Install as a package.
+ Install via another installer
+  Download and compile the source code.

Then you should select the **OS platform** (Mac, windows and Linux) you need and familiar with, to set up the Git system on it, if you are select **MAC** operating system use terminal to install Git because it’s The simplest method or you can download it from Git or GitHub. If you select **windows** you can download it from Git website and following the posted directions or Install Git as part of the GitHub for Windows install. Finally, if you are select **Linux** there is two way using Package Manager through distribution’s inherent package management tool or Git Website. 

You can also download Git by visiting [this link](http://git-scm.com/download/) and following the posted directions.

* Then perform some customization steps, which should only need to be completed once on any machine.
###### Note To change settings, you can repeat these steps.

* After installing Git, users should immediately set the useIdentity Setting
r name and email address, which will be used for every Git commit.
<<<<<<< HEAD
Also you can use inherent Git tool called *Git Config* allows the setting of configuration variables that control aspects of Gets operation and look. 

The third step is Check Settings by using related command and your credential user name, email…etc. 
Please note that: if you didn’t select text editor git have feature that called “Default Text Editor” To configure a different text editor, such as Emacs, type the following into your Terminal or Command Line. 

#### Now you Git system is ready! 


# Setting Up A Git Repository

The first step on setting up a get repository its import an existing project or directory into Git by following three steps:
- Switch to the target project’s directory
- Use the git init command
- start tracking these repository files.
 
Also You can create a copy of an existing Git repository from a particular server by using the **clone command** its called the clone process.


#  Workflow
![wrfl](https://blog.udemy.com/wp-content/uploads/2015/08/image036.png)

# Remote Repositories

![RR](https://csharpcorner.azureedge.net/article/git-and-github-version-control-local-and-remote-repository/Images/Git%20And%20Github%20Version%20Control.png)
## Why we need remote repository? 
We need it to collaborate on Git projects, in other word to Access versions of a project residing online or on a Network also Teams can use remote repositories to push Information to and pull data from.
There is a lot privileges type such as read/write or Read-only to access the versions to control it and forbidden some users from edit or delete, insert… etc on The data. So Git provide you privileges management system.  


## How to manage your repository? 
You can manage your repository by (mange Cloned Repositories, Seeing Your Remotes, Adding Remotes, Fetching,Pushing and Renaming/Removing Remotes).


###	Cloned Repositories:
We talked about it earlier (see Setting up a Git Repository) 
