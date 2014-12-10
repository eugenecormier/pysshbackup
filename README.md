pysshbackup
===========

A python cli for 'ssh + rsync + cp with hardlinks' backups featuring menu and incremental backups


##########################################
#
# Pysshbackup v1.0
#   A python backup system
#
#   eugenecormier@gmail.com
#
# This program is free software; you can redistribute
# it and/or modify it under the terms of the GNU General
# Public License as published by the Free Software
# Foundation; either version 2 of the License, or (at
# your option) any later version.
#
# This program is distributed in the hope that it will be
# useful, but WITHOUT ANY WARRANTY; without even the
# implied warranty of MERCHANTABILITY or FITNESS FOR A
# PARTICULAR PURPOSE. See the GNU General Public License
# for more details.
#
# You should have received a copy of the GNU General Public
# License along with this program; if not, write to the
# Free Software Foundation, Inc., 59 Temple Place, Suite
# 330, Boston, MA 02111-1307 USA
#
##########################################

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

