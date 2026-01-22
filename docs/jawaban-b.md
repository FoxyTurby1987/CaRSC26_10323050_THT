* Dasar Pemrograman
  
* Firmware dan Sistem Benah
  1. Firmware (Links are [here](https://www.ibm.com/think/topics/firmware) and [here](https://www.geeksforgeeks.org/operating-systems/what-is-firmware/))
     Firmware can be thought of as 'Software for Hardware', it is the software that is pre-downloaded on our hardware (i.e. BIOS), and is responsible in making the hardware work. Its difference from software is:
     1. It's already inside the system
     2. It can't be erased as it's used to ensure the hardware runs (i.e. booting up the computer)  
     Firmware is there to ensure the UAV's hardware works as intended
  2. Real Time Operating System (RTOS) (Links are [here](https://www.ibm.com/think/topics/real-time-operating-system) and [here](https://www.unmannedsystemstechnology.com/expo/real-time-operating-systems/))
     A RTOS is meant as an operating system for time sensitive tasks, tasks that require microsecond precision. In UAV's, RTOS is important to ensure safety, and effectivity in missions with tight time constraints (i.e. in a competition)
  3. Basics of Serial Communication (UART,SPI,I2C) (Links are [here](https://theembeddedgeorge.github.io/theEmbeddedNewTestament.github.io/Communication_Protocols/Serial_Communication_Fundamentals.html))
     Serial Communication is, in essence, data transfer through one bit at a time. Different from Parallel Communication that does data transfer through multiple bits at a time

      For a UAV, Serial Communication allows bits of information to pass one at a time between different components, ensuring good communication between them in doing tasks
* Jurusan Control & Perception
  1. Basic concepts in ROS
     1. Node ([link](https://wiki.ros.org/Nodes))  
        Processes that do computation
     2. Topics ([link](https://wiki.ros.org/Topics))  
        Connectors connecting between nodes, allowing the exchange of information between
     3. Services ([link](https://wiki.ros.org/Services))  
        Mechanism on how two nodes communicate with each other (sender/receiver type)
     4. Parameters ([link](https://docs.ros.org/en/kilted/Concepts/Basic/About-Parameters.html))  
        Configure nodes without changing the code
     5. Actions ([link](https://docs.ros.org/en/rolling/Tutorials/Beginner-CLI-Tools/Understanding-ROS2-Actions/Understanding-ROS2-Actions.html))  
        Similar to services, but can be cancelled and continuously send feedback, instead of services, which give one response
* Jurusan Ground Control Station
