# Cmod S7 Root Repository

This repository is designed to offer a unified and comprehensive approach to all of the aspects of the demos that we provide for the Cmod S7, across multiple tools. By cloning this repo recursively you will receive the repositories for Vivado projects (HW), and Vitis workspaces (SW). Each submodule may have its own submodule dependencies which will also be pulled when cloning. An important aspect of this structure is the fact that the SW heavily depends on hardware hand-off files from the HW repository.

This repository also provides the release point for project and image files exported from the various tools involved. Releases provide files that are directly usable, without requiring the use git or any scripting systems. To get access to these files, visit this repository's releases page, find a release for a demo you may be interested in, and download the files therein. For additional documentation on individual demos, and how to use these releases, visit the READMEs for each demo, found on their respective master branches in this repository:

* [Cmod S7-25 Out-of-Box Demo](FIXME)
* [Cmod S7-25 XADC Demo](FIXME)

For more information about the Cmod S7, visit its [Resource Center](https://reference.digilentinc.com/reference/programmable-logic/cmod-s7/start) on the Digilent Wiki.

Each branch of this repository represents a different project with preset functionality. When checking out a branch, all the submodules will be automatically configured to the same branch, thus providing a unified flow between all the submodules. For details about the individual functionality of the submodules, please refer to the README.md files within the submodules.

For a detailed structural description of this repository and it's submodules, along with the branching system, please visit [Digilent FPGA Demo Git Repositories](https://reference.digilentinc.com/reference/programmable-logic/documents/git).