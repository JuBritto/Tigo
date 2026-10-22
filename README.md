# Tigo - Mecanum Robot
## Códigos do Tigo

Github para salvar códigos do Tigo

## Comandos do Terminal:

### Comando para atualizar/compilar no arduino
nano ~/tigo_arduino/tigo_arduino/tigo_arduino.ino  
arduino-cli compile --fqbn arduino:avr:mega ~/tigo_arduino/tigo_arduino  
arduino-cli upload -p /dev/ttyUSB0 --fqbn arduino:avr:mega ~/tigo_arduino/tigo_arduino  

### Comando para o Teleop omnidirecional
source install/setup.bash  
ros2 run mecanum_serial_bridge custom_teleop

### Comando para rodar o nó de cmd_vel
source install/setup.bash  
ros2 run tigo_control custom_teleop

### Comando upload arduino notebook
nano MeuProjeto/MeuProjeto.ino  
arduino-cli compile --upload -p /dev/ttyUSB0 --fqbn arduino:avr:mega MeuProjeto

### Comando github
git clone git@github.com:lyssa-virus/TIGO.git tigo_ws
cd tigo_ws
git checkout -b julia
git push -u origin julia
