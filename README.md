#Nothin But .Net - Setup Instructions

#Required Setup

The following is the setup that you will need to perform to configure all necessary prerequisites to be able to enjoy the week. If you have any questions, please do not hesitate to ask!!

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


##Fork the project repositories for the week

1. Login to your account at [github](https://github.com/login)
2. Search for the username developwithpassion:

![Search for developwithpassion](http://github.com/developwithpassion/nbdn_setup/raw/master/imagesgithub_search_for_develop_with_passion.png)

3. Click on the developwithpassion user

![developwithpassion user](http://github.com/developwithpassion/nbdn_setup/raw/master/images/github_developwithpassion_user.png)

4. Click on the shawaugp repository:

![shawaugp repository](http://github.com/developwithpassion/nbdn_setup/raw/master/images/github_shawaugp.png)

5. Click on the fork button to create your own copy of this repository

![shawaugp fork](http://github.com/developwithpassion/nbdn_setup/raw/master/images/github_fork.png)

6. Repeat steps 2-5 for the repository shawaugs.


## Checkout your local copies of the code

1. Create a folder named course (keep it all lowercase) at the root of your main drive.
2. Open up a git bash prompt and navigate to your course folder.
3. Issue the following command from inside the course folder:



#Optional Setup

##Install TestDriven .Net

* Download and install the latest student version of [TestDriven.Net](http://testdriven.net/download_release.aspx?LicenceType=Personal)

##


