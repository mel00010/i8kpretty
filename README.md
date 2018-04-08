# i8kpretty

## Summary
i8kpretty is a pretty printer for `/proc/i8k`.  `/proc/i8k` is used on Dell laptops to monitor the state of the fans, among other things.  However, this file has no labels for which numbers represent what information.  This program parses the file and outputs a nicely formatted table containing the parsed information.  


## Dependencies
* awk
* bash
* expand
* i8k
* GNU getopt

`sudo apt install 

## Ubuntu 16.04 Dependencies
* coreutils
* bash
* gawk
* i8kutils


`sudo apt install gawk i8kutils`

## Installation
Simply run `sudo make install`.   The program will be installed under `/usr/local/bin`.  


## Usage
When run without any arguments, i8kpretty displays the CPU temperature, the speed of the right fan, and the status of the right fan.  

| Short option   | Long option          | Description                                                                              |
|----------------|----------------------|------------------------------------------------------------------------------------------|
| `-h`           | `--help`             | Prints usage information then exits.                                                     |
| `-a`           | `--all`              | Enables the display of everything.  Equivalent to `-ibtclrLRAf`.                         |
| `-i`           | `--i8k-version`      | Enables the display of the format version of `/proc/i8k`.                                |
| `-b`           | `--bios-version`     | Enables the display of the BIOS version.                                                 |
| `-t`           | `--service-tag`      |	Enables the display of the laptop's service tag/serial number.                     |
| `-c`           | `--cpu-temp`         | Enables the display of the CPU temperature.                                              |
| `-s`           | `--fan-speed`        |	Enables the display of the speed of the left and right fans.  Equivalent to `-lr`. |
| `-l`           | `--left-fan-speed`   |	Enables the display of the speed of the left fan.                                  |
| `-r`           | `--right-fan-speed`  | Enables the display of the speed of the right fan.                                       |
| `-S`           | `--fan-status`       | Enables the display of the status of the left and right fans.  Equivalent to `-LR`.      |
| `-L`           | `--left-fan-status`  |	Enables the display of the status of the left fan.                                 |
| `-R`           | `--right-fan-status` |	Enables the display of the status of the right fan.                                |
| `-A`           | `--ac-status`        |	Enables the display of the status of the AC adapter.                               |
| `-f`           | `--fn-status`        |	Enables the display of the status of the function buttons.                         |


### Note
In the context of the options relating to fan status, a negative number indicates that the device is not present, 0 means off, 1 means low speed, and 2 means max speed.

For all of the other options, a negative number indicate that that device that is not present.


## Contributing
This project is licensed under the GNU General Public License version 3.  Feel free to submit a pull request if you make changes.
