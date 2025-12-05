# Claude Local - Varios modelos

Interfaz web local para usar modelos de IA vía Puter, inspirada en la UI oficial de Claude.  
Funciona en tu navegador y se ejecuta con un servidor local muy sencillo (sin backend propio).

Este repositorio es una versión mejorada del repositorio original de: 
👉 [hassanmsthf11/unlimited-claude-AI](https://github.com/hassanmsthf11/unlimited-claude-AI).  

---

## Cambios y mejoras en esta versión:

- 🗣️ **Interfaz traducida al español**  
  Textos de botones, mensajes de ayuda y avisos adaptados.

- 💾 **Historial de chats persistente**  
  - Los chats se guardan automáticamente en `localStorage`.  
  - Se mantienen entre sesiones mientras no se borren.

- 🗑️ **Gestión de chats mejorada**  
  - Botón para borrar todos los chats.  
  - Borrado manual de conversaciones individuales desde la lista de “Chats”.

- 🔐 **Manejo de autenticación con Puter ajustado**  
  - Mensajes de error más claros cuando Puter no responde o hay problemas de uso.  
  - Flujo de autenticación manual ligeramente mejor explicado.

- 🎨 **Personalización visual**   
  - Colores y pequeños detalles visuales adaptados.

La lógica principal de conexión con Puter.js y el uso de modelos de IA sigue el diseño del proyecto original.

---

## Requisitos:

- 🐍 **Python 3**  
  Solo se usa para levantar el servidor local con `http.server`.  
  No necesitas instalar paquetes extra.

- 🌐 **Navegador moderno**  
  Chrome, Edge, Firefox, etc.

---

## Cómo ejecutar en local:

### Windows

1. Descarga este repositorio como ZIP y descomprímelo.
2. Entra en la carpeta del proyecto.
3. Dentro de `unlimited claude`, haz doble clic en `run_server.bat`.
4. Se abrirá una ventana de consola y tu navegador irá a una URL tipo:  
   `http://localhost:8010/Claude.html` (o el puerto que especifique el script).

### Mac / Linux / otros

1. Descarga y descomprime el ZIP.
2. Abre una terminal y navega a la carpeta `unlimited claude`.
3. Ejecuta:

   ```bash
   python -m http.server 8000
