## MQTT / TTN / Python Project

<p align="justify">
    Projeto de integração de dispositivos IoT com a plataforma The Things Network (TTN) e o protocolo MQTT, utilizando a linguagem de programação Python.
</p>

<p align="justify">
    O projeto consiste em um dispositivo IoT (LHT65N) que envia dados para a plataforma TTN, que por sua vez, envia os dados para um servidor MQTT. O servidor MQTT é responsável por receber os dados e armazená-los em um arquivo de log/texto qualquer.
</p>

<p align="justify">
    Desenvolvido para fins de estudo e aprendizado, e tem como objetivo principal a integração de dispositivos IoT com a plataforma TTN e o protocolo MQTT. Além disso, utiliza a biblioteca Paho MQTT do Python para a devida comunicação.
</p>

## Tecnologias utilizadas:
- Python
- LoRa e LoRaWAN
- The Things Network (TTN)
- MQTT (Mosquitto)

## Pré-requisitos
- Python 3.x
- Paho MQTT instalado na máquina
- Conta na plataforma The Things Network (TTN)
- Dispositivo IoT (LHT65N) ou "Uplink" simulado na TTN
- API Key na plataforma TTN para o servidor MQTT - Cadastro em "Integrations" e "MQTT"
- Servidor MQTT instalado localmente (Mosquitto, HiveMQ, etc)
- Conhecimentos básicos em Python, MQTT, LoRa, LoRaWAN, TTN

## Como utilizar o modo de recebimento de dados
1. Clone o repositório
2. Garanta que o dispositivo IoT esteja enviando dados para a plataforma TTN
3. Altere as variáveis (`USER`, `PASSWORD`, `PUBLIC_TLS_ADDRESS`, `PUBLIC_TLS_ADDRESS_PORT`, `DEVICE_ID`) no arquivo "receive_uplink_messages.py" conforme as informações da sua conta na TTN
3. Execute o arquivo "receive_uplink_messages.py" para receber os dados
4. Visualize os dados recebidos no arquivo de texto gerado

## Como utilizar o modo de envio de dados
1. Clone o repositório
2. Altere as variáveis (`USER`, `PASSWORD`, `PUBLIC_TLS_ADDRESS`, `PUBLIC_TLS_ADDRESS_PORT`, `DEVICE_ID`) no arquivo "send_downlink_messages.py" conforme as informações da sua conta na TTN
3. Execute o arquivo "send_downlink_messages.py" para enviar os dados
4. Visualize os dados enviados na aba "Live Data" da plataforma TTN

## Autor:
<a href="https://github.com/mateusferroantunesdeoliveira"><img src="https://avatars.githubusercontent.com/u/53230135?v=4" width="100px;" alt=""/><br /><sub><b>Mateus Ferro Antunes de Oliveira</b></sub></a>

Adaptado de: [Receive Uplink](https://www.mobilefish.com/download/lora/receive_uplink_messages.py.txt) e [Send Downlink](https://www.mobilefish.com/download/lora/send_downlink_messages.py.txt) do mobileFish

## 
Projeto desenvolvido e finalizado em 03/2024
