# 🌊 Sistema de Alerta de Enchentes com Arduino — Projeto IoT

Este é um projeto de Internet das Coisas (IoT) que simula um **sistema inteligente de alerta de enchentes**, utilizando sensores para monitorar o nível da água e a umidade do ar, com alertas visuais e sonoros. O sistema foi desenvolvido para rodar no simulador Wokwi, usando componentes 100% compatíveis.

---

## 🎯 Objetivo

Criar uma solução acessível para detectar riscos de enchentes, com base em:
- Monitoramento de nível da água
- Medição da umidade do ar (indicando chuva)
- Alertas automáticos em tempo real

---

## 🧰 Componentes Utilizados

- Arduino Uno  
- Sensor Ultrassônico HC-SR04 (nível da água)  
- Sensor DHT22 (umidade e temperatura)  
- Display LCD 16x2 com módulo I2C  
- LEDs (verde, amarelo, vermelho)  
- Buzzer (alarme sonoro)  
- Protoboard e jumpers

---

## ⚙️ Funcionamento

1. **Sensor HC-SR04** mede a distância até a superfície da água.
2. **DHT22** monitora a umidade do ar (simula presença de chuva).
3. O **LCD 16x2** exibe os dados em tempo real.
4. LEDs indicam o nível de risco:
   - 🟢 Verde: seguro
   - 🟡 Amarelo: atenção
   - 🔴 Vermelho: alerta
5. O **buzzer** é ativado em situação de risco elevado.

Gif do projeto funcionando no wokwi:
![GSegdeAlertaEnchente](https://github.com/user-attachments/assets/2013e4e2-903d-4d3f-9d22-28fcb9142c48)

---

## 💡 Lógica de Alerta

| Nível de Água (cm) | Umidade (%) | Alerta |
|--------------------|-------------|--------|
| < 60               | > 85        | Crítico (LED vermelho + buzzer) |
| < 120              | > 70        | Atenção (LED amarelo) |
| >= 20              | <= 70       | Seguro (LED verde) |

---

## 🧪 Simulação no Wokwi

💻 O projeto é totalmente funcional no simulador online.  
📎 [Link para o projeto no Wokwi](https://wokwi.com/projects/432572281111019521)

---

## 🎥 Video Demonstrativo

💻 Video demonstrativo publicado no youtube.  
📎 [Video Demonstrativo](https://youtu.be/lWTvgWU_bWE)

---

## 👨‍💻 Integrantes

- **Lucas Cavalcante RM 562857**  
- **Matheus Rodrigues RM 561689**

---
