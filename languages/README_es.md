# vkt-shortcut — Gestor de atajos de teclado

[English](../README.md) | [中文](README_zh.md) | Español | [Deutsch](README_de.md) | [日本語](README_ja.md) | [Français](README_fr.md)

Una extensión ligera para el navegador que bloquea y reasigna atajos de teclado. Detén las teclas no deseadas, redirige combinaciones a acciones personalizadas y toma el control total de tu teclado.

> Basada en Chromium · Manifest V3 · Sin rastreo · Procesamiento completamente local

---

## ¿Por qué vkt-shortcut?

La mayoría de bloqueadores de atajos solo bloquean teclas — no pueden reasignarlas. vkt-shortcut es diferente: **bloquea gratis, reasigna con Premium**, con un conjunto de reglas que se aplica en todas partes por defecto — más el alcance por sitio cuando lo necesitas.

| Ventaja | Detalle |
|---------|--------|
| 🚫 **Bloquear teclas** | Intercepta y desactiva atajos de teclado dentro de la página, en cualquier sitio |
| 🔁 **Reasignar teclas** | Redirige una combinación de teclas a otra dentro de la página — poco común en herramientas similares (Premium) |
| 🌐 **Reglas globales + por sitio** | Las reglas se aplican en todos los sitios web por defecto; opcionalmente limita una regla a un sitio (subdominios incluidos) |
| ⌨️ **Grabación de teclas** | Pulsa la combinación directamente — se captura automáticamente |
| ⚡ **Preajustes por sitio** | Reglas de bloqueo con un clic para conflictos conocidos en sitios populares — YouTube (K/J/L/M/F/C/I/T), X (N/L/R/T/B/M, /), Reddit (votos A/Z, J/K/C/S), Facebook (J/K/L/C/S, /), GitHub (S/T/W/B/X), el Ctrl+J de Doubao, el Ctrl+P/J de Notion, el Ctrl+P/J de VS Code Web. Todos los sitios compatibles aparecen en el panel, sin tener que visitarlos antes. Cada tecla del preajuste crea una regla, y puedes editarla o borrarla por separado |
| 🔇 **Bloquear todos los atajos** | Un interruptor por sitio que neutraliza cada atajo de la página, más un interruptor global en la parte superior del panel para todos los sitios a la vez (escribir, las flechas, el portapapeles y recargar siguen funcionando; la pausa por sitio tiene prioridad) |
| 📤 **Importar / Exportar** | Respaldo y restauración de reglas como JSON (Premium) |

---

## Gratis vs Premium

| Plan | Funcionalidades |
|------|----------|
| **Gratis** | Bloquear atajos, grabación de teclas, interruptor global, ajustes, import/export, reglas ilimitadas |
| **⭐ Premium** | Reasignación de teclas, sincronización entre dispositivos (cuenta del navegador), soporte prioritario |

Bloquear, grabar, ajustes e import/export son gratis para siempre y sin límite de reglas. La **reasignación de teclas** y la **sincronización entre dispositivos** requieren una licencia VKT Premium.

- ⚙ Activarla: abre el panel lateral de vkt-shortcut → haz clic en el botón **⚙** → introduce tu clave de licencia.

> La activación de licencia es **opcional**. El nivel gratuito funciona completamente sin ella — sin cuenta, sin registro, sin clave de licencia.

---

## Vista previa

<p align="center">
  <img src="screenshot/promo.png" alt="Vista previa de vkt-shortcut" width="640">
</p>

---

## Navegadores compatibles

| Navegador | Estado |
|---------|--------|
| Google Chrome | ✅ Totalmente compatible |
| Microsoft Edge | ✅ Totalmente compatible |
| Otros navegadores basados en Chromium | ✅ Debería funcionar |

---

## Instalación

1. Visita la página de Chrome Web Store de vkt-shortcut
2. Haz clic en **Añadir a Chrome** y confirma
3. Haz clic en el icono ⌨️ de vkt-shortcut en tu barra de herramientas para abrir el panel lateral

---

## Uso

1. **Haz clic en el icono ⌨️** en la barra de herramientas de tu navegador para abrir el panel lateral
2. **Haz clic en "➕ Nueva regla"** para crear una regla de atajo
3. **Elige el tipo de regla** — Bloquear (desactivar tecla) o Reasignar (redirigir tecla A → tecla B)
4. **Establece la tecla de origen** — haz clic en el campo de entrada y pulsa la combinación que quieres interceptar
5. **Para reasignar: establece la tecla de destino** — haz clic en el campo de destino y pulsa la combinación a la que redirigir
6. **(Opcional) Limitar a un sitio web** — introduce un dominio como `youtube.com` (subdominios incluidos), o déjalo vacío para aplicar en todas partes
7. **Guarda la regla** — entra en vigor inmediatamente, sin necesidad de recargar la página
8. **Alterna reglas** — usa el interruptor global para pausar sin eliminar

---

## Casos de uso

- **Aplicaciones web** — Bloquea F1 para que no abra la ayuda en Google Docs, Office 365 o cualquier editor web
- **Juegos online** — Desactiva atajos definidos por la página que interfieran con el juego (nota: las teclas reservadas por el navegador como Ctrl+W o F11 nunca llegan a la página, por lo que la interceptación a nivel de página no puede bloquearlas; las extensiones que usan `chrome.commands` solo pueden neutralizar algunas vinculándolas a comandos vacíos)
- **Herramientas de desarrollo** — Reasigna atajos de DevTools para evitar conflictos con combinaciones del IDE
- **Accesibilidad** — Reasigna combinaciones complejas a teclas más simples para facilitar el acceso
- **Modo presentación** — Bloquea todos los atajos de la página excepto la navegación durante presentaciones

---

## Privacidad

- ✅ Las reglas nunca salen de tu navegador — el bloqueo/reasignación ocurre completamente localmente
- ✅ Sin analíticas, sin rastreo, sin cookies
- ✅ Las reglas se almacenan solo en `chrome.storage.local`
- ✅ Solo permisos `storage` + `sidePanel`
- ℹ️ Las únicas solicitudes de red son la activación/validación opcional de licencia, que envía tu clave de licencia, un identificador de instalación aleatorio y metadatos del navegador a nuestro servidor de licencias (`api.annmax1983.com`)

---

## Aviso de derechos de autor

Esta extensión intercepta eventos de teclado en páginas web a nivel de navegador para comodidad del usuario. Todo el contenido, la funcionalidad y la propiedad intelectual de los sitios web originales permanecen sin cambios. Bloquear o reasignar atajos no modifica el contenido de ningún sitio web — solo evita o redirige la entrada del teclado antes de que llegue a la página.

---

## Aviso sobre el código fuente

> ⚠️ **Este repositorio no publica código fuente.** Contiene únicamente documentación de uso, notas de lanzamiento y recursos de soporte. La extensión se distribuye exclusivamente a través de Chrome Web Store. No se proporcionan paquetes de instalación sin conexión ni código fuente para usuarios finales.

---

## Licencia

Copyright © 2026 vkt-shortcut. Todos los derechos reservados.

---

## ❤️ Apoyo

Si te resulta útil vkt-shortcut, ¡considera invitarme a un café!

**[👉 Haz clic aquí para apoyar](https://ko-fi.com/annmax?ref=vkt-shortcut)**
