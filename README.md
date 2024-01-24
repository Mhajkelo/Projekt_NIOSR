Projekt został wykonany przy użyciu TurtleBot.
Klikając w lewą stronę okna publishera robot zacznie obracać się w lewo, klikając prawą stronę, w prawo.
Klikając górną część okna publishera robot zacznie poruszać się do przodu, w dolną stronę okna, do tyłu.

Aby uruchomić projekt należy:
Uruchomić dwa okna terminala
  W pierwszym oknie należy:
    1. Przejść do katalogu "projekt/camera_subscriber"
    2. Wpisać następujące komendy:
    - source /opt/ros/humble/setup.bash
    - source install/setup.bash
    - export TURTLEBOT3_MODEL=burger
    - export GAZEBO_MODEL_PATH=$GAZEBO_MODEL_PATH:`ros2 pkg \
      prefix turtlebot3_gazebo \
      `/share/turtlebot3_gazebo/models/
    - ros2 launch turtlebot3_gazebo empty_world.launch.py
 
  W drugim oknie terminala należy:
    1. Prześć do katalogu "projekt/camera_subscriber"
    2. Wpisać następujące komendy:
    - source /opt/ros/humble/setup.bash
    - source install/setup.bash
    - ros2 run camera_subscriber camera_node

Program powinien wyświetlić puste okno publishera oraz wizualizację turtlebot w programie gazebo.



