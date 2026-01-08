# 📊 Sistema de Gestión de Cartera con Notificaciones por WhatsApp

## 🧾 Descripción

Este sistema de **gestión de cartera** permite administrar clientes, obligaciones (deudas), fechas de vencimiento y estados de pago. Cuando un cliente **no paga a tiempo**, el sistema envía automáticamente un **mensaje de recordatorio por WhatsApp** utilizando **APIs externas** (como WhatsApp Business API, Twilio o proveedores similares).

Está pensado para negocios pequeños y medianos que necesitan llevar control de pagos y hacer seguimiento automático a clientes morosos.

---

## 🚀 Funcionalidades principales

* 📁 Gestión de clientes (crear, editar, eliminar)
* 💰 Gestión de deudas / facturas
* 📅 Control de fechas de vencimiento
* ✅ Registro de pagos
* ⚠️ Detección automática de mora
* 📲 Envío automático de mensajes por WhatsApp
* 🕒 Programación de recordatorios
* 📊 Reportes de cartera (al día / vencida)

---

## 🧠 Flujo general del sistema

1. Se registra un cliente con su número de WhatsApp
2. Se crea una deuda con fecha de vencimiento
3. El sistema revisa diariamente las deudas
4. Si una deuda está vencida y no está pagada:

   * Se genera un mensaje automático
   * Se envía por WhatsApp usando una API

---

## 🛠️ Tecnologías sugeridas

### Backend

* Node.js / Express **o** Python (FastAPI / Django)
* Base de datos: MySQL / PostgreSQL / MongoDB

### Frontend (opcional)

* HTML, CSS, JavaScript
* React / Vue

### WhatsApp API

Puedes usar cualquiera de estas opciones:

* ✅ WhatsApp Business Cloud API (Meta)
* ✅ Twilio WhatsApp API
* ✅ 360dialog

---

## ✉️ Ejemplo de mensaje automático

> Hola *Juan*, te recordamos que tienes un pago pendiente por **$250.000 COP** con vencimiento el **10/01/2026**. Por favor comunícate para evitar recargos. Gracias.

---

## ⏰ Automatización

El sistema puede usar:

* Cron Jobs
* Tareas programadas del servidor

Para revisar pagos vencidos, por ejemplo, **una vez al día**.

---

## ⚠️ Consideraciones importantes

* El cliente debe aceptar recibir mensajes por WhatsApp
* WhatsApp Business API **no es gratuita**
* Cumplir normas de protección de datos (Habeas Data)

---

## 📌 Futuras mejoras

* Mensajes personalizados por nivel de mora
* Historial de notificaciones enviadas
* Panel de métricas
* Integración con pagos en línea (PSE, Nequi, Daviplata)

---

## 👨‍💻 Autor

Sistema desarrollado como proyecto de gestión de cartera con automatización de cobros vía WhatsApp.

---

📩 *Cualquier mejora o integración adicional puede adaptarse según la necesidad del negocio.*
