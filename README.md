Projekt został wykonany przy użyciu TurtleBot.
Klikając w lewą stronę okna publishera robot zacznie obracać się w lewo, klikając prawą stronę, w prawo.
Klikając górną część okna publishera robot zacznie poruszać się do przodu, w dolną stronę okna, do tyłu.

Aby uruchomić projekt należy:
<p> Uruchomić dwa okna terminala
 <p> W pierwszym oknie należy:
   <p> 1. Przejść do katalogu "projekt/camera_subscriber"
  <p>  2. Wpisać następujące komendy:
   <p> - source /opt/ros/humble/setup.bash
   <p> - source install/setup.bash
  <p>  - export TURTLEBOT3_MODEL=burger
  <p>  - export GAZEBO_MODEL_PATH=$GAZEBO_MODEL_PATH:`ros2 pkg \
        prefix turtlebot3_gazebo \
        `/share/turtlebot3_gazebo/models/
  <p>  - ros2 launch turtlebot3_gazebo empty_world.launch.py
 
<p>  W drugim oknie terminala należy:
<p>    1. Prześć do katalogu "projekt/camera_subscriber"
 <p>   2. Wpisać następujące komendy:
 <p>   - source /opt/ros/humble/setup.bash
 <p>   - source install/setup.bash
 <p>   - ros2 run camera_subscriber camera_node

<p> Program powinien wyświetlić puste okno publishera oraz wizualizację turtlebot w programie gazebo.



