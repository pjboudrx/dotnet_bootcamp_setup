#Nothin But .Net - Setup Instructions

#Required Setup

The following is the setup that you will need to perform to configure all necessary prerequisites to be able to enjoy the week. If you have any questions, please do not hesitate to ask!!

##Make sure that you have configured windows to show all hidden files and folders

##Configure Powershell

1. Make sure you are running Powershell 2.0.
  * Open up a powershell prompt
  * Type in $hostname.version
  * You should see a Major version of 2 like the following screenshot: <br>![powershell version](http://github.com/developwithpassion/nbdn_setup/raw/master/images/powershell_version.png)
2. Enable execution of local scripts
  * Open up a powershell prompt
  * Type in the following command:
    set-executionpolicy RemoteSigned
  * At the prompt that follows, make sure you type in a capital Y as in the following screenshot: <br>![powershell set_executionpolicy](http://github.com/developwithpassion/nbdn_setup/raw/master/images/powershell_set_execution_policy.png)

##Get setup at [Github](http://github.com)

* [Sign up](https://github.com/signup/free) for a free account at github.com. My recommendation is to use an all lowercase username.

##Install Ruby

* Install the latest version of Ruby from [here](http://rubyforge.org/frs/download.php/75127/rubyinstaller-1.9.2-p290.exe)
* Make sure you select the following options:
  * Add Ruby Executables to your path
  * Associate .rb and .rbw files with this Ruby installation
* Once the install has completed, verify your installation by opening up a command prompt and typing in: ruby -v. You should see:
  * ruby 1.9.2p180 (2011-02-18) [i386-mingw32]

##Install Git for windows

1. Install the 1.7.4 version of git for windows from [here](http://code.google.com/p/msysgit/downloads/detail?name=Git-1.7.4-preview20110204.exe&can=2&q=)

* Configure according to the following screenshots:

![git_setup_part_1](http://github.com/developwithpassion/nbdn_setup/raw/master/images/git_setup_part_1.png)
![git_setup_part_2](http://github.com/developwithpassion/nbdn_setup/raw/master/images/git_setup_part_2.png)

##Setup your git ssh authentication key

1. Open up a git bash prompt
2. Enter the following command:    
   ssh-keygen -t rsa -c your_email_address  
   Accept the defaults for the remaining prompts (leave the passphrase blank).  
3. Navigate to the folder where your ssh key was created (by default your profile folder C:\Users\your_user_name)
4. Open the file id_rsa.pub and copy the contents to the clipboard.
5. Login to your account at [github](https://github.com/login).
6. Navigate to your [ssh settings](https://github.com/account/ssh)
7. Click on the link: Add Another Public Key:
8. Give your key a title and paste the public key that is in your clipboard from step 4 into the Key text entry:

![ssh key entry](http://github.com/developwithpassion/nbdn_setup/raw/master/images/add_ssh_key.png)

##Verify that your git ssh authentication works

1. Open up a git bash prompt
2. Enter the following command:
   ssh-v git@github.com

3. You may be prompted to cache the server identity (type yes)
4. If you have setup your ssh settings correctly the bottom part of the command output should look similar to the following:

![successful authentication](http://github.com/developwithpassion/nbdn_setup/raw/master/images/git_authentication.png)

##Update git configuration details

1. To ensure that you have settings that will work in the most optimal way for the class, I recommend downloading the following [file](http://github.com/developwithpassion/nbdn_setup/raw/master/dev_tools/git/.gitconfig). Edit the file to make the necessary changes for your name and email address. Once you have changed the username and email address, copy the file to your home folder.


##Fork the project repositories for the week

1. Login to your account at [github](https://github.com/login)
2. Search for the username developwithpassion: <br>![Search for developwithpassion](http://github.com/developwithpassion/nbdn_setup/raw/master/images/github_search_for_develop_with_passion.png)
3. Click on the developwithpassion user <br>![developwithpassion user](http://github.com/developwithpassion/nbdn_setup/raw/master/images/github_developwithpassion_user.png)
4. Click on the name of your prep repository for the week(repository name in the screenshot is for example purposes only!!): ![repository](http://github.com/developwithpassion/nbdn_setup/raw/master/images/github_shawaugp.png)
5. Click on the fork button to create your own copy of this repository <br>![fork](http://github.com/developwithpassion/nbdn_setup/raw/master/images/github_fork.png)
6. Repeat steps 2-5 for the app repository for the week.

## Checkout your local copies of the code

1. Create a folder named course (keep it all lowercase) at the root of your C: drive.
2. Open up a git bash prompt and navigate to your course folder.
3. Issue the following command from inside the course folder:

  * git clone git@github.com:[your github user name]/[prep repository name].git prep
    
    Assuming your github username is jp and the prep repository is named bootcamp_prep, the command would look as follows:

    git clone git@github.com:jp/bootcamp_prep.git prep  

4. Issue the following command from inside the course folder:

  * git clone git@github.com:[your github user name]/[app repository name].git app
    
    Assuming your github username is jp, and the app repository is named bootcamp_app the command would look as follows:

    git clone git@github.com:jp/bootcamp_app.git app

5. Once you have completed steps 3 and 4 your course folder should look as follows:

![checked out directory](http://github.com/developwithpassion/nbdn_setup/raw/master/images/checked_out_directory.png)


##Install TestDriven .Net

* Download and install the latest student version of [TestDriven.Net](http://testdriven.net/download_release.aspx?LicenceType=Personal)

##Resharper

1. Download and install the latest version of [ReSharper](http://www.jetbrains.com/resharper/)

##Autohotkey

* Download and install the latest version of [Autohotkey](http://www.autohotkey.com/)


