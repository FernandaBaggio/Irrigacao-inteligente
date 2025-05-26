# Sistema de Irrigação Inteligente com ESP32

Este projeto simula um sistema de irrigação automática utilizando um microcontrolador ESP32, sensor de umidade do solo (DHT22), relé, servo motor e LEDs, com simulação da comunicação via protocolo MQTT.

## Funcionalidade

- Leitura da umidade do solo (simulada via Wokwi)
- Abertura automática da válvula quando a umidade estiver abaixo de 40%
- Feedback visual com LEDs (vermelho = irrigando, verde = umidade ok)
- Simulação da conexão com Wi-Fi e envio de dados via MQTT (exibido no Serial Monitor)

## Componentes Utilizados

- ESP32 Dev Module
- Sensor DHT22
- Servo motor
- Módulo relé
- LED vermelho e LED verde
- Resistores de 220Ω
- Protoboard (simulada)

## Bibliotecas necessárias

- ESP32Servo
- DHT sensor library

Essas bibliotecas devem ser adicionadas no projeto Wokwi usando o painel lateral ou este link direto:
[https://wokwi.com/projects/new?libraries=ESP32Servo,DHT%20sensor%20library](https://wokwi.com/projects/new?libraries=ESP32Servo,DHT%20sensor%20library)

## Como executar no Wokwi

1. Acesse [https://wokwi.com](https://wokwi.com)
2. Crie um novo projeto com ESP32 e cole os arquivos:
   - `sketch.ino`
   - `diagram.json`
   - `libraries.txt`
3. Clique em **Start Simulation**
4. Acompanhe o Serial Monitor para ver o envio simulado via MQTT

## Arquivos neste repositório

- `sketch.ino` – código-fonte do projeto
- `diagram.json` – circuito de ligação dos componentes
- `libraries.txt` – bibliotecas usadas na simulação
- `README.md` – esta documentação

## Desenvolvido por

Fernanda Baggio – Projeto acadêmico de IoT para irrigação inteligente com MQTT  
Faculdade Presbiteriana Mackenzie – Curso de Análise e Desenvolvimento de Sistemas
