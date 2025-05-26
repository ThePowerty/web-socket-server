# Aplicación de Chat en Tiempo Real con Spring Boot y WebSocket

Esta es una aplicación de chat en tiempo real desarrollada con **Spring Boot** que utiliza **WebSocket** para habilitar la comunicación bidireccional entre clientes y servidor. El proyecto incluye un frontend básico integrado dentro de la estructura del proyecto con una página HTML sencilla para la interacción con el chat.

---

## Características

- Comunicación en tiempo real mediante WebSocket.
- Frontend básico integrado usando HTML y JavaScript.
- Soporta múltiples usuarios conectados simultáneamente.
- Mensajes instantáneos que se reflejan sin necesidad de recargar la página.

---

## Tecnologías utilizadas

- Java 24+
- Spring Boot
- Spring WebSocket
- HTML, CSS y JavaScript para el frontend integrado

---

## Estructura del proyecto

```plaintext
├── src
│   ├── main
│   │   ├── java
│   │   │   └── dev.williams.web_socket_server
│   │   │       ├── chat
│   │   │       │    ├── ChatController.java
│   │   │       │    ├── ChatMessage.java
│   │   │       │    └── MessageType.java
│   │   │       ├── config
│   │   │       │    ├── WebSocketConfig.java
│   │   │       │    └── WebSocketEventListener.java
│   │   │       └── ChatApplication.java
│   │   └── resources
│   │       ├── static
│   │       │   ├── css
│   │       │   │    └── main.css
│   │       │   ├── js
│   │       │   │    └── main.js
│   │       │   └── index.html                  # Frontend del chat
│   │       └── application.properties
```

---
# Cómo correr la aplicación

## Requisitos previos

- JDK 24
- Maven

## Pasos para ejecutar

1. Clonar el repositorio

    ```bash
    git clone &lt;url-del-repositorio&gt;
    cd &lt;nombre-del-proyecto&gt;
    ```

2. Ejecutar la aplicación
3. Abir el navegador y acceder a:

   http://localhost:8080

   Verás la página de chat donde podrás escribir mensajes y enviarlos en tiempo real.
---
## Detalles Técnicos
* La configuración de WebSocket se define en WebSocketConfig.java.
* El backend gestiona los mensajes entrantes y los retransmite a todos los clientes conectados.
* El frontend index.html se encuentra en la carpeta src/main/resources/static y utiliza JavaScript para abrir y manejar la conexión WebSocket.
* No requiere base de datos ni autenticación para funcionar, es un ejemplo básico y funcional.

---
# Contacto

Para dudas o sugerencias, puedes contactarme o abrir un issue en el repositorio