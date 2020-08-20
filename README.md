# Path Planer node
ROS node to interface with an ASV path planner

## Requirements
This package is meant to work in CCOMJHC's Project 11 simulation environment, the installation instructions for which are found <a href="https://github.com/CCOMJHC/project11_documentation/blob/master/SettingUpASimulationEnvironment.md">here</a>. It also uses a MPC ROS node, found <a href="https://github.com/afb2001/mpc">here</a>.

This package was developed solely on Ubuntu 18.04, so try anything else at your own risk.

## Installation
Install the <a href="https://github.com/CCOMJHC/project11_documentation/blob/master/SettingUpASimulationEnvironment.md">CCOMJHC Project 11 simulation environment</a>. MOOS-IvP components  are not required.

Installing the simulation environment will clone this repository and the associated <a href="https://github.com/afb2001/mpc">model predictive controller</a>. No additional setup is required.

There is a test scenario runner node that's in development, which is <a href="https://github.com/afb2001/test_scenario_runner.git">here</a>. It includes a suite of scenarios. See the README of that repository for instructions on how to use the test runner.

## Usage
See the simulation environment documentation for instructions on getting that running. The planner and controller nodes are included in the standard launch files. Once everything is running, use the dynamic_reconfigure window to switch the path follower to the path planner, in the mission_manager parameter section. 
