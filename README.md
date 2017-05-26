## Dali - Mark, Annotate, Augment

Dali is an application for the Microsoft HoloLens that allows a user to **augment** spaces by **marking** important locations and **annotating** them with notes, task-lists, images, and webpages.


### Use-Cases

The application is general enough to be used in various spaces, from marking your personal house to marking an office space or datacenter or even an industrial plant, for example:

- Home
	- Mark apartment for incoming guests to inform them about the nuances of the living area.
	- Show vacation readiness list next to door. (A/C set, windows closed, neighbors informed, post delivery suspended) 
	- Point repairman to broken appliance.
	- Show list of things to be repaired next to broken appliance.

- Datacenter
	- Point to defective compute node.
	- Show realtime metrics for a network device next to the device.
	- Show list of running containers on a compute node.

All those lists, notes, and images at the marked spots can be update in realtime through an API.


### Architecture

At its core Dali consists of following components:

![diagram](https://github.com/att-innovate/dali/blob/master/assets/dali-architecture.png)

Those core components are typically used in following sequence:
 
1. The Dali-HoloLens application is used to **mark** important locations in the space.
2. The Dali-Mgmt application or the API offered by the Dali-Server is used to **annotate** those previously marked locations by assigning notes, task-lists, images, or urls.
3. The HoloLens is then used to observe the now **augmented** space.


### Installation

#### Dali-HoloLens
The Dali-HoloLens project and its C# code can be found at 
[github.com/att-innovate/dali-hololens](https://github.com/att-innovate/dali-hololens).

#### Dali-Mgmt
The Dali-Mgmt project and its Javascript/React Native based code can be found at [github.com/att-innovate/dali-mgmt](https://github.com/att-innovate/dali-mgmt).

#### Dali-Server
And the Dali-Server Go code and its project are at [github.com/att-innovate/dali-server](https://github.com/att-innovate/dali-server).


### Team

This platform got built by Sarah Radzihovsky as part of an internship project at AT&T Foundry. Engineering lead and mentor was Marcel Neuhausler.
