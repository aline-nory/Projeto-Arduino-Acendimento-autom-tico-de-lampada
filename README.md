# Iluminação inteligente: proteja você e aqueles que ama

Este repositório é um projeto desenvolvido para a disciplina de Objetos inteligentes conectados da Universidade Presbiteriana Mackenzie, {TURMA 05A} 2021/2, e tem como objetivo apresentar a automação de um acionamento automático de lâmpada utilizando arduino, sensor, atuador, comunicação/controle via internet (tcp/ip) e o monitoramento via MQTT.  

## Descrição do funcionamento

A porta analógica do Arduino irá ler as informações recebidas pelo sensor LDR e dependendo da leitura o acionamento de uma porta de saída digital é ligada ou desligada, acionando o módulo relé que fechará o contato da alimentação da lâmpada (atuador). Os dados vão retornar via protocolo MQTT se o estado da lâmpada é true (ligada) ou false (desligada).

## Hardwares e softwares utilizados

- Microcontrolador arduino: Este é o equipamento que fica armazenado o código criado pelo usuário (transmitido via porta usb) e que controla as os pinos de entrada/saída, conforme a sua programação e os processa para o controle de acendimento automático das lâmpadas. Modelo utilizado: Uno R3 ATmega328.

- Protoboard: Dispositivo projetado para permitir a criação de circuitos sem a necessidade de solda. Modelo utilizado: protoboard 400 pontos.

- Sensores de luz LDR: são utilizados para indicar a presença ou ausência de luz através de um foto-resistor, o qual mede a intensidade luminosa do ambiente através da variação de sua resistência interna.

- Resistores: são dispositivos que oferecem resistência à passagem de eletricidade, ou seja, limitam a intensidade de corrente elétrica. Modelos utilizados: resistores ôhmicos, 220 ohms e 10k ohm.

- Módulo relé: é um dispositivo capaz de acionar um interruptor a partir de um sinal, sendo utilizado para acionar cargas que empregam correntes maiores do que a fornecida pelo Arduino. Modelo utilizado: módulo de 2 canais 5V - 10ª.

- Node-red: é uma ferramenta de desenvolvimento visual, criada originalmente pela IBM para conectar dispositivos de hardware, APIs e serviços online como parte da Internet das Coisas (IoT). É um editor de fluxo, construído em Node.js, que pode ser usado para criar funções em JavaScript e armazenados usando JSON. Versão utilizada: 2.0 e o pacote serialport.

- Arduino IDE: é um editor de texto para escrever e compilar código, uma área de mensagem, um console de texto e uma série de menus junto com uma barra de ferramentas para criação, sendo utilizada para fazer a integração entre o Arduíno e a ferramenta Node-RED através do protocolo Firmata. 

- Protocolo MQTT via broker: é um protocolo de mensagens de publicação/assinatura que possui características simples, abertas e leves. O protocolo MQTT é executado usando TCP/IP, portanto, este protocolo requer transporte para executar comandos MQTT, fluxos de bytes de cliente/servidor ou servidor/cliente. O broker é o elemento responsável por gerir as publicações e as subscrições do protocolo MQTT.

- MQTTBox: Programa auxiliar de desenvolvedores para criar e testar o protocolo de conectividade MQTT. 

## Instalação

É necessário ter o Node instalado e executar o código abaixo em um terminal para instalar o NodeRed:

Node-red


