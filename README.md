# ESP-SimHub Custom Protocol - Dashboard

![ESP-SimHub Logo](https://www.simhubdash.com/wp-content/uploads/2017/09/gamehub-icon-small-text-1.png)

![screen-shot](https://github.com/Gambya/neo-racing-esp-simhub-dashboard/blob/main/assets/diplay_example01.jpg)

## Connection Diagram
![connection diagram](https://github.com/Gambya/neo-racing-esp-simhub-dashboard/blob/main/assets/esp32_display.png)

A placa ESP32-2432S028 já vem com o esp32 embitido na pcb, conforme imagem acima. Existem portas io disponíveis para extender o projeto além da dashboard.

## Table of Contents

- [Introdução](#introdução)
- [Prerequisitos](#prerequisitos)
- [Getting Started](#getting-started)
    - [Instalação](#instalação)
- [Contribuindo](#contribuindo)
- [License](#license)

## Introdução

Este projeto extende a funcionalidade do [ESP-SimHub](https://github.com/eCrowneEng/ESP-SimHub) adicionando um protocolo personalizado para permitir a comunicação com ESP8266/ESP32 e SimHub para renderizar uma dashboard de corrida simples. Neste projeto estamos parametrizando os arquivos para utilizarem a placa ESP32-2432S028 que ja vem com o display.

## Prerequisitos

Antes de usar este projeto, certifique-se de ter os seguintes pré requisitos:

- [Visual studio code](https://code.visualstudio.com/download)
- [PlatformIO extension](https://platformio.org/install/ide?install=vscode)
- [ESP-SimHub](https://github.com/eCrowneEng/ESP-SimHub): Você precisa ter instalado e configurado o ESP-SimHub em sua máquina.
- [LovyanGFX Library](https://github.com/lovyan03/LovyanGFX)

## Getting Started

Siga estas etapas para instalar e usar o painel de protocolo personalizado ESP-SimHub.

### Instalação

1. Download da pasta zipada deste repository:

   [Download ziped folder](https://github.com/Gambya/neo-racing-esp-simhub-dashboard/archive/refs/heads/main.zip)

2. Extraia a pasta zip e substitua o arquivo "SHCustomProtocol.h" no projeto ESP-Simhub pelo que você obteve neste repositório:

3. Instale a dependência necessária [LovyanGFX Library](https://github.com/lovyan03/LovyanGFX).

4. Após instalação da dependência em seu projeto pelo platformio, substitua o arquivo "LGFX_ESP32_sample.hpp" deste repositório no lugar do mesmo arquivo no caminho a ".pio/libdeps/esp32/LovyanGFX/src/lgfx_user/LGFX_ESP32_sample.hpp". O arquivo "LGFX_ESP32_sample.hpp" deste repositório contem todo o mapeamento dos pinos da placa ESP32-2432S028 para que o display funcione corretamente.

5. Edite o protocolo personalizado do Simhub com o conteudo do arquivo "customProtocol-dashBoard.txt" que se encontra neste repositório.

### Vídeo Tutorial:



## Contribuindo

Agradecemos contribuições da comunidade para melhorar a funcionalidade deste projeto. Se você tiver ideias, relatórios de bugs ou melhorias, abra um problema ou envie uma solicitação pull.

---

Boa simulação e desenvolvimento com ESP-SimHub e sua extensão de protocolo personalizada! Se você tiver alguma dúvida ou precisar de ajuda, sinta-se à vontade para entrar em contato com os mantenedores do projeto ou com a comunidade ESP-SimHub.

---

Este projeto usou como base o projeto [Sim Esp Dashboard](https://github.com/MoemenMostafa/simhub-esp-dashboard)
