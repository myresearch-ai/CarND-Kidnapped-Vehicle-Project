# **CarND-Kidnapped-Vehicle-Project-6** 
[![Udacity - Self-Driving Car NanoDegree](https://s3.amazonaws.com/udacity-sdc/github/shield-carnd.svg)](http://www.udacity.com/drive)

Overview
---

This project implements & utilizes a **particle filter** to estimate & localize an autonomous car on the global map.

This project involves the Term 2 Simulator which can be downloaded [here](https://github.com/udacity/self-driving-car-sim/releases).

This repository includes two files that can be used to set up and install [uWebSocketIO](https://github.com/uWebSockets/uWebSockets) for either Linux or Mac systems. For windows you can use either Docker, VMware, or even [Windows 10 Bash on Ubuntu](https://www.howtogeek.com/249966/how-to-install-and-use-the-linux-bash-shell-on-windows-10/) to install uWebSocketIO. Please see the uWebSocketIO Starter Guide page in the classroom within the EKF Project lesson for the required version and installation scripts.

Once the installation for uWebSocketIO is complete, the main program can be built and run by doing the following from the project top directory.

1. mkdir build
2. cd build
3. cmake ..
4. make
5. ./particle_filter

Alternatively some scripts have been included to streamline this process, these can be leveraged by executing the following in the top directory of the project:

1. ./clean.sh
2. ./build.sh
3. ./run.sh

Directory Structure
---

```
root
|   build.sh
|   clean.sh
|   CMakeLists.txt
|   README.md
|   run.sh
|
|___data
|   |   
|   |   map_data.txt
|   
|   
|___src
    |   helper_functions.h
    |   main.cpp
    |   map.h
    |   particle_filter.cpp
    |   particle_filter.h
```

Implementation Flow Path (Algorithm)
---

The schematic below provides a visual summary and approach to implement the particle Filter (PF). For detailed breakdown of the PF, several resources exist on the web including udacity's nanodegree.

![process](https://user-images.githubusercontent.com/76077647/131680149-3ac2e4e0-5e2f-4c1e-b725-c19c18acebaf.JPG)

Code Style
---

Please (do your best to) stick to [Google's C++ style guide](https://google.github.io/styleguide/cppguide.html).

Results & Performance (Success Criteria)
---

If the particle filter successfully localizes the car, the simulator indicates the pass notification as shown with this implementation in the image below.!

#### Basis of success criteria:

- Accuracy: the particle filter should localize vehicle position and yaw to within the values specified in the parameters max_translation_error and max_yaw_error in src/main.cpp.

- Performance: the particle filter should complete execution within the time of 100 seconds.

![final_img](https://user-images.githubusercontent.com/76077647/131683942-7354ed33-ac05-42ba-812b-1fb5fe8715cf.JPG)

References & Credits
---

* udacity (self driving car nanodegree - particle filter module)
* course peers
