# OGC.Engineering
### ogc_project_layered_development_demo - project level definition of a layered development demonstration set
developer contact - dustin ( at ) ogc.engineering

---

## Description:
* Demonstration of a layered development process for embedded systems
* Explores a user space bootloader, multiple embedded operating systems, and runs on multiple types of hardware

## File and Folder Planning:
* project folder ( this repository ) - contains documentation, certs, designs, etc. for creating embedded systems
    * deployments - hardware, firmware, and software collection along with build scripts for a single device
        * software folder - holds hardware independent sources
            * applications - high level guide of device operations
            * libraries - application support building blocks handling background operations and intermediate processes
        * firmware folder - holds hardware dependent sources
            * hal ( hardware abstraction layer(s) ) - interface/bridge between hardware specific and independent sources
            * drivers - collections of sources supporting advanced hardware specific features
            * csp ( chip support package(s) ) - collection of sources from manufaturers supporting hardware
        * hardware folder - holds hardware production files and descriptions headers
            * hardwae design folder - datasheets, schematics, pcb and enclosure procduction files
            * hardware description(s) - generic redirection and specific definition headers
