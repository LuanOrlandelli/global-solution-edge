# global-solution-edge
Global Solution - Edge Computing

# GLOBAL SOLUTION 01 EDGE COMPUTING

# Projeto: Monitoramento de Iluminação Subaquática com Arduino


## Integrantes
- **Luan Orlandelli (RM: 554747)**
- **Jorge Luiz (RM: 554418)**

## Link para o simulador:
https://wokwi.com/projects/399787878606656513

## Link para o vídeo:
https://drive.google.com/file/d/1jCGzBoW3VRwSgQ6p1IS8u1VB-QEdPyaR/view?usp=sharing

## Descrição 
Este projeto utiliza um sensor de luz submersível para medir a intensidade da luz a diferentes profundidades. Os dados são exibidos em um display LCD e dois LEDs indicam visualmente se a intensidade da luz está adequada, muito clara ou muito escura. Esse tipo de monitoramento pode ser crucial para o estudo do crescimento de plantas marinhas e corais.

## Requisitos
- **Hardware**: Arduino (Uno, Nano, etc.), sensor de luz submersível, display LCD com I2C, LEDs, resistores, protoboard, fios jumper, fonte de alimentação, caixa à prova d'água.
- **Software**: Arduino IDE, bibliotecas `Wire` e `LiquidCrystal_I2C`.

## Componentes
Os componentes necessários para este projeto são:
* Arduino (Uno, Nano, etc.)
* Sensor de Luz Submersível (LDR ou Fotodiodo à prova d'água)
* Display LCD (16x2 com I2C)
* LED Verde
* LED Vermelho
* Resistores (220Ω para os LEDs)
* Protoboard e Fios Jumper

## Como Montar
1. **LDR (Light Dependent Resistor)**:
    - Conecte um terminal do LDR ao pino A0 do Arduino.
    - Conecte o outro terminal do LDR ao VCC (5V).
    - Conecte um resistor de 10kΩ entre o pino A0 e o GND.

2. **Conexão do Display LCD com I2C**
    - Conecte o pino VCC do módulo I2C ao pino 5V do Arduino.
    - Conecte o pino GND do módulo I2C ao pino GND do Arduino.
    - Conecte o pino SDA do módulo I2C ao pino A4 do Arduino.
    - Conecte o pino SCL do módulo I2C ao pino A5 do Arduino.

3. **Conexão dos LEDs**
    - Conecte o anodo (perna mais longa) do LED verde ao pino D2 do Arduino através de um resistor de 220Ω.
    - Conecte o catodo (perna mais curta) do LED verde ao GND.
    - Conecte o anodo do LED vermelho ao pino D3 do Arduino através de um resistor de 220Ω.
    - Conecte o catodo do LED vermelho ao GND.

## Imagem do projeto
![Imagem README Edge GS](https://github.com/LuanOrlandelli/global-solution-edge/assets/161336507/5cce7866-9ce3-4231-a255-d5b2d2ab64b8)


## Considerações Finais

- **Calibração**: Os valores `200` e `800` usados no código são exemplos. Ajuste esses valores conforme necessário para seu ambiente específico.
- **Proteção à Prova d'Água**: Verifique as especificações do sensor de luz submersível para garantir que ele seja adequadamente protegido contra a água.
