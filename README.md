# SSD utility check #

# Overview #

This utilitu provides extensible "Quality of Life" information about the Solid State Drive (SSD):

 * TBW (Terra Bytes Written)
 * Average write rate (MB/day and GB/day)
 * Drive health in %
 * Online time

Which currently aren't shown by `smartctl` utility at this moment.

### Prerequisites ###

Before using launching this utility, make sure these tools are installed on your machine:

* `smartctl` (can be installed via running following command: `sudo apt install smartctl`)

### How to ###

* Clone repository `git clone https://reborn0105@bitbucket.org/aulanchik/ssd-info-check.git`
* Using a terminal access the folder: `cd <your-clone-path>/ssd-info-check`
* Give execution permissions to the utility: `sudo chmod +x ./ssd-info-check.sh`
* Execute the utility: `./ssd-info-check`

Note: Upon launching utility it will prompt for admin password. This happens due to `smartctl`
attempting to consult drive for specific information which isn't available for regular users.

### Testing ###

* Tested on Samsung SSD 860 (QVO/EVO/PRO) series. For other SSD series output might differ. 

### Contributors ###

Author: Artyom Ulanchik <artyom.u@outlook.com>
