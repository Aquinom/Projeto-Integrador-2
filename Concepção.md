# Concepção

Acesso Rápido:

* [Concepção](https://github.com/Aquinom/Projeto-Integrador-2/blob/main/Concep%C3%A7%C3%A3o.md)
* [Design](https://github.com/Aquinom/Projeto-Integrador-2/blob/main/Design.md)
* [Implementação](https://github.com/Aquinom/Projeto-Integrador-2/blob/main/Implementa%C3%A7%C3%A3o.md)
* [Operação](https://github.com/Aquinom/Projeto-Integrador-2/blob/main/Opera%C3%A7%C3%A3o.md)

---

Este projeto tem como objetivo desenvolver todos os aspectos de automação para uma casa inteligente, desde sua ideia inicial até a operação no mundo real. Através do método CDIO e empregando princípios básicos de domótica, será desenvolvido um sistema eletrônico de baixo custo capaz de gerenciar vários aspectos de uma residência trazendo conforto, comodidade e segurança.

Abaixo estão algumas das funções a serem implementadas:

* Central de monitoramento baseada em Arduino para tomada de decisões.
* Sensoriar temperatura e abrir ou fechar uma janela para refrigerar a casa. Deve ter prioridade menor que o sensor de gás.
* Sensoriar a presença de pessoas e disparar o sistema de alarme (buzzer).
* Sensoriar vazamento de gás e então desativar componentes eletrônicos que possam gerar faíscas e disparar um alarme. Em baixas concentrações abrir a janela.
* Controlar um atuador ligado a uma janela.
* Sensor de chuva avisando o morador da residência que está a chover e fechar as janelas. Deve ter prioridade menor que o sensor de gás.
* Painel para monitoramento e avisos.

![PI2 drawio (2)](https://user-images.githubusercontent.com/92688963/139969140-f6a0feef-729a-44d8-971e-1e9b81ce0097.png)

## Hardware

* 1x Arduino Mega 2560 R3
* 1x Sensor de umidade e temperatura DHT11
* 1x Sensor de presença e movimento PIR
* 1x Sensor de gás MQ-2
* 1x Micro Servo SG92R 9g TowerPro
* 1x  Módulo Sensor de Umidade/Nível Água Chuva
* 1x Módulo Relé 5 V
* 1x Sensor ultrasônico HC-SR04
* 1x Módulo Matriz de LED 8×8 com MAX7219
* 1x Buzzer
* 1x Display LCD 16×2 I2C Backlight Azul
