# microbit_umidade
Utilização do Microbit para medir umidade

Resumo das funções e fluxo do código:

Variável reading: Armazena a leitura atual do sensor de umidade.

led.set_brightness(64): Define o brilho dos LEDs do display do micro

Função on_forever:

Ativa o sensor de umidade.

Lê o valor do sensor e o armazena na variável reading.
Desativa o sensor.

Exibe a leitura como um gráfico de barras no display LED.

Pausa por 5 segundos antes de repetir o processo.

Função on_button_pressed_a:

Exibe a leitura do sensor como um número no display LED quando o botão A é pressionado.

input.on_button_pressed(Button.A, on_button_pressed_a): Configura o micro
para chamar a função on_button_pressed_a ao pressionar o botão A.

basic.forever(on_forever): Inicia a execução contínua da função on_forever
