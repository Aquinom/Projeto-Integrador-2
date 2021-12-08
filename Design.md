# Design

Acesso Rápido:

* [Concepção](https://github.com/Aquinom/Projeto-Integrador-2/blob/main/Concep%C3%A7%C3%A3o.md)
* [Design](https://github.com/Aquinom/Projeto-Integrador-2/blob/main/Design.md)
* [Implementação](https://github.com/Aquinom/Projeto-Integrador-2/blob/main/Implementa%C3%A7%C3%A3o.md)
* [Operação](https://github.com/Aquinom/Projeto-Integrador-2/blob/main/Opera%C3%A7%C3%A3o.md)

---

Definido as necessidades do projeto, é possível desenhar a maquete do circuito final no software Fritzing de forma que auxilie no processo de montagem. Também nesta etapa alguns dos sistemas vão ter suas funcionalidades avaliadas de forma individual. 

## Componentes Utilizados

| Componente |  Quantidade  |
| ------------------- | ------------------- |
|  Sensor de umidade e temperatura DHT11 |  1 |
|  Sensor de presença e movimento PIR |  1 |
|  Sensor de gás MQ-2 |  1 |
|  1x Micro Servo SG92R 9g TowerPro |  1 |
|  Módulo Sensor de Umidade/Nível Água Chuva |  1 |
|  Sensor ultrasônico HC-SR04|  1 |
|  Módulo Matriz de LED 8×8 com MAX7219|  1 |
|  Buzzer |  1 |
|  Display LCD 16×2 I2C Backlight Azul |  1 |

### Arduino Mega 2560 R3 

Cérebro do projeto, com seu núcleo ATmega2560 e 4KB de E2PROM, é a ferramenta de processamento perfeita para implementar a lógica de tomada de decisões e comunicação com sensores. 

### Sensor DHT11

Utiliza o princípio de resistência variável para medir umidade e um termistor NTC para medir temperatura, tudo isso no mesmo pacote. 

### Sensor PIR

Quando polarizado, este sensor piroelétrico manda um pequeno sinal ao ser submetido à radiação infravermelha, dessa forma agindo como um detector de objetos que possuem calor.

### Sensor MQ2

Quando submetido à atmosferas diferentes de ar limpo, a pequena quantidade de Dióxido de Estanho em seu interior tem sua condutividade alterado, permitindo que aja como um resistor variável.

### Servo SG92R

O motor escovado de corrente contínua em seu interior permite 180° de rotação e 2.5 Kg-cm de torque graças a suas engranagens de nylon e fibra de carbono. Recomendado utilizar um capacitor de 470uF entre VCC e GND para evitar surtos de energia ocasionados pelo servomotor.

### Sensor de Umidade

Descrição do componente.

### Sensor HC-SR04

Permite mensurar a distância de um objeto calculando o tempo que um pulso ultrassônico leva para atingir um objeto e retornar. Melhor utilizado em atmosferas de ar.

### Matriz de LED MAX7219

Recebe esse nome pois cada LED possui um endereço na matriz, um para linha e outro para coluna. Devido ao seu método construtivo apenas um LED pode ser acionado por vez, dessa forma para alcaçar um resultado que pareça constantemente aceso ao olho humano, todos os LED's devem ser acesos um por vez em um curto período de tempo (normalamente na faixa de 20 microsegundos). Se comunica com o Arduino através do protocolo I2C.

### Buzzer

Podendo ser do tipo ativo ou passivo. O primeiro não pode ser utilizado para se criar melodias, diferente do segundo que ao ter a frequência de alimentação alterada, permite a reprodução de sons mais complexos.

### Display I2C

Tela LCD que utiliza o protocolo serial I2C para transmissão dados. Neste projeto o Arduino MEGA é o controlador (mestre) e o display o periférico (escravo).

## Maquete Eletrônica

![image](https://user-images.githubusercontent.com/92688963/145125054-17db91c0-5587-447f-8d66-fe37137208cd.png)


