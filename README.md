# Sistema de rastreamento e alerta de pessoas em zonas proibidas

Este projeto tem como objetivo o desenvolvimento de um sistema de rastreamento de pessoas com tecnologia UWB utilizando o módulo DWM1001C-Dev, conectado ao Raspberry Pi, para monitoramento de segurança em  ambientes críticos. O sistema emite alertas por vibração ao detectar a entrada de um trabalhador em uma zona proibida classificada como "Red Zone".

## 🔍 Objetivo

Desenvolver um sistema funcional capaz de:
- Rastrear em tempo real a posição de tags UWB (pessoas).
- Definir zonas proibidas no ambiente.
- Emitir alertas automáticos por vibração ao entrar em Red Zones.

## 🧩 Componentes do Projeto

- **Módulo UWB DWM1001C** (tags + âncoras)
- **Raspberry Pi** (gateway de rastreamento)
- **Motor de vibração** (para emissão de alerta)
- **MQTT Broker** (interface de comunicação com API de alertas)
- **Script Python + Código C++** para controle e alertas

## 📁 Estrutura do Projeto

```
uwb-monitoring/
├── docs/                  # Documentação escrita (PC1, relatórios, etc.)
│   ├── PC1_proposta.md
│   └── imagens/
│       └── diagrama_blocos.png
│
├── diagrams/              # Diagramas do sistema e fluxogramas de lógica
│   ├── diagrama_blocos
│   └── fluxograma_alertas
│
├── hardware/              # Desenhos técnicos, ligações elétricas, pinagem
│   ├── esquema_rasp_tag.png
│   └── anotacoes.txt
│
├── software/
│   ├── scripts/           # Scripts de leitura da posição e publicação MQTT
│   │   ├── read_position_uart
│   │   └── publish_alert_mqtt
│   ├── testes/            # Logs, testes de comunicação
│   │   └── test_uart_read
│   └── C/                 # Código em C/C++ a ser usado no PC3 e PC4
│       ├── main.c
│       └── utils/
│           └── position_check
│
├── .gitignore             # Arquivos/pastas a ignorar no Git
├── README.md              # Descrição geral do projeto
└── LICENSE                # Licença do projeto (opcional)
```
