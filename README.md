pysshbackup
===========

A python cli for 'ssh + rsync + cp with hardlinks' backups featuring menu and incremental backups

 Pysshbackup v2.0
   A python backup system

Installation
##########################################

1) edit the defaults.xml file to your liking: you can change
  * backupfolder
  * ssh server
  * sshuser (if doing full system, you'll need to use root to preserve permssions)
  * ssh password
  * and any files/folders you want backed up

2) save file in /home/<user>/.pysshbackup/defaults.xml (or if you'll run as root, /root/.pysshbackup/defaults.xml)

3) open a terminal, cd to the uncompressed folder and run ./pysshbackup

Remember: you'll need to create an initial full backup before creating partials (f)
Also: I find naming my backups by date (year-mo-da) tends to work well

Dependencies
##########################################
python, paramiko, rsync, ssh, elementtree


**** This script works best with passwordless ssh by key
