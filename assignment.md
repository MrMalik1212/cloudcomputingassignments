# ASSIGNMENT 1 : MONTH 1 WEEK 2 - LINUX PROCESS MANAGEMENT = INSTALL PHP 7.4
# Step 1 : add PPA repository
* run the command : 'sudo apt install php7.4-fpm'
### output : php -v
``` PHP 7.4.33
(cli) (built: Apr 11 2024 22:13:06) ( NTS )
Copyright (c) The PHP Group
Zend Engine v3.4.0, Copyright (c) Zend Technologies
    with Zend OPcache v7.4.33, Copyright (c), by Zend Technologies
 ```
# ASSIGNMENT 2 : MONTH 1 WEEK 2 - lINUX DEEP DIVE
# Step 1 : Create 3 groups
* run The command : 'sudo groupadd -m -s /bin/bash admin2'
* run the command : 'sudo groupadd -m -s /bin/bash support'
*  run the command : 'sudo groupadd -m -s /bin/bash technical'
# Step 2 : add user to each group
* run the command : 'sudo useradd -G admin2 -m -s /bin/bash zeenat'
* run the command : 'sudo useradd -G support -m -s /bin/bash malik'
* run the command : 'sudo useradd -G technical -m -s /bin/bash muni'
# Step 3 : add admin2 group to the group of sudoers
* run the command : 'usermod -aG sudo admin2'

# ASSIGNMENT 3  : MONTH 1 WEEK 2 - LINUX DEEP DIVE
 #  Step 1 : content of /etc/apt/sources.list 
 CONTENT BELOW : ## Note, this file is written by cloud-init on first boot of an instance
modifications made here will not survive a re-bundle.
 if you wish to make changes you can:
a.) add 'apt_preserve_sources_list: true' to /etc/cloud/cloud.cfg
     or do the same in user-data
 b.) add sources in /etc/apt/sources.list.d
 c.) make changes to template file /etc/cloud/templates/sources.list.tmpl

 See http://help.ubuntu.com/community/UpgradeNotes for how to upgrade to
 newer versions of the distribution.
deb http://archive.ubuntu.com/ubuntu focal main restricted
 deb-src http://archive.ubuntu.com/ubuntu focal main restricted

 Major bug fix updates produced after the final release of the
 distribution.
deb http://archive.ubuntu.com/ubuntu focal-updates main restricted
 deb-src http://archive.ubuntu.com/ubuntu focal-updates main restricted

 N.B. software from this repository is ENTIRELY UNSUPPORTED by the Ubuntu
 team. Also, please note that software in universe WILL NOT receive any
 review or updates from the Ubuntu security team.
deb http://archive.ubuntu.com/ubuntu focal universe
 deb-src http://archive.ubuntu.com/ubuntu focal universe
deb http://archive.ubuntu.com/ubuntu focal-updates universe
 deb-src http://archive.ubuntu.com/ubuntu focal-updates universe

 N.B. software from this repository is ENTIRELY UNSUPPORTED by the Ubuntu
 team, and may not be under a free licence. Please satisfy yourself as to
 your rights to use the software. Also, please note that software in
 multiverse WILL NOT receive any review or updates from the Ubuntu
 security team.
deb http://archive.ubuntu.com/ubuntu focal multiverse
 deb-src http://archive.ubuntu.com/ubuntu focal multiverse
deb http://archive.ubuntu.com/ubuntu focal-updates multiverse
 deb-src http://archive.ubuntu.com/ubuntu focal-updates multiverse

 N.B. software from this repository may not have been tested as
 extensively as that contained in the main release, although it includes
 newer versions of some applications which may provide useful features.
 Also, please note that software in backports WILL NOT receive any review
 or updates from the Ubuntu security team.
deb http://archive.ubuntu.com/ubuntu focal-backports main restricted universe multiverse
 deb-src http://archive.ubuntu.com/ubuntu focal-backports main restricted universe multiverse

 Uncomment the following two lines to add software from Canonical's
 'partner' repository.
 This software is not part of Ubuntu, but is offered by Canonical and the
 respective vendors as a service to Ubuntu users.
 deb http://archive.canonical.com/ubuntu focal partner
 deb-src http://archive.canonical.com/ubuntu focal partner

deb http://security.ubuntu.com/ubuntu focal-security main restricted
 deb-src http://security.ubuntu.com/ubuntu focal-security main restricted
deb http://security.ubuntu.com/ubuntu focal-security universe
 deb-src http://security.ubuntu.com/ubuntu focal-security universe
deb http://security.ubuntu.com/ubuntu focal-security multiverse# deb-src http://security.ubuntu.com/ubuntu focal-security multiverse
