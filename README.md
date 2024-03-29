# Little Red Rover

ROS enabled robots are (really) expensive, preventing many aspiring robotic engineers from accessing powerful ROS tools.

Little Red Rover (LLR) is a highly capable, differential drive, ROS 2 robot designed for an amateur budget.
While none of the rovers' specs are top of the line, LLR gives students, hobbyists, and educators a representative ROS 2 experience and an entry point into the wonderful world of research robotics.
Extensive development tooling, example code / projects, and documentation is provided to smooth the learning curve.

## Use Cases

Little Red Rover was developed with educational use in mind. Each rover is affordable enought to be funded by a small course fee, and the detailed documentation and tutorials provide a starting point for a full curriculum.

LLR is also perfect for robotics hobbyists interested in elevating their work. Breaking out of tinkery ecosystems like Arduino can be difficult, and LLR is an affordable starting point.

## Stackup

Little Red Rover is currently in developement, and the specs below may or may not be implemented already. For now, this section serves as a roadmap.

### Software
* ESP32 onboard, running [micro-ROS](https://micro.ros.org/)
    * Publishes sensor data and reacts to movement commands
* Dockerized development environment runs on any OS and communicates with the rover wirelessly over UDP
    * Interact with the robot just as you would any ROS node

### Hardware
* [FHL-LD20 Lidar](https://www.youyeetoo.com/products/youyeetoo-fhl-ld20)
* Custom circuit board integrated as the rovers body
* Wheel encoders and IMU for odometry
* Designed for low effort assembly and large scale production

## Capabilities

* ROS 2 navigation stack
    * SLAM
    * Path planning
    * Ect

## Repo Structure

* `/SOFTWARE`: ROS and micro-ROS code, along with the Docker developement infrastructure. See `/SOFTWARE/README.md` for more details
* `/HARDWARE`: KiCad PCB design files, and [SKiDL](https://github.com/devbisme/skidl) circuit description. See `/HARDWARE/README.md` for more details

## Thanks

LRR is part of my Masters of Engineering (MEng) thesis for Cornell University.

Special thanks to my advisor, [Professor Tapomayukh Bhattacharjee](https://robotics.cornell.edu/faculty/tapomayukh-bhattacharjee-bio/) of the [EmPRISE Lab](https://emprise.cs.cornell.edu/). LLR was inspired by his course, Foundations of Robotics, and his help on the project has been invaluable.
