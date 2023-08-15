# INA219 ROS 2 Driver

This repository contains a ROS 2 driver for the INA219 current sensor from Adafruit. The driver reads voltage, current, and power data from the sensor and publishes it as ROS 2 topics.

## Table of Contents

- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Usage](#usage)
- [Topics](#topics)
- [Contributing](#contributing)

## Prerequisites

- ROS 2 (Humble Hippo or later)
- C++17 compatible compiler
- i2c-tools (for accessing the I2C bus on Linux)

## Installation

1. Navigate to your ROS 2 workspace's `src` directory.
    ```bash
    cd ~/ros2_ws/src/
    ```

2. Clone the repository.
    ```bash
    git clone [YOUR_REPOSITORY_LINK]
    ```

3. Build the package.
    ```bash
    colcon build --packages-select ina219_driver
    ```

4. Source your workspace.
    ```bash
    source ~/ros2_ws/install/setup.bash
    ```

## Usage

To run the INA219 node:

```bash
ros2 run ina219_driver ina219_node
```

## Topics
- /ina219/bus_voltage: Publishes the bus voltage in volts.
- /ina219/current: Publishes the current in amperes.
- /ina219/power: Publishes the power in watts.

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change. 

