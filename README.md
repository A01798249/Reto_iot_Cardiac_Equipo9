# Reto IoT: Cardiac
## Equipo 9
- Stephanie Herrera Cervantes
- Alan Farid Hernández Sanmartin
  
Descripcion general: Sistema IoT wearable basado en ESP32 para monitoreo biomédico en tiempo real mediante MQTT, InfluxDB y Grafana, con generación de alertas automáticas.

Objetivo: Desarrollar un dispositivo wearable basado en ESP32 capaz de monitorear automáticamente variables biomédicas en tiempo real, enviar los datos mediante MQTT, almacenarlos en una base de datos y visualizarlos remotamente, generando alertas cuando se detecten valores fuera de los rangos establecidos.

Componentes
Hardware
- ESP32 — Microcontrolador y conexión Wi-Fi.
- MAX30102 — Medición de SpO₂ y frecuencia cardiaca.
- DS18B20 — Medición de temperatura corporal.
- Sensor/variable de oxigenación corporal — Variable adicional enfocada en monitoreo deportivo y respiratorio.
- Batería y elementos necesarios para hacer el dispositivo portable.

Software y comunicación
- MQTT / Mosquitto — Comunicación entre el wearable y el servidor.
- InfluxDB 2 — Almacenamiento de datos biomédicos.
- Grafana — Visualización y monitoreo remoto.
- Telegram / Email — Sistema de alertas.

## Estructura
``` text
wearable-iot/
│
├── README.md
│
├── esp32/
│   ├── src/
│   ├── include/
│   └── config/
│
├── mqtt/
│   └── broker/
│
├── backend/
│   ├── database/
│   └── processing/
│
├── grafana/
│   └── dashboards/
│
├── alerts/
│   └── notifications/
│
├── docs/
│   └── architecture/
│
└── tests/
```
