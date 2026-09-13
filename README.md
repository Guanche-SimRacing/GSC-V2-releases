<!--
BORRADOR -- para el futuro repositorio PÚBLICO de distribución
(todavía no creado). NO es el README.md interno del repo privado
(ese ya existe y es correcto tal cual, de cara a desarrollo).

Cosas marcadas [PENDIENTE] necesitan un dato o una decisión tuya
antes de publicarse. Revísalo entero antes de usarlo -- es un
borrador, no un texto legal ni definitivo.
-->

# GSC V2 — Guanche SimRacing Control

> **🧪 Versión Beta.** Esta primera versión pública incluye la
> versión **Free** completa. **Pro llegará próximamente** — todavía
> no hay fecha ni precio cerrados. Si algo falla, cuéntanoslo por
> Discord.

**Configura tu volante, botonera o pedales DIY sin escribir ni una
línea de código.**

GSC V2 es la aplicación de escritorio (Windows) de Guanche SimRacing
para crear tu propio periférico de simracing: eliges tu placa, añades
los componentes que tengas (botones, matriz de botones, encoder,
sensores, pedales...), y la app te genera el diagrama de cableado y
te carga el firmware directamente — sin tocar código, sin Arduino IDE,
sin saber programar.

## ¿Para quién es esto?

Para cualquiera que se esté montando su propio volante, botonera o
pedales de simracing con una placa Arduino (Pro Micro o Leonardo), y
quiera evitarse la parte de programar el firmware a mano.

## Qué hace

- Eliges tu placa (Pro Micro / Leonardo, o un producto Guanche ya
  identificado como tal).
- Añades los componentes de tu proyecto: botones, matriz de botones,
  encoder rotativo, sensores Hall, joystick, interruptor rotativo de
  12 posiciones, célula de carga (pedales)...
- La app te asigna los pines automáticamente (o los eliges tú a
  mano), te avisa si un pin no es compatible con lo que necesitas.
- Te genera un diagrama de cableado claro: qué cable va a qué pin.
- Compila y sube el firmware a tu placa directamente desde la app.
- Cuando conectas tu dispositivo terminado al PC, aparece con el
  nombre que tú le pusiste (o el nombre del producto Guanche, si es
  uno de nuestros kits) — nunca como "Arduino Leonardo" a secas.

## Free y Pro

| | Free | Pro |
|---|---|---|
| Matriz de Botones (hasta 4×4) | ✅ | ✅ |
| Rotary Encoder | ✅ | ✅ |
| Botón simple / Interruptor | ❌ | ✅ |
| Sensor Hall | ❌ | ✅ |
| Joystick (2 ejes) | ❌ | ✅ |
| Interruptor rotativo (12 posiciones) | ❌ | ✅ |
| Célula de carga (pedales) | ❌ | ✅ |
| Matriz mayor de 4×4 | ❌ | ✅ |

**Pro llegará próximamente** — precio y enlace de compra se añadirán
aquí en cuanto estén listos.

## Descarga

👉 **[Descarga la última versión (Releases)](../../releases/latest)**

## Instalación

1. Descarga el `.zip` de la última versión.
2. Descomprime la carpeta completa en cualquier sitio de tu PC (no
   muevas solo el `.exe`, necesita el resto de la carpeta).
3. Ejecuta `GSC V2.exe`.

**Aviso importante:** la primera vez que la abras, es muy probable
que Windows muestre un aviso de **"Windows protegió tu PC"**
(SmartScreen). Esto pasa porque la app todavía no tiene un
certificado de firma de código (es caro y no aporta nada a la
función de la app) — no significa que sea un virus. Pulsa **"Más
información"** → **"Ejecutar de todas formas"**.

## Requisitos

- Windows 10/11.
- Un cable USB para conectar tu placa (Pro Micro, Leonardo, o
  cualquier producto Guanche).
- Si usas un clon de Pro Micro (muy habituales, chinos, baratos),
  puede que Windows necesite instalar el driver CH340 la primera
  vez — [descárgalo de la página oficial de WCH](https://www.wch-ic.com/downloads/CH341SER_ZIP.html)
  (nunca de otra web).
- Conexión a internet la primera vez que uses "Cargar Firmware"
  (la app instala sola las herramientas de Arduino que necesita).
  Después de eso, todo funciona sin conexión.

## Activar Pro

**[PENDIENTE]** Instrucciones paso a paso una vez Lemon Squeezy esté
conectado: comprar → recibir la clave → pegarla en Ajustes → Activar.

## Soporte

- Discord: **[Únete aquí](https://discord.gg/MDgCRAzTWJ)** — es el
  canal principal para dudas, ayuda y avisar de fallos.
- También puedes abrir un [Issue](../../issues) en este repositorio
  si prefieres dejarlo por escrito de forma pública.

## Placas y productos compatibles

- Arduino Pro Micro / Leonardo (genérico).
- Guanche SimRacing Wheel, Guanche Pedals Pro, Guanche Button Box,
  Guanche Hand Brake.

## Preguntas frecuentes

**¿GSC V2 es de código abierto?**
No. GSC V2 es software propietario — ver [EULA.md](EULA.md).

**¿Necesito saber programar?**
No, para nada. La app hace todo el trabajo de generar y cargar el
firmware.

**¿Funciona sin internet?**
Sí, salvo la primera vez que uses "Cargar Firmware" (instala
herramientas de Arduino) y al activar/desactivar una licencia Pro.

---

© 2026 Guanche SimRacing. Todos los derechos reservados.
