# Cmod S7 Root Repository

This repository is designed to offer a unified and comprehensive approach to all of the aspects of the demos that we provide for the Cmod S7, across multiple tools. By cloning this repo recursively you will receive the repositories for Vivado projects (HW), and Vitis workspaces (SW). Each submodule may have its own submodule dependencies which will also be pulled when cloning. An important aspect of this structure is the fact that the SW heavily depends on hardware hand-off files from the HW repository.

This repository also provides releases containing project and image files used by the various tools involved. Releases provide files that are directly usable, without requiring the use git or any scripting systems. Documentation of each demo, as well as instructions for using their releases, can be found by visiting the corresponding pages on the Digilent Wiki, links below. All releases in this repository can be found in this repository's [releases page](https://github.com/artvvb/Cmod-S7/releases), however, use of the wiki pages to find specific well-tested releases is advised.

| Name and Wiki Link | Description | Demo Master Branch | Submodules Used |
|--------------------|-------------|--------------------|-----------------|
| [Cmod S7-25 Out-of-Box Demo](https://reference.digilentinc.com/reference/programmable-logic/cmod-s7/oob-demo/staging) | A simple hardware-only design using the LEDs, buttons, and USBUART Bridge | 25/OOB/master | HW |
| [Cmod S7-25 Microblaze XADC Demo](https://reference.digilentinc.com/reference/programmable-logic/cmod-s7/xadc-demo/staging) | Uses a Microblaze soft core processor and analog input pins to measure and print voltages | 25/XADC/master | HW, SW |

For more information about the Cmod S7, visit its [Resource Center](https://reference.digilentinc.com/reference/programmable-logic/cmod-s7/start) on the Digilent Wiki.

For instructions on how to use this repository with git, and for additional documentation on the submodule and branch structures used, please visit [Digilent FPGA Demo Git Repositories](https://reference.digilentinc.com/reference/programmable-logic/documents/git) on the Digilent Wiki. Note that use of git is not required to use this demo. Digilent recommends the use of project releases, for which instructions can be found in each demo wiki page, linked in the table of demos, above.

Demos were moved into this repository during 2020.1 updates. History of these demos prior to these updates can be found in their old repositories, linked below:
* [Cmod S7-25 Out-of-Box Demo](https://github.com/Digilent/Cmod-S7-25-OOB)
* [Cmod S7-25 Microblaze XADC Demo](https://github.com/Digilent/Cmod-S7-25-XADC)