# Cmod S7 Root Repository

This repository is designed to offer a unified and comprehensive approach to all of the aspects of the demos that we provide for the Cmod S7, across multiple tools. By cloning this repo recursively you will receive the repositories for Vivado projects (HW), and Vitis workspaces (SW). Each submodule may have its own submodule dependencies which will also be pulled when cloning. An important aspect of this structure is the fact that the SW heavily depends on hardware hand-off files from the HW repository.

This repository also provides the release point for project and image files exported from the various tools involved. Releases provide files that are directly usable, without requiring the use git or any scripting systems. To get access to these files, visit this repository's releases page, find a release for a demo you may be interested in, and download the files therein.

Each branch of this repository represents a different project with preset functionality. Additional documentation on these demos can also be found on the Digilent wiki. Setup instructions for each demo can be found in READMEs within each demo's master branch.

| Wiki Page | README |
|-----------|--------|
| [Cmod S7-25 Out-of-Box Demo](https://reference.digilentinc.com/reference/programmable-logic/cmod-s7/oob-demo/staging) | [25/OOB/master README](https://github.com/artvvb/Cmod-S7/tree/25/OOB/master) |
| [Cmod S7-25 Microblaze XADC Demo](https://reference.digilentinc.com/reference/programmable-logic/cmod-s7/xadc-demo/staging) | [25/XADC/master README](https://github.com/artvvb/Cmod-S7/tree/25/XADC/master) |

For more information about the Cmod S7, visit its [Resource Center](https://reference.digilentinc.com/reference/programmable-logic/cmod-s7/start) on the Digilent Wiki.

For a detailed structural description of this repository and it's submodules, along with the branching system, and how to interact with this repository through git, please visit [Digilent FPGA Demo Git Repositories](https://reference.digilentinc.com/reference/programmable-logic/documents/git).

## Cmod S7-25 Out-Of-Box Demo Setup Instructions
- Download and extract the most recent release ZIP archive from this repository's Releases Page.
- Open the project in Vivado 2020.1 by double clicking on the included XPR file found at `<archive extracted location>/vivado_proj/Cmod-S7-25-OOB.xpr`.
- In the Flow Navigator panel on the left side of the Vivado window, click Open Hardware Manager.
- Plug the Cmod S7 into the computer running Vivado using a MicroUSB cable.
- Open a serial terminal emulator (such as TeraTerm) and connect it to the Cmod S7's serial port, using a baud rate of 9600.
- In the green bar at the top of the window, click Open target. Select "Auto connect" from the drop down menu.
- In the green bar at the top of the window, click Program device.
- In the "Program Device" Wizard, enter `<archive extracted location>/vivado_proj/Cmod-S7-25-OOB.runs/impl_1/top.bit` into the "Bitstream file" field. Then click Program.
- The demo will now be programmed onto the Cmod S7. See the Introduction section of this README for a description of how this demo works.