# i8kpretty

## Summary
i8kpretty is a pretty printer for /proc/i8k.  

## Dependencies
* awk
* bash
* expand
* i8k
* GNU getopt

## Installation

Simply run `sudo make install`.   The program will be installed under /usr/local/bin.  

## Usage
When run without any arguments, i8kpretty displays the CPU temperature, the speed of the right fan, and the status of the right fan.  

Option list:
* -h|--help:					Prints usage information
* -a|--all:						Enables the display of everything
* -i|--i8k-version				Enables the display of the format version of /proc/i8k
* -b|--bios-version				Enables the display of the BIOS version
* -t|--service-tag				Enables the display of the laptop's service tag/serial number
* -c|--cpu-temp					Enables the display of the CPU temperature
* -s|--fan-speed				Enables the display of the speed of the left and right fans
* -l|--left-fan-speed			Enables the display of the speed of the left fan
* -r|--right-fan-speed			Enables the display of the speed of the right fan
* -S|--fan-status				Enables the display of the status of the left and right fans
* -L|--left-fan-status			Enables the display of the status of the left fan
* -R|--right-fan-status			Enables the display of the status of the right fan
* -A|--ac-status				Enables the display of the status of the AC adapter
* -f|--fn-status				Enables the display of the status of the function buttons

## Contributing
This project is licensed under the GNU General Public License version 3.  Feel free to submit a pull request if you make changes.  

