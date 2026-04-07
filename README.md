# Radar Ultrassônico com Arduino
 
Radar de curto alcance usando Arduino UNO, sensor ultrassônico HC-SR04 e servo motor SG90, com visualização em tempo real no Processing.
 
## Como funciona
 
O servo gira o sensor de 15° a 180°. A cada grau, o HC-SR04 mede a distância até o objeto mais próximo (alcance máximo: 40 cm). Os dados são enviados via porta serial e exibidos como um radar no Processing.
 
## Hardware
 
- Arduino UNO
- Sensor ultrassônico HC-SR04
- Servo motor SG90
- Breadboard + jumpers
 
### Pinagem
 
| Componente | Pino Arduino |
|---|---|
| Servo (sinal) | 12 |
| HC-SR04 Trig | 11 |
| HC-SR04 Echo | 10 |
 
VCC no 5V, GND no GND.
 
## Software
 
- **Arduino IDE** — `sonar_arduino.ino` (código do microcontrolador)
- **Processing** — `radar_display.pde` (interface gráfica do radar)
 
### Como rodar
 
1. Carregue o código `.ino` no Arduino pelo Arduino IDE.
2. Feche o Serial Monitor.
3. Abra o `.pde` no Processing e ajuste a resolução na linha `size()` e a porta serial (`COM3`) conforme seu setup.
4. Rode o sketch no Processing.
 
## Autores
 
- [alenarth](https://github.com/alenarth)
- [caiovfaria](https://github.com/caiovfaria)
- [Joao-Thees] (https://github.com/Joao-Thees) 