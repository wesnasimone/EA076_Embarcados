## Acionamento do motor CC

Esse programa tem por objetivo controlar o sentido e velocidade
do motor CC por meio de uma ponte H (L293D). Para isso, foram
desenvolvidas quatro rotinas, uma associada ao giro no sentido
horário, outra no sentido anti-horário e a terceira relacionada
a parada do motor. A quarta função recebe como parâmetros o sentido
e a velocidade e só então chama uma das três funções anteriores.
A velocidade é calculada através do duty cycle (porcentagem de tempo
que o sinal ficará em nível alto). Assim, o argumento da quarta 
função é a porcentagem do duty cycle.
Por fim, no loop principal do programa uma pequena rotina foi
desenvolvida para testar os sentidos de rotação e valores de
duty cycle.
