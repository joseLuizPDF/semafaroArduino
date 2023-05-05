# semafaroArduino
O código é escrito na linguagem C++ e é destinado para ser executado em uma placa Arduino. 
A linguagem C++ é comumente usada para programar microcontroladores como o Arduino, que é uma plataforma de hardware para prototipagem eletrônica.
Este código é uma implementação simples de um semáforo de trânsito controlado por um potenciômetro que regula o tempo de troca de sinais.

Os primeiros seis comandos declaram as constantes para os pinos que serão utilizados como saídas para os LEDs dos semáforos. 
O semáforo 1 utiliza os pinos 2, 3 e 4 para verde, amarelo e vermelho, respectivamente. O semáforo 2 utiliza os pinos 6, 7 e 8 para verde, amarelo e vermelho,
respectivamente.

Em seguida, no método setup(), são configurados os pinos como saída.

O método loop() inicia lendo o valor do potenciômetro com o comando analogRead(). O valor lido é então mapeado para um valor entre 10000 e 120000 com o comando map(). 
O valor mapeado é armazenado na variável outputValue.

O semáforo é então controlado por uma série de comandos digitalWrite(), que acionam ou desligam os LEDs dos semáforos de acordo com um padrão de sinalização específico. 
Os comandos delay() são utilizados para controlar o tempo de cada sinal.

O código termina com um loop infinito while(true){} que mantém o semáforo no estado vermelho para ambos os lados do trânsito.
