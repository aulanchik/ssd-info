# SSD utility check #

# Overview #

This utility provides extensible "Quality of Life" information about the Solid State Drive (SSD):

 * TBW (Terra Bytes Written)
 * Average write rate (MB/day and GB/day)
 * Drive health in %
 * Online time

Which currently aren't shown by `smartctl` unix utility at this moment.

### Prerequisites ###

Before using launching this utility, make sure these tools are installed on your machine:

* `smartctl` (can be installed via running following command: `sudo apt install smartctl`)

### How to ###

* Clone repository `git clone https://github.com/aulanchik/ssd-info.git`
* Using a terminal access the folder: `cd <your-clone-path>/ssd-info`
* Give execution permissions to the utility: `sudo chmod +x ./ssdinfo.sh`
* Execute the utility: `./ssdinfo`

Note: Upon launching utility it will prompt for admin password. This happens due to `smartctl`
attempting to consult drive for specific information which isn't available for regular users.

### Testing ###

* Tested on Samsung SSD 860 (QVO/EVO/PRO) series. For other SSD series output might differ. 
