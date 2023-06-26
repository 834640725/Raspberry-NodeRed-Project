# Raspberry-NodeRed-Project
Internet of Things Project
设计制作只属于自己的一套物联网生态，实现万物皆可控，功能随意拓展。本次的DEMO包含4个基础功能，分别是现场环境监测、设备参数监测、智慧照明、设备控制。先对这4个功能进行分析，现场环境监测功能实现对环境的温度、湿度进行监测，那硬件上就需要用到温湿度传感器。因为应用环境就是家用，所以传感器我选择DHT11就足够了。
设备参数监测功能实现对设备的电压、电流进行监测，硬件就需要电流、电压采集模组。这里为了便于展示功能，我只对功能进行模拟，所以，电流采集范围设置为DC 0至1.5安，电压采集范围设置为DC 0至30伏，使用电子负载作为假负载。电流采样使用一个1欧姆的精密电阻采样，电压采样由一个1K电阻和10K电阻进行分压采样。
智慧照明功能实现对环境光强监测，同时，还能调节灯光的亮度，硬件就需要光强传感器、照明装置以及驱动器。光强传感器选择TEMT6000，它可以将0-1000流明的光强转换为电流的形式，通过一个10K电阻进行采样；照明装置我采用1组12瓦的LED进行模拟，驱动器使用光耦隔离模块和MOS管，通过PWM 的方式控制LED的亮度。
设备控制功能实现对设备开关控制，硬件就需要用到电控器件。这里我使用一个带光耦隔离的继电器模组进行演示，通过控制继电器的开闭，实现设备开关控制。
