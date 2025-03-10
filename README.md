#### 重要参考资料

PX4是一个开源的飞行控制系统（飞控软件），用于无人机（UAV）和其他自动化飞行平台。它支持多种飞行模式，包括自动飞行、手动飞行和半自动模式，并且可以控制各种类型的飞行器，如多旋翼、固定翼、VTOL（垂直起降）等。PX4提供强大的功能，如传感器数据融合、航迹规划、姿态控制和任务执行，并且与地面控制站软件（如QGroundControl）和通信协议（如MAVLink）兼容，广泛应用于学术研究、商业和消费级无人机中。

PX4 官方github

[PX4 Autopilot (github.com)](https://github.com/PX4)

PX4官方用户手册

[PX4 Autopilot User Guide | PX4 Guide (main)](https://docs.px4.io/main/zh/)

PX4官方开发者手册

[PX4 Development | PX4 Guide (main)](https://docs.px4.io/main/zh/development/development.html)



QGC（QGroundControl）是一个开源的地面控制站软件，用于与无人机进行通信和控制。QGC可以与PX4兼容，用于配置、监控和控制PX4飞行控制器。两者常常一起使用，QGC作为用户界面，PX4作为飞行控制系统。

QGC 用户手册

[QGroundControl User Guide | QGC Guide (master)](https://docs.qgroundcontrol.com/master/zh/qgc-user-guide/)

QGC 开发者手册

[QGroundControl Dev Guide | QGC Guide (master)](https://docs.qgroundcontrol.com/master/zh/qgc-dev-guide/index.html)



MAVLink（Micro Air Vehicle Link）是一种轻量级的通信协议，专门用于无人机（UAV）和地面控制站（GCS）之间的数据传输。它支持遥控、飞行状态监控、任务规划等功能，广泛应用于无人机系统，如PX4和ArduPilot。MAVLink允许通过串口、UDP、TCP等方式传输数据，具有高效、可靠的特点。

MAVLINK 开发者手册

[MAVLink Developer Guide | MAVLink Guide](https://mavlink.io/zh/)

MAVSDK 官网

[Introduction · MAVSDK Guide (mavlink.io)](https://mavsdk.mavlink.io/main/zh/index.html)



MAVROS是一个ROS（Robot Operating System）包，用于在ROS环境中与MAVLink协议兼容的飞行控制系统（如PX4和ArduPilot）进行通信。它通过提供与MAVLink消息的接口，使得ROS可以与无人机的飞行控制器进行数据交换、控制飞行任务、获取飞行状态等。MAVROS为ROS用户提供了与无人机交互的便利，包括控制命令、传感器数据和状态信息等，使得开发者可以在ROS框架中实现更复杂的无人机任务和功能。

mavros wiki

[mavros - ROS Wiki](https://wiki.ros.org/mavros)

ros wiki

[Documentation - ROS Wiki](https://wiki.ros.org/)



XTDrone 基于PX4的开源仿真平台，里面有很多搭建好的仿真场景

https://gitee.com/robih_shaun/XTDrone

FASTLAB 浙江大学的一个实验室团队，发布了许多PX4算法论文

http://zju-fast.com/

古月居 ROS社区

https://www.guyuehome.com/

超维空间科技 中文博主，发布了许多PX4的教程视频和博客文章，都较为完善

[南京超维空间科技的个人空间-南京超维空间科技个人主页-哔哩哔哩视频 (bilibili.com)](https://space.bilibili.com/479817593)

[超维空间科技-CSDN博客](https://blog.csdn.net/qq_38768959?spm=1018.2118.3001.5148)





#### 硬件

资料全部参考官方手册硬件栏目

[Hardware Hardware Selection & Setup | PX4 Guide (main)](https://docs.px4.io/main/en/hardware/drone_parts.html)

搭载PX4的飞控硬件只推荐官方的Pixhawk系列

[Pixhawk Standard Autopilots | PX4 Guide (main)](https://docs.px4.io/main/en/flight_controller/autopilot_pixhawk_standard.html)

PX4 支持许多将信号发送到 ESC(电调) 的常见协议：[PWM ESC](https://docs.px4.io/main/zh/peripherals/pwm_escs_and_servo.html)、[OneShot ESC](https://docs.px4.io/main/zh/peripherals/oneshot.html)、[DShot ESC](https://docs.px4.io/main/zh/peripherals/dshot.html)、[DroneCAN ESC](https://docs.px4.io/main/zh/dronecan/escs.html)、PCA9685 ESC（通过 I2C）和一些 UART ESC（来自 Yuneec）。

[Actuators | PX4 Guide (main)](https://docs.px4.io/main/en/actuators/)

PX4支持多种常见的遥控接收机协议，包括PPM、S.BUS、CRSF、DSM等，也支持一些特定厂商的协议（如TBS Crossfire、Express LRS、TBS Ghost等）。

[Radio Control Systems | PX4 Guide (main)](https://docs.px4.io/main/en/getting_started/rc_transmitter_receiver.html)

有关机载电脑

[Companion Computers | PX4 Guide (main)](https://docs.px4.io/main/en/companion_computer/)



#### 起飞

这方面的教程主要参考第三方资料，国内的中文资料在这方面也十分完善了

FastLab 浙大团队的教程，涉及组装硬件，烧录固件，起飞，只是想起飞的话看这个系列就可以

[【完结】从0制作自主空中机器人 | 开源 | 浙江大学Fast-Lab_哔哩哔哩_bilibili](https://www.bilibili.com/video/BV1WZ4y167me)

超维空间科技教程，比较深入，涉及ROS，PID调参，一些二次开发，可做参考

[南京超维空间科技的个人空间-南京超维空间科技个人主页-哔哩哔哩视频 (bilibili.com)](https://space.bilibili.com/479817593/channel/collectiondetail?sid=1627309&spm_id_from=333.788.0.0)





#### 二次开发

GitHub下载PX4源码

[PX4 Autopilot (github.com)](https://github.com/PX4)

官方开发者手册，十分重要

[PX4 Development | PX4 Guide (main)](https://docs.px4.io/main/en/development/development.html)

固件的二次开发

[南京超维空间科技的个人空间-南京超维空间科技个人主页-哔哩哔哩视频 (bilibili.com)](https://space.bilibili.com/479817593/channel/collectiondetail?sid=2162525)

mavros

[【ROS】MAVROS基础知识和使用-CSDN博客](https://blog.csdn.net/caiqidong321/article/details/132013439)

[自定义机架](https://blog.csdn.net/qq_38768959/article/details/124945512)
