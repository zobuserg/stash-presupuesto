# 💸 Stash — 20/50/30 budgeting for irregular income

**[English](#english) · [Español](#español)**

🔗 **Open it now / Ábrela ahora:** **[dantedanielgm.github.io/stash-presupuesto](https://dantedanielgm.github.io/stash-presupuesto/)**

---

<a name="english"></a>
## English

**An envelope-budgeting app built for people who get paid in halves, carry real debt, and live real money — not perfect-spreadsheet money.**

No account, no install, no cost. Works on your phone and your computer, in **English and Spanish** (pick your language on the welcome screen or with the 🌐 button). Your data never leaves your device.

### Why it exists

Traditional budgets assume one fixed paycheck on the 30th and zero debt. Real life for a lot of people isn't that: you get paid in parts, you carry revolving credit cards at brutal interest rates, and sometimes you're planning the next cycle before the money has even landed.

Stash takes an old, simple idea — **pay yourself first** — and makes it executable. That's why the rule isn't 50/30/20 but **20/50/30**: the 20% savings comes out **first**, not from whatever's left.

| | |
|---|---|
| 🟢 **20% Savings** | Every sol that raises your net worth: paying debt, cushion, goals, investing. |
| 🔵 **50% Needs** | Housing, food, transport, health, education. |
| 🟡 **30% Wants** | What makes life worth living. |

### What makes it different

- **📅 Half-month native.** Not a monthly budget with patches. Every cycle (half-month, month, or custom period) is its own statement: you open with X, move money, close with Y.
- **💳 Revolving debt as a first-class citizen.** Cards are modeled as what they are (credit limit, available, minimum, APR) and the app tells you the uncomfortable truth: at 165% APR, charging the card is a trap, not a bridge. It prioritizes what to pay first (snowball).
- **🚦 Debt at a glance.** Each debt is one row: what you owe, when it's due, and a green/amber/red dot. Loans are simple (balance + installment + date); the full credit machinery only appears for cards.
- **🌊 Automatic cascade.** Overspend one box and the excess is covered from wherever there's balance — no manual math, no unmanageable negative numbers.
- **💰 Live two-way counter.** "On hand" drops with every expense you check ✓ and rises when you mark income as arrived. Money that hasn't landed shows as *incoming*, not as a lying red number.
- **⚡ Quick expense in 2 taps.** Floating button → amount → done. Logged and deducted instantly.
- **🔒 Honest Reserve.** When you check savings, the app asks plainly: *was it paid out, or did it stay in your Reserve?* Every sol knows where it went.
- **🌎 Free, bilingual, no account.** One link you share over WhatsApp. Your family opens it and uses it.

### How to use it

1. **Open the link** → [dantedanielgm.github.io/stash-presupuesto](https://dantedanielgm.github.io/stash-presupuesto/)
2. Pick your language, enter the amount you're splitting and the period it covers.
3. Spread it across the 3 boxes, add your debts, check ✓ what you pay.
4. When the cycle ends, **close it** and the app carries the result into the next one.

**Install as an app (optional):** on your phone, open the link → browser menu → **"Add to Home Screen"**. It behaves like a native app and works offline.

**Move your data between devices:** data lives **only in your browser** (there is no server). Use **⬇ Export backup** on one device → **⬆ Import backup** on the other. That file is also your safety net.

### Privacy

**Zero backend. Zero accounts. Zero telemetry.** Everything is stored in your own browser's `localStorage`. Nobody — including the author — sees your numbers. If you wipe your browser data it's gone; that's what Export/Import is for.

### How it's built

Stash is **a single HTML file** (`index.html`) with everything inside: markup, styles, and logic. No frameworks, no JS build step, no external dependencies.

- **Guiding principle — "the spiderweb":** one source of truth + derived state. Touch one thing and everything updates (reactive full re-render). No two numbers can drift apart.
- **i18n:** a tiny inline `tx('español','english')` helper — Spanish lives in the code as the source, English travels beside it. No separate dictionaries to fall out of sync.
- **PWA:** `manifest.webmanifest` + `sw.js` (network-first for HTML, so updates arrive on their own).
- **Persistence:** `localStorage`, with JSON Export/Import.

### Status

**Live beta (July 2026).** The core is solid and used daily with real data. It evolves by use: every friction found in the street gets fixed and republished at the same link.

---

<a name="español"></a>
## Español

**Una app de presupuesto por sobres, hecha para quien cobra por quincenas, arrastra deudas y vive la plata de verdad — no la del Excel perfecto.**

Sin cuenta, sin instalar, sin costo. Funciona en el celular y en la compu, en **español e inglés** (eliges el idioma en la pantalla de bienvenida o con el botón 🌐). Tus datos nunca salen de tu dispositivo.

### Por qué existe

Los presupuestos tradicionales asumen un sueldo fijo el día 30 y cero deudas. La vida real de mucha gente no es así: te pagan por partes, tienes tarjetas revolviendo al 165% de interés, y a veces el sueldo aún no cae cuando ya estás planificando.

Stash nace de una idea vieja y simple —**"págate a ti primero"**— y la vuelve ejecutable. Por eso la regla no es 50/30/20 sino **20/50/30**: el 20 de ahorro va **primero**, no con lo que sobra.

| | |
|---|---|
| 🟢 **20% Ahorro** | Todo sol que sube tu patrimonio: pagar deuda, colchón, metas, invertir. |
| 🔵 **50% Necesidades** | Techo, comida, transporte, salud, educación. |
| 🟡 **30% Gustos** | Lo que hace que la vida valga la pena vivirla. |

### Qué lo hace distinto

- **📅 Quincena nativa.** No es un presupuesto mensual parchado. Cada ciclo (quincena, mes o periodo libre) es un estado de cuenta propio: abres con X, te mueves, cierras con Y.
- **💳 Deuda revolvente de primera clase.** Modela tarjetas como lo que son (línea, disponible, mínimo, TCEA) y te dice la verdad incómoda: a 165% de interés, tarjetear es trampa, no puente. Prioriza qué pagar primero (bola de nieve).
- **🚦 Deudas de un vistazo.** Cada deuda es una fila: cuánto debes, cuándo vence y un punto verde/ámbar/rojo. El préstamo es simple (saldo + cuota + fecha); la maquinaria de crédito completa solo aparece en tarjetas.
- **🌊 Cascada automática.** Si te pasas en una caja, el sobrante se cubre solo desde donde hay saldo — sin que hagas la resta a mano. Nunca ves un número negativo que no puedas administrar.
- **💰 Contador vivo bidireccional.** "Tengo ahora" baja con cada gasto que marcas ✓ y sube cuando marcas que te llegó un ingreso. Lo que aún no cae se ve como *en camino*, no como un rojo mentiroso.
- **⚡ Gasto suelto en 2 taps.** Botón flotante → monto → listo. Se anota y baja de tu plata al instante.
- **🔒 Reserva honesta.** Cuando marcas ahorro, la app pregunta claro: *¿se pagó o quedó en tu Reserva?* Cada sol sabe a dónde fue.
- **🌎 Gratis, bilingüe, sin cuenta.** Un link que compartes por WhatsApp. Tu familia lo abre y lo usa.

### Cómo se usa

1. **Abre el link** → [dantedanielgm.github.io/stash-presupuesto](https://dantedanielgm.github.io/stash-presupuesto/)
2. Elige tu idioma, pon cuánta plata vas a repartir y qué periodo cubre.
3. Reparte en las 3 cajas, agrega tus deudas, marca ✓ lo que pagas.
4. Al terminar el ciclo, **ciérralo** y la app pasa el resultado al siguiente.

**Instalar como app (opcional):** en el celular, abre el link → menú del navegador → **"Agregar a pantalla de inicio"**. Queda como app nativa y funciona offline.

**Mover tus datos entre dispositivos:** los datos viven **solo en tu navegador** (no hay servidor). Usa **⬇ Exportar copia** en uno → **⬆ Importar copia** en el otro. Esa copia también es tu red de seguridad.

### Privacidad

**Cero backend. Cero cuentas. Cero telemetría.** Todo se guarda en el `localStorage` de tu propio navegador. Nadie —ni el autor— ve tus números. Si borras los datos del navegador, se van; por eso existe Exportar/Importar.

### Cómo está hecho

Stash es **un solo archivo HTML** (`index.html`) con todo adentro: estructura, estilos y lógica. Sin frameworks, sin build de JavaScript, sin dependencias externas.

- **Principio rector — "la telaraña":** una sola fuente de verdad + estado derivado. Mover una cosa mueve todo (full re-render reactivo). No hay dos números que puedan desincronizarse.
- **i18n:** un helper inline mínimo `tx('español','english')` — el español vive en el código como fuente, el inglés viaja al lado. Sin diccionarios aparte que se desincronicen.
- **PWA:** `manifest.webmanifest` + `sw.js` (red-primero para el HTML → las actualizaciones llegan solas).
- **Persistencia:** `localStorage`, con Exportar/Importar en JSON.

#### Desarrollo local

La fuente de verdad es **`presupuesto.html`** (en la carpeta de trabajo). La carpeta `web/` que ves en este repo es **derivada** — se regenera, no se edita a mano:

```powershell
# 1. Editas presupuesto.html
# 2. Regeneras la carpeta de despliegue:
.\build-pwa.ps1
# 3. Publicas el contenido de web/ (GitHub Pages lo sirve solo)
```

Para probar en local, basta abrir `presupuesto.html` en el navegador. No necesita instalación de nada.

### Estado

**Beta viva (julio 2026).** El núcleo es sólido y se usa a diario con datos reales. Sigue evolucionando por uso: cada fricción que aparece en la calle se arregla y se vuelve a publicar en el mismo link.

**Roadmap abierto:** cadencia de gastos recurrentes, historial de cierres (patrimonio neto por ciclo), id estable por deuda, y afinar el modelo de tarjeta con el interés real.

---

## Author / Autor

**Dante Daniel Gutiérrez Matos** ([@dantedanielgm](https://github.com/dantedanielgm)) — built conversationally with Claude Code, iterating on real half-month budgeting problems. / Construido de forma conversacional con Claude Code, iterando sobre problemas reales de presupuesto quincenal.

## License / Licencia

Open source for personal use. Reuse or adapt it freely — credit appreciated. / Código abierto para uso personal. Reutilízalo o adáptalo con libertad — un crédito se agradece.
