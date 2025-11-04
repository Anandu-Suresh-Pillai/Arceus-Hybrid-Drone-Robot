# Arceus-Hybrid-Drone-Robot

This project implements a dual-mode hybrid robot that can operate both as a quadcopter drone in the air and a self-balancing two-wheel rover on the ground.

This is an ongoing project.

![Arceus Drone Rover Hybrid](arceus_images/arc_image_1)

## Repository Structure

- `arceus_CAD/`
  - Contains CAD files for mechanical modeling and design.
  - Has a `README.MD` file.

- `arceus_code/`
  - Contains code for simulations and control.
  - Subfolders for simulation and package organization:
    - `simulation_code/arceus_minimal_sim_description/`
      - ROS (Robot Operating System) launch scripts (`launch/`)
      - Visualization configuration (`config/`)
      - URDF (Unified Robot Description Format) and mesh files for the quadcopter drone model.
      - `setup.py` for Python package setup.
      - Tests: code style (PEP257, Flake8), copyright.
    - `simulation_code/self_balancing_robot_description/`
      - ROS launch scripts (`launch/`)
      - Visualization configuration (`config/`)
      - URDF and mesh files for the self-balancing robot model.
      - `setup.py` for Python package setup.
      - Tests: code style (PEP257, Flake8), copyright.

- `arceus_docs/`
  - Documentation directory.

- `arceus_images/`
  - Contains related images.


## Major Functionality

- ROS launch files for both drone and rover in simulation environments (`gazebo.launch.py`, `display.launch.py`).
- URDF and mesh support in both simulation packages for realistic physical modeling.
- Ready-to-use Rviz visualization configuration for both modes.
- All code style follows PEP257 and Flake8, verified by test scripts in each module.

## Notable Files

- [LICENSE](LICENSE): MIT License
- [README.md](README.md): This file


## How to Use

- Each robot mode (drone and self-balancing rover) has separate ROS description packages for use in simulation.
- Launch scripts such as `gazebo.launch.py` and `display.launch.py` are available for both packages to visualize and simulate the robots in Gazebo and Rviz.

## Notes

- The repository is publicly available and uses Python as its main language.
- Designed for extensibility, with modular simulation packages for both robot modes.


## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.


> All information above is strictly based on the repository's files and content. No assumptions or external knowledge are included.
