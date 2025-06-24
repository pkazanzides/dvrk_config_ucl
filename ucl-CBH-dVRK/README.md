dVRK configuration files for ucl-CBH-dVRK
=========================================

## June 2025 Status

 * PSM2 (S/N 21653): Encoder 2 (linear translation) does not work
 * PSM3 (S/N 25389): Encoder 1 (second axis) does not work
 * PSM2 controller:  FPGA #1 (S/N 6007-041) has broken Firewire ports (was removed from enclosure)
 * Ethernet interface ("udp") is too slow, especially when using SUJ
 * Instrument detection does not work; verified that PSM2 controller has dMIB Rev F, with jumpers set for 1-wire interface; not certain if dMIB Rev F was used in other controllers.
 * Increased current limit for ECM brake on second axis.
 * Currently using dVRK Software Version 2.1.0 and Firmware Rev 7.

## New files

 * `console-SUJ-ECM-MTML-PSM1-MTMR.json`: Use MTML to teleoperate PSM1; both MTMs to teleoperate ECM
 * `console-SUJ-ECM-MTML-MTMR-PSM1.json`: Use MTMR to teleoperate PSM1; both MTMs to teleoperate ECM

## Future tasks

 * Update dVRK software and firmware
 * Figure out why automatic instrument detection is not working
 * Replace broken FPGA in PSM2 controller
 * Fix or replace broken PSM2 and PSM3, or swap patient cart with other system
