
1. **Navigate to Your ROS 2 Workspace:**

   ```bash
   cd ~/ros2_ws
   ```

2. **Clone the `ros1_bridge` Repository:**

   ```bash
   cd src
   git clone https://github.com/ros2/ros1_bridge.git
   ```

   <img width="591" alt="2-update ros2 version to match ros2" src="https://github.com/user-attachments/assets/fb6d7da1-df62-4c95-a184-f91dcf8ab8ae">

3. **Install Dependencies:**

   <img width="620" alt="1-install all dep" src="https://github.com/user-attachments/assets/8d6cce80-f8d5-4790-a664-d7b36b83faf3">

4. **Build the Workspace:**

   ```bash
   colcon build --symlink-install
   ```

<img width="570" alt="3-build correct dep" src="https://github.com/user-attachments/assets/a44dfe65-bcd9-4078-8595-0bc08635eb5c">

5. **Source the Workspace:**

   After building, source the setup file:

   ```bash
   source ~/ros2_ws/install/setup.bash
   ```

### 2. Verify `ros1_bridge` Installation

Make sure `ros1_bridge` is installed:

```bash
ros2 pkg list | grep ros1_bridge
```

This should list `ros1_bridge` if it is installed correctly.

### 3. Running the Bridge

Once `ros1_bridge` is installed and built, you can run the bridge:

```bash
ros2 run ros1_bridge dynamic_bridge
```

<img width="957" alt="7-run the brdg and pkg in sprated term" src="https://github.com/user-attachments/assets/4001ca84-f808-4f1f-a54f-25de02813d68">

### 4. Print from ROS1 to ROS2

<img width="957" alt="7-run the brdg and pkg in sprated term" src="https://github.com/user-attachments/assets/39b22fad-ac91-40f4-a30b-7192268c267d">
