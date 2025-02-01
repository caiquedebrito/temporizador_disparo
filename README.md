# Temporizador de um disparo (One Shot)

![Gif](./temporizador%20disparo.gif)

Com o emprego da função add_alarm_in_ms(), presente na ferramenta Pico SDK, projete um sistema de temporização para o acionamento de LEDs, que atua a partir do clique em um botão (pushbutton).

## Componentes

1) Microcontrolador Raspberry Pi Pico W. 
2) 03 LEDs (azul, vermelho e verde). 
3) 03 Resistores de 330 Ω. 
4) Botão (Pushbutton). 

## Requisitos implementados

1) Caso o usuário clique no botão (pushbutton), os três LEDs serão ligados (todos em nível alto). A partir da primeira rotina de atraso, ocorrerá uma mudança de estado para dois LEDs ligados e, em seguida, apenas um. 
2) O temporizador do alarme deve ser ajustado para um atraso de 3 segundos (3.000ms), entre os estados de acionamento dos LEDs. 
3) A mudança de estado dos LEDs deve ser implementa em funções de call-back do temporizador. 
4) O botão só pode alterar o estado dos LEDs quando o último LED for desligado. Deste modo, durante a execução das rotinas de temporização, o botão não pode iniciar uma nova chamada da 
função call-back. 
5) Com o emprego da Ferramenta Educacional BitDogLab, faça um experimento com o código deste exercício utilizando o LED RGB – GPIOs 11, 12 e 13 e o Botão A, GPIO 05. 
6) Opcional: Implementar uma rotina em software para atenuação do efeito bouncing no botão (software debounce).

## Como executar o projeto

### Pré-requisitos

- Git
- CMake
- Ferramentas de desenvolvimento para Raspberry Pi Pico
- Visual Studio Code com as extensões recomendadas
- Extensão do Wokwi

### Passos

1. Clone o repositório
Abra o terminal e execute o comando:
```
git clone https://github.com/caiquedebrito/temporizador_disparado.git
cd temporizador_periodico
```

2. Abra o projeto no VS Code
```
code .
```

3. Compile o projeto com a extensão CMake

4. Clique no arquivo diagram.json para abrir o simulador wokwi

5. Execute o projeto