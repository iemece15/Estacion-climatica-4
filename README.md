## Requisitos

- Tener funcionando NodeRed

## Instrucciones

- Crear un nuevo flow
- Agregar un nodo mqtt
- Agregar un nuevo broker y agregar únicamente la url
- localhost (mosquitto)
- Tema: codigoIoT/mqtt/clima
- Output: a String
- Agregar un nodo JSON. Siempre convertir a JavaScript Object
- Agregar dos nodos function

---
Nodo function temperatura

msg.payload = msg.payload.temp; msg.topic = "Temperatura"; return msg;

Nodo function humedad

msg.payload = msg.payload.hum; msg.topic = "Humedad"; return msg;
---

- Crear una pestaña y dos grupos de informacion

---
    Pestaña: Clima local
    Grupo1: Indicadores
    Grupo2: Gráclksfica
---

- Agregar 2 nodos gauge y configurarlos

- Asociarlos al grupo indicadores
- Determine etiquetas y rangos

- Agregar el nodo chart

- Asociarlos al grupo indicadores

