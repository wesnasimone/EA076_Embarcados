## Estimativa da frequência de rotação do eixo de um motor a partir de encoder óptico     

Esse programa tem por objetivo estimar a frequência de rotação
do motor DC através de um encoder óptico. Essa estimativa é
mostrada através do monitor serial a cada 0.8s. Para isso,
foram desenvolvidas duas rotinas de interrupção: uma baseada
na interrupção por timer, para contar o tempo de estimação da
frequência, e a outra baseada em interrupção externa que ocorre 
a cada mudança de borda coletada do pino do encoder. Essa última
interrupção é utilizada para auxiliar no calculo da frequência de 
rotação, que é dada por

f = Np/(N*T) [Hz], onde

Np --> é o número de pulsos gerados pelo encoder dentro de um intervalo
de tempo T;
T --> é o período que se deseja estimar a frequência;
N --> é o número de pulsos que o encoder gera em uma volta.

Note que T é definido pela interrupção de timer e Np pela interrupção
externa. N já é um valor conhecido, e no caso para o motor usado vale 2.
