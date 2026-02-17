# 🤖 Agente Virtual Web

Proyecto de desarrollo del **Chatbot Web** basado en **OpenAI AgentKit**, integrado con el ecosistema **Odoo 17** de Cement Design.

Este agente virtual será capaz de asistir a usuarios del sitio web (clientes, distribuidores o visitantes) mediante una interfaz conversacional, resolviendo consultas y conectando con módulos internos de Odoo.

---

## 🧩 Objetivo del proyecto

Desarrollar un **agente virtual web inteligente**, integrado al entorno digital centralizado de Cement Design, capaz de:

- Responder preguntas frecuentes (catálogo, productos, servicios).
- Escalar solicitudes o casos al CRM de Odoo.
- Asistir en procesos comerciales y de soporte básico.
- Extender sus capacidades mediante módulos adicionales (VoIP, citas, marketing, etc.).

---

## ⚙️ Estructura del proyecto

```plaintext
  chatbot/              → Lógica central del agente
  ├── agent.py        → Script principal
  ├── config.py       → Configuración global
  ├── prompts.py      → Mensajes e instrucciones del agente
  └── utils.py        → Funciones auxiliares
```
`odoo_connector/`        → Módulo de integración con Odoo
`web_interface/`         → API o interfaz web para incrustar el chatbot
`tests/`                 → Scripts de prueba
`docs/`                  → Documentación técnica y funcional


## 🧭 Flujo de desarrollo

***Fase 0 – Preparación:***
Entorno Python, configuración de API y estructura del repositorio.

***Fase 1 – Chatbot local:***
Creación del agente virtual básico y su interacción por consola.

***Fase 2 – Interfaz web:***
Integración del chatbot en la web institucional.

***Fase 3 – Conexión Odoo:***
Comunicación bidireccional con Odoo (ventas, CRM, soporte, etc.).

## 🧰 Requisitos técnicos

* Python ≥ 3.10
* OpenAI SDK (openai)
* python-dotenv
* Acceso API a OpenAI (clave en .env)
* Odoo 17 (para fases futuras)

## 🚀 Configuración inicial

1. Clonar el repositorio:
   ```bash
     git clone https://github.com/tuusuario/agentkit-chatbot.git
     cd agentkit-chatbot
   ```
2. Crear entorno virtual
   ```bash
   python -m venv venv
   venv\Scripts\activate # En Windows
   ```
3. Instalar dependencias
   ```bash
   pip install -r requirements.txt
   ```
4. Crear archivo `.env` con tu clave de OpenAI
   ```bash
   OPENAI_API_KEY=TU-CLAVE-AQUI
   ```
5. Probar conexion
   ```bash
   python test_openai.py
   ```
## 🧱 Convenciones del proyecto

* Documentacion: todo cambio debe de reflejarse en `/docs/`
* Commits: Mensajes cortos y claros, si requieres una descripcion mas larga, puedes agregarlo en la parte #2 del commit, ejemplo:
  `git commit -m "[ddmmaaaa##] feat(agent): New base tree for the whole project" -m "A completely new folder structure has been added to the project to refactor existing components."`

## 🧾 Licencia
Este proyecto esta bajo la Licencia "GNU GENERAL PUBLIC LICENSE Version 3", consulta el archivo `LICENSE` para mas detalles

## © Cement Design
Desarrollado por [Camiicode](https://github.com/camiicode) – Frontend Developer & Odoo Implementer
