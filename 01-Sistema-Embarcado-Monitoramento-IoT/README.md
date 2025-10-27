# 🤖 01-Sistema-Embarcado-Monitoramento-IoT

## 🚨 Projeto Integrador I: Sensor de Presença com ESP32-CAM e Alerta Telegram

### 💡 Visão Geral do Projeto

Este projeto consiste no desenvolvimento de um sistema de segurança residencial de baixo custo utilizando o microcontrolador **ESP32-CAM** para monitorar a presença de pessoas em um ambiente e enviar alertas instantâneos via **API do Telegram**.

O objetivo principal foi aplicar os fundamentos de **Sistemas Embarcados**, programação de hardware e comunicação de rede (Wi-Fi) para criar uma solução prática e funcional de Internet das Coisas (IoT).

### 🎯 Resultados e Valor Entregue

* **Comunicação Ciberfísica:** Demonstração da capacidade de interligar um componente físico (Sensor PIR) com um serviço digital (Telegram API).
* **Alerta em Tempo Real:** Criação de um sistema de notificação imediata, essencial para aplicações de segurança e monitoramento.
* **Programação de Baixo Nível:** Domínio da sintaxe C/C++ (Arduino IDE) para controle direto de hardware, fundamental em projetos de IoT.

### 🛠️ Tecnologias Utilizadas

| Categoria | Tecnologia | Uso no Projeto |
| :---: | :--- | :--- |
| **Microcontrolador** | **ESP32-CAM** | Execução do código, gestão da conexão Wi-Fi, Responsável pela fotografia. |
| **Linguagem Base** | **C/C++** | Lógica de leitura do sensor e controle do hardware (via Arduino IDE). |
| **Sensor** | **Sensor PIR (Infravermelho Passivo)** | Detecção de movimento e presença no ambiente. |
| **Comunicação** | **Telegram Bot API** | Serviço de nuvem utilizado para envio das notificações (mensagens) em tempo real. |

### ⚙️ Arquitetura e Diagrama de Conexão

O sistema opera em um ciclo contínuo: o ESP32 lê o estado do Sensor PIR. Se o estado muda de "sem movimento" para "movimento detectado" (nível lógico alto), o ESP32 utiliza sua conexão Wi-Fi para acionar o bot do Telegram e enviar a mensagem de alerta.

[**IMAGEM:** Inclua aqui uma foto ou diagrama mostrando como o Sensor PIR foi conectado ao ESP32.]

### 💻 Guia de Instalação e Execução

Para replicar e testar este projeto, siga os passos abaixo:

1.  **Instale a Arduino IDE:** Certifique-se de que a IDE está instalada e configurada para a placa ESP32.
2.  **Configure o Telegram Bot:**
    * Crie um novo bot no Telegram usando o **BotFather** e obtenha o **`TOKEN`** do bot.
    * Inicie uma conversa com seu bot e obtenha o seu **`CHAT_ID`** (você pode usar um bot de terceiros para descobrir seu ID).
3.  **Atualize as Credenciais:** No código-fonte do ESP32 (`.ino`), substitua os seguintes placeholders:
    ```c++
    const char* ssid = "SEU_NOME_DA_REDE_WIFI";
    const char* password = "SUA_SENHA_DO_WIFI";
    #define BOT_TOKEN "SEU_TOKEN_DO_TELEGRAM";
    long CHAT_ID = SEU_CHAT_ID;
    ```
4.  **Conexão de Hardware:** Conecte o Sensor PIR ao ESP32:
    * VCC do PIR ao 3.3V do ESP32.
    * GND do PIR ao GND do ESP32.
    * OUT (Data) do PIR a um pino digital do ESP32 (ex: D2).
5.  **Compilar e Carregar:** Faça o upload do código para o ESP32.

---

[⬅️ Voltar ao README Principal](../../README.md)
