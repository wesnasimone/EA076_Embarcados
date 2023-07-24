# EA076_Embarcados 🤖

Essa disciplina teve por finalidade desenvolver dois projetos utilizando o microcontrolador Arduino UNO.

### Projeto I: Controlador de Ventilador de Teto
  
Esse projeto teve por objetivo desenvolver um controlador
de ventilador de teto, explorando conceitos de transmissão
serial, protocolo I2C, display LCD, display de sete segmentos,
encoder óptico + schmitt trigger, ponte H (L293D), 
expansor de portas (PCF8574), decodificador de display 
de sete segmentos (CD4511B) e módulo bluetooth. 
Assim, a função do programa é controlar o motor DC através
de comandos enviados via bluetooth (mas também pode ser
enviado via serial) e exibir o estado do motor (VENTILACAO, 
EXAUSTOR, PARADO e o valor do duty cycle atual) em um display 16x2. 
Além disso, através do acionamento de um display de sete segmentos 
é informado a todo momento o valor da velocidade atual.

O seguinte link mostra o funcionamento do projeto I: [Projeto I](https://drive.google.com/file/d/1BjrbBGYjtxeWDO4zEh8ldHjUshyBKO-7/view)

### Projeto II: Datalogger

Esse projeto teve como objetivo construir um datalogger, isto é,
um dispositivo que coleta dados ambientais, no caso a temperatura ambiente,
e os armazena ao longo do tempo. Assim, explorou-se o conceito de
máquina de estados, protocolo I2C, transmissão serial, bem como
o uso de display LCD, display de sete segmentos, sensor de temperatura
(LM35), expansor de portas (PCF8574), decodificador de display 
de sete segmentos (CD4511B), teclado matricial e uma memória EEPROM (AT24C16).

O seguinte link mostra o funcionamento do projeto II: [Projeto II](https://drive.google.com/file/d/1NLcIG2gLZQWUlSuNDIRBFAI37bLwspUP/view)
