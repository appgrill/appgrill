<div align="center">

# 🔥 Will's Grill — Control de Feria

### La caja de tu negocio, en tu tablet, sin internet y sin complicaciones.

![status](https://img.shields.io/badge/estado-en%20uso-brightgreen)
![platform](https://img.shields.io/badge/plataforma-tablet%20%2F%20navegador-orange)
![stack](https://img.shields.io/badge/hecho%20con-HTML%20%2B%20JS%20puro-black)
![offline](https://img.shields.io/badge/funciona-sin%20internet-blueviolet)

</div>

---

## 🧾 ¿Qué es esto?

**Control de Feria** es la app hecha a la medida para llevar las cuentas de **Will's Grill** en cada feria: ventas, gastos, propinas, pagos a los trabajadores y fotos de facturas — todo desde una tablet, todo en un solo archivo, sin depender de internet para trabajar.

No es una app de tienda ni necesita servidor: es una sola página web que vive en el navegador y guarda todo ahí mismo. Y cuando quieres respaldo extra, se conecta sola a Google Drive.

## ✨ Por qué es chévere

- 📴 **Funciona sin internet** — registra ventas y gastos en pleno parque, sin señal.
- 📷 **Cámara integrada** — toca "Tomar foto" y se abre la cámara directo, sin apps externas.
- 📅 **Calendario nativo** — los campos de fecha abren el selector de la tablet con un toque.
- 👥 **Trabajadores por nombre** — agrégalos una vez y repárteles las propinas automáticamente, en partes iguales.
- ☁️ **Respaldo automático a Google Drive** — conecta una sola vez y cada movimiento y cada foto se suben solos, organizados en carpetas (Mercado / Gasolina / Respaldos).
- 📊 **Exporta a Excel** cuando quieras — por mes, por rango de fechas, por una feria puntual, o todo — con los links de Drive de cada foto incluidos.
- 🎨 **Diseño propio** — nada de plantilla genérica, hecho a la medida de la marca.
- 📲 **Se instala como app** — "Agregar a pantalla de inicio" y queda con ícono propio, pantalla completa.

## 🚀 Cómo abrirla

1. Entra al link de este sitio desde Chrome en la tablet.
2. Toca el menú (⋮) → **"Agregar a pantalla de inicio"**.
3. Ábrela siempre desde ese ícono — ahí es donde quedan guardados tus datos.

> 📘 Guía completa, paso a paso y con capturas: **`Manual_Control_de_Feria.docx`** (instalación, uso diario, y cómo conectar Google Drive).

## 🗂️ Cómo se organiza una feria

```
Feria
 ├─ Ventas          → efectivo / tarjeta, con propina opcional
 ├─ Factura Mercado  → con foto de factura → sube sola a Drive
 ├─ Gasolina         → con foto de factura → sube sola a Drive
 ├─ Otro gasto       → hielo, gas, imprevistos, alquiler del stand...
 ├─ Pago a trabajador → elige el nombre, queda como sueldo
 └─ Consignación     → lo que se entrega al encargado
```

Cada feria calcula solita: **Ventas**, **Gastos**, **Utilidad**, **Caja esperada en efectivo**, y el reparto de **Propinas** por trabajador.

## ☁️ Google Drive (opcional)

Una sola vez, el dueño conecta una cuenta de Google desde la tablet. Desde ahí:

```
Will's Grill - Control de Feria/     ← carpeta en Drive
 ├─ Respaldos/           → respaldo-control-feria.json (se actualiza solo)
 ├─ Facturas Mercado/    → cada foto de "Factura Mercado"
 └─ Facturas Gasolina/   → cada foto de "Gasolina"
```

Si no está conectado, o no hay internet, la app sigue funcionando 100% normal — Drive es una capa extra, no un requisito.

## 📊 Exportar a Excel

Desde la pestaña **"Resumen mensual"**, con un toque descargas un `.xlsx` con 3 hojas:

| Hoja | Contenido |
|---|---|
| **Totales** | Ventas, gastos, utilidad, consignado, propinas del filtro elegido |
| **Resumen por feria** | Una fila por feria con sus totales |
| **Movimientos** | Detalle completo: fecha, día, tipo, trabajador, valor, y **link directo a la foto en Drive** |

Puedes filtrar por mes, por rango de fechas exacto, por una sola feria, o traer todo.

## 🛠️ Por dentro

Un solo archivo `index.html`. Nada de instalar, nada de compilar.

- **Vanilla JavaScript** — sin frameworks, sin build.
- **localStorage** — toda la información vive en el navegador.
- **Chart.js** — la gráfica de gastos por categoría.
- **SheetJS (xlsx)** — genera el Excel en el propio navegador.
- **Google Identity Services + Drive API** — conexión directa con Drive, sin backend propio.

## 💾 Respaldo

Además de Drive, siempre puedes usar los botones **"⬇ Respaldo"** / **"⬆ Restaurar"** para guardar o recuperar un `.json` con todo — tu red de seguridad manual, pase lo que pase.

---

<div align="center">

Hecho a la parrilla 🔥 para **Will's Grill**

</div>
