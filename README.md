# Sistema de rastreamento e alerta de pessoas em zonas proibidas

Este projeto tem como objetivo o desenvolvimento de um sistema de rastreamento de pessoas com tecnologia UWB utilizando o módulo DWM1001C-Dev, conectado ao Raspberry Pi, para monitoramento de segurança em  ambientes críticos. O sistema emite alertas por vibração ao detectar a entrada de um trabalhador em uma zona proibida (Red Zone).

## 🔍 Objetivo

Desenvolver um sistema funcional capaz de:
- Rastrear em tempo real a posição de tags UWB (pessoas).
- Definir zonas proibidas no ambiente.
- Emitir alertas automáticos por vibração ao entrar em Red Zones.

## 🧩 Componentes do Projeto

- **Módulo UWB DWM1001C** (tags + âncoras)
- **Raspberry Pi** (gateway de rastreamento)
- **Motor vibratório** (para alerta)
- **MQTT Broker** (comunicação)
- **Script Python + Código C++** para controle e alertas

## 📁 Estrutura do Projeto

