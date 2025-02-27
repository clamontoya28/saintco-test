# IoT Smart Sensor con ESP8266 e MicroPython

Un progetto IoT che utilizza ESP8266 per raccogliere dati da sensori e inviarli al cloud.

![Smart Sensor](docs/saintco_primologo.png)

## ✨ Funzionalità

- 📡 **Connessione Wi-Fi:** Il dispositivo si connette alla rete per inviare dati.
- 📊 **Monitoraggio Sensori:** Rileva temperatura e umidità con il sensore DHT11.
- ☁️ **Invio Dati al Cloud:** Salva le letture in un database remoto.
- 🔧 **Facile Configurazione:** Semplice da installare e configurare.

## 🔧 Requisiti

### 📟 Hardware
- ESP8266 (NodeMCU o Wemos D1 Mini)
- Sensore DHT11/DHT22
- Breadboard e cavi jumper

### 💻 Software
- MicroPython (firmware per ESP8266)
- Thonny IDE o uPyCraft per scrivere codice
- Wi-Fi per la connessione

## 🚀 Installazione e Configurazione

1️⃣ **Flashare MicroPython su ESP8266**  
Scarica il firmware da [MicroPython.org](https://micropython.org/download/) e installalo con `esptool.py`:

```bash
esptool.py --port /dev/ttyUSB0 erase_flash
esptool.py --port /dev/ttyUSB0 --baud 460800 write_flash --flash_size=detect 0 firmware.bin
