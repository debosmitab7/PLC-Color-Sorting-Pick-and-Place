# PLC-Based Color Sorting and Pick-and-Place System

## Overview

A PLC-based automated color sorting and pick-and-place system developed using
Siemens PLC and STEP 7 Ladder Logic.

The system detects the color of an object moving on a conveyor, stops the
conveyor, picks the object using a robotic arm, and places it into the
corresponding red, blue, or green bin.

## Objectives

- Automate color-based object sorting
- Control a conveyor and robotic pick-and-place mechanism using a PLC
- Implement sequential control using Ladder Logic
- Demonstrate sensor-based industrial automation
- Reduce manual intervention in repetitive sorting operations

## System Components

- Siemens S7 PLC
- Conveyor motor
- Object detection sensor
- Color sensor
- Robotic arm
- Gripper
- Home-position sensor
- Pick-position sensor
- Start/Stop push buttons
- Red, blue and green collection bins

## Software

- Siemens STEP 7
- SIMATIC Manager
- Ladder Logic

## System Architecture

```text
Start Button
     |
     v
Siemens PLC
     |
     +------------------+
     |                  |
 Conveyor          Color Sensor
     |                  |
Object Sensor      Color Detection
     |                  |
     +--------+---------+
              |
        PLC Decision
              |
              v
      Pick-and-Place Arm
        /      |      \
       /       |       \
 Red Bin    Blue Bin   Green Bin
