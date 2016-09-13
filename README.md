# CMSIS Version 5

CMSIS Version 5.0.0 is now available as beta release, but will need further refinement as we are reviewing the feedback that we have got via various channels. We are scheduling the final release for November 2016.

This GitHub repository reflects our current development stage and is constantly updated.

The [pre-built documentation](http://arm-software.github.io/CMSIS_5/General/html/index.html) is available under http://arm-software.github.io/CMSIS_5/General/html/index.html

Use *Issues* to provide feedback and report problems for CMSIS Version 5. Note that this repository gives our users and partners contiguous access to the CMSIS development. It allows you to review the work and provide feedback or create pull requests for contributions.

## Implemented Enhancements
 - Support for ARMv8-M Architecture (Mainline and Baseline)

 - CMSIS-RTOS API and RTX reference implementation with several enhancements:
     - Dynamic object creation, Flag events, C API, additional thread and timer functions

## Futher Planned Enhancements
 - CMSIS-RTOS API Secure and Non-Secure support, multi-processor support

 - Improvements for Cortex-A / M hybrid devices (focus on Cortex-M interaction)

 - CMSIS-Pack 
     - Additions for generic example, project templates, multiple download portals
     - Adoption of IAR Flash Loader technology

For further details see also the [Slides of the Embedded World CMSIS Partner Meeting](https://github.com/ARM-software/CMSIS_5/blob/master/CMSIS_EW2016.pdf).

## Directory Structure

| Directory       | Content                                        |                
| --------------- | ---------------------------------------------- |
| CMSIS/Core      | CMSIS-Core related files (for release)         |
| CMSIS/DAP       | CMSIS-DAP related files and examples           |
| CMSIS/Driver    | CMSIS-Driver API headers and template files    |
| CMSIS/DSP       | CMSIS-DSP related files                        |
| CMSIS/RTOS      | RTOS v1 related files (for Cortex-M)           |
| CMSIS/RTOS2     | RTOS v2 related files (for Cortex-M & ARMv8-M) |
| CMSIS/DoxyGen   | Source of the documentation                    |
| CMSIS/Utilities | Utility programs                               |

## Generate CMSIS Pack for Release

This GitHub development repository contains already pre-build libraries of various libraries (DSP, RTOS, RTOS2).
These libraries are validated for release.

To build a complete CMSIS pack for installation the following additional tools are required:
 - **doxygen.exe**    Version: 1.8.6 (Documentation Generator)
 - **mscgen.exe**     Version: 0.20  (Message Sequence Chart Converter)
 - **7z.exe (7-Zip)** Version: 16.02 (File Archiver)
  
Using these tools, you can generate on a Windows PC:
 - **CMSIS Software Pack** using the batch file **gen_pack.bat** (located in ./CMSIS/Utilities). This batch file also generates the documentation.
  
 - **CMSIS Documentation** using the batch file **genDoc.bat** (located in ./CMSIS/Doxygen). 

The file ./CMSIS/DoxyGen/How2Doc.txt describes the rules for creating API documentation.

## License

ARM CMSIS is licensed under Apache-2.0.

## Contributions and Pull Requests

Contributions are accepted under Apache-2.0. Only submit contributions where you have authored all of the code.
