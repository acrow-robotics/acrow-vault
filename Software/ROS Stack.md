[ROS 2 on Raspberry Pi — ROS 2 Documentation: Humble documentation](https://docs.ros.org/en/humble/How-To-Guides/Installing-on-Raspberry-Pi.html)

We tried the first option **Ubuntu Linux on Raspberry Pi with binary ROS 2 install** but we had issues with getting other things, such as PiJuice and the Pico SDK, working as they were designed for Raspberry Pi OS. Therefore, we will take the second option [Raspberry Pi OS with ROS 2 in docker](https://docs.ros.org/en/humble/How-To-Guides/Installing-on-Raspberry-Pi.html#raspberry-pi-os-with-ros-2-in-docker "Permalink to this heading") 
## Raspberry Pi OS with ROS 2 in docker

Raspberry Pi OS 64 bit version is [available here](https://www.raspberrypi.com/software/operating-systems/).

Raspberry Pi OS is based on Debian which receives Tier 3 support, but it can run Ubuntu docker containers for Tier 1 support.

After flashing the OS, [install Docker](https://docs.docker.com/engine/install/debian/#install-using-the-convenience-script).

The official OSRF ROS 2 Docker container definitions can be found [here](https://github.com/osrf/docker_images/).

Then do:
```bash
docker pull osrf/ros:humble-desktop
```
and
```bash
docker run -it osrf/ros:humble-desktop
```
