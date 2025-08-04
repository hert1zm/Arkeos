<p align="center">
  <img src="https://i.imgur.com/BFbMfse.png" alt="Arkeos logo" width="100"/>
</p>

<h1 align="center">Arkeos</h1>
<p align="center">
  Automazione distribuita e controllo remoto. Esame finale del corso UF17 reti e bus di campo.<br>
  Raspberry Pi 5 • ESP32 • PLC • Node-RED
</p>

<p align="center">
  <img src="https://img.shields.io/badge/status-active-brightgreen?style=flat-square" />
  <img src="https://img.shields.io/badge/platform-RaspberryPi5-blue?style=flat-square" />
  <img src="https://img.shields.io/badge/open%20source-yes-lightgrey?style=flat-square" />
</p>

---

## ✨ Cos'è Arkeos

**Arkeos** è un progetto di automazione distribuita che integra Raspberry Pi 5, microcontrollori ESP32 e PLC industriali tramite un server **Node-RED** su Raspberry Pi5.

È progettato per essere **scalabile**, **reattivo** ed estremamente **user-friendly**, grazie all'interfaccia grafica accessibile da browser. L'obiettivo è creare un ponte tra hardware eterogeneo, semplificandone la comunicazione, la visualizzazione e il controllo.

---

## ⚙️ Architettura del Sistema

- **Raspberry Pi 5** come hub centrale
- **ESP32** per sensori e attuatori remoti via Wi-Fi
- **PLC** industriale per la logica di controllo
- **Node-RED** come orchestratore visuale, event-driven
- **Telegram Bot** per notifiche e comandi remoti

![Architettura](docs/architettura.png)

---

## 🧠 Funzionalità principali

- 🔌 Controllo remoto di dispositivi e attuatori
- 📊 Dashboard live in tempo reale
- 💬 Bot Telegram integrato per allarmi e comandi
- 🔁 Sincronizzazione tra ESP32 e PLC
- 💾 Logging e data storage

---

## 🧭 Naviga i flussi

Il cuore logico del progetto è costruito con **flussi Node-RED**, modulari e documentati.  
Trovi i file `.json` nella cartella `/flows`.

Esempi:
- `esp32_control.json`: flusso per acquisizione e comandi
- `plc_comm.json`: interfaccia con PLC
- `telegram_bot.json`: integrazione bot

---

## 📥 Installazione

> ⚠️ Requisiti: Node-RED, Python 3.x, ESP32 con firmware compatibile, Raspberry Pi OS

```bash
git clone https://github.com/tuo-username/arkeos.git
cd arkeos
bash install.sh  # installa dipendenze e avvia Node-RED
