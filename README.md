# Claude IA Local Ilimitado en Español

Interfaz web local para usar modelos de IA vía Puter, inspirada en la UI oficial de Claude.  
Funciona en tu navegador y se ejecuta con un servidor local muy sencillo (sin backend propio).

Este repositorio es una versión mejorada del repositorio original
👉 [hassanmsthf11/unlimited-claude-AI](https://github.com/hassanmsthf11/unlimited-claude-AI).  

---

## Cambios y mejoras en esta versión

En comparación con el repositorio original, esta variante se centra en:

- 🗣️ **Uso cómodo en español:**  
  Toda la interfaz (botones, avisos y textos guía) está traducida y adaptada al castellano, pensada para uso real.

- 💾 **Historial de chats persistente:**  
  - Las conversaciones se guardan automáticamente en `localStorage`.  
  - Puedes cerrar el navegador o apagar el PC sin perder el chat, mientras no los borres manualmente.

- 🗑️ **Control del historial:**  
  - Botón dedicado para borrar **todos** los chats cuando quieras “empezar de cero”.  

- 🔐 **Autenticación con Puter más clara:**  
  - Mensajes de error más entendibles cuando Puter no responde o limita el uso.  
  - Explicación más directa del flujo de autenticación manual para evitar confusiones.

- ⚙️ **Llamadas a la IA ajustadas para más estabilidad:**  
  - Uso de respuestas completas (sin `stream: true`) para reducir cuelgues tras varios mensajes.  
  - Envío solo de las últimas interacciones al modelo para no sobrecargar el contexto.

- 🎨 **Personalización visual:**  
  - Textos, colores y pequeños detalles visuales adaptados.

La lógica principal de conexión con Puter.js y el uso de modelos de IA sigue el diseño del proyecto original.

---

## Requisitos

- 🐍 **Python 3:**  
  Solo se usa para levantar el servidor local con `http.server`.  
  No necesitas instalar paquetes extra.

- 🌐 **Navegador moderno:**  
  Chrome, Edge, Firefox, etc.

---

## Cómo ejecutar en local

### Windows:

1. Descarga este repositorio como ZIP y descomprímelo.
2. Entra en la carpeta del proyecto.
3. Dentro de `unlimited claude`, haz doble clic en `run_server.bat`.
4. Se abrirá una ventana de consola y tu navegador irá a una URL tipo:  
   `http://localhost:8010/Claude.html` (o el puerto que especifique el script).

### Mac / Linux / otros:

1. Descarga y descomprime el ZIP.
2. Abre una terminal y navega a la carpeta `unlimited claude`.
3. Ejecuta:

   ```bash
   python -m http.server 8010

---

## Autor

Esta versión está mantenida por:

- 🌐 Web: [https://dupavi.es](https://dupavi.es)  
- 💼 LinkedIn: [Eduard Pampalona Viladot](https://www.linkedin.com/in/eeduuu-seo-ia/)

<p align="left">
  <a href="https://dupavi.es" target="_blank"><img src="https://img.shields.io/badge/DUPAVI.ES-f97316?style=for-the-badge&logo=google-chrome&logoColor=white" alt="Web dupavi.es" /></a> &nbsp; <a href="https://www.linkedin.com/in/eeduuu-seo-ia/" target="_blank"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn - Eduard Pampalona Viladot" /></a>
</p>

---

## Licencia

Este proyecto mantiene la misma licencia que el repositorio original: **MIT**.  
Consulta el archivo `LICENSE` para ver el texto completo de la licencia.
