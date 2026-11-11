---
opportunity: confianza-plata-obra
status: testing-several
chosen: cambios-con-precio, avances-verificables
tests: product/tests/2026-11-10-2054-confianza-plata-obra.md
---

# Solutions for: Confianza con la plata durante la obra

## What the evidence says now
- No hay evidencia real todavía: la encuesta y las entrevistas siguen pendientes.
- #2 [opportunity] [value]: prometedora en el ensayo sintético (quienes no supervisan verifican con esfuerzo y costo). Sin verificar.
- #3 [opportunity] [viability]: weakened por el ensayo sintético (en 6 de 9 casos los atrasos fueron por caja, no por falta de evidencia).
- #5 [product]: weakened por el ensayo sintético (los sobrecostos vinieron de cambios aprobados sin precio).
- Mercado (secondary): las quejas en la SIC piden cambios por escrito; las herramientas de EE. UU. se venden por "transparencia con el propietario".

## Baseline: what people do today
Fotos por WhatsApp cuando el constructor se acuerda, visitas sin avisar que cuestan medio día de trabajo, un veedor de confianza (familiar o arquitecto pagado) que va a mirar, y cambios aprobados con un "sí" por chat y cobrados después.
Fuentes: `product/insights/2026-11-10-2023-ensayo-confianza-plata-obra.md` (synthetic); `product/research/2026-11-09-2056-mercado-cotizador-obra.md` (secondary). Hay que contrastarlo con las entrevistas reales.

## Constraints added by the sponsor
- El constructor quiere probar en un formato formal: un portal o página web simple a la que entre el cliente, no una super app.

## Alternatives
### A1. Avances con evidencia verificable (`avances-verificables`)
Fotos y videos con fecha, hora y ubicación que no se pueden reutilizar, organizados por espacio, en una página web por obra. Ataca la desconfianza en las fotos del constructor. Para Camila y Andrés (primary) y Jhon Fredy (tertiary). Reemplaza las fotos sueltas por WhatsApp.

### A2. Control de cambios con precio antes de aprobar (`cambios-con-precio`)
Cada cambio lleva su valor y los días extra, y la familia lo aprueba por escrito antes de ejecutarlo, con fecha límite para pedir cambios por etapa. Une la idea aparcada de "registro de cambios con fecha límite" con una orden de cambio. Para Luz Marina y Hernán y Camila y Andrés (primary). Reemplaza el "sin problema" por chat. Su versión mínima es una plantilla de WhatsApp más una cláusula de contrato.

### A3. Pagos atados a hitos visibles (`pagos-por-hito`)
El plan de pagos se define por hitos y cada cobro va con la evidencia de que el hito se cumplió. Para Luz Marina y Hernán y Jhon Fredy.

### A4. El veedor de la familia entra al proyecto (`veedor-invitado`)
El constructor invita formalmente al familiar o asesor que la familia elija: acceso a los avances, una visita por hito y un acta firmada. Para Jhon Fredy y las familias que no pueden ir.

### A5. Calendario de pagos según la caja del cliente (`pagos-segun-caja`)
Una política: los cobros se cuadran desde el contrato con la quincena, la prima, el desembolso del crédito o el giro desde el exterior, y cada cobro se avisa con anticipación. No es software.

## Comparison
| Alternative | Desirable | Feasible | Viable | Riskiest belief |
|---|---|---|---|---|
| A1 | mixed: 2 de 12 desconfían de las fotos del constructor (synthetic); pain evidenced, relief not tested | to check with tech | mixed: menos preguntas de avance (assumption) | Con evidencia con fecha y ubicación, la familia deja de mandar a su veedor y de preguntar por el avance |
| A2 | mixed: 5 de 12 con sobrecosto por cambios sin precio; sin roce en los 4 casos con precio previo (synthetic); la SIC pide cambios por escrito (secondary); pain evidenced, relief not tested | strong (assumption: es un proceso que controla el constructor) | mixed: ataca menos discusiones por plata y más satisfacción (synthetic) | Con el precio y los días delante antes de aprobar, la familia decide sin roce y al final no reclama sobrecostos |
| A3 | weak: solo 2 de 9 atrasos fueron por falta de evidencia (synthetic) | to check with tech | weak: la creencia #3 está weakened | Los pagos se atrasan porque falta evidencia del hito |
| A4 | mixed: 5 de 12 ya usan veedor (synthetic) | strong (assumption) | unknown: puede sumar reclamos | Sumar al veedor reduce la ansiedad y las preguntas, en vez de sumar reclamos |
| A5 | mixed: 6 de 9 atrasos fueron por caja (synthetic) | mixed: depende del capital de trabajo del constructor (assumption) | mixed: evita obras paradas (synthetic) | Si los cobros se cuadran con la caja, la plata llega a tiempo y la obra no se para |

Nota: toda la evidencia de deseabilidad es sobre el problema, no sobre la solución. Por eso ninguna pasa de mixed.

## Decision
El constructor (sponsor) eligió probar A2 y A1 en paralelo, igual que la recomendación. Razones: A2 tiene la señal más fuerte, es la más barata y ataca directo el primer resultado del sponsor; A1 es la base natural del portal que el sponsor quiere y se cae por otra creencia. Las dos caben en una sola página web por obra, lo que además prueba la creencia de que las familias entran al portal.

## To test
- A2: "Con el precio y los días delante antes de aprobar, la familia decide sin roce y al final no reclama sobrecostos". Es la que la mata: si con el precio delante igual hay reclamos, controlar los cambios no resuelve la desconfianza.
- A1: "Con evidencia con fecha y ubicación, la familia deja de mandar a su veedor y de preguntar por el avance". Es la que la mata: si la familia sigue necesitando a su veedor, la evidencia del constructor no aporta confianza.
- Transversal: "Las familias abren el portal al menos una vez por semana sin que se les recuerde por WhatsApp". Si no lo abren, ninguna de las dos funciona en formato web.

Diseño de las pruebas: [product/tests/2026-11-10-2054-confianza-plata-obra.md](../tests/2026-11-10-2054-confianza-plata-obra.md) (T1: cambios-con-precio; T2: avances-verificables; T3: uso del portal).

## Value proposition: cambios-con-precio (A2)
- Pain relieved: enterarse del costo de un cambio cuando ya está hecho y no se puede deshacer (5 de 12 en el ensayo sintético; entre $1,4 y $8,4 millones).
- Gain created: cada decisión de cambio se toma sabiendo cuánto cuesta y cuánto atrasa; no hay sorpresas en la cuenta final.
- Replaces: el "sin problema" por chat y la cuenta que llega después; la familia lo cambia porque hoy esa sorpresa le cuesta plata y le daña la relación con el constructor.
- Deliberately does not: cotizar la obra completa, recomendar acabados ni impedir cambios; solo pone el precio antes del "sí".

## Value proposition: avances-verificables (A1)
- Pain relieved: no saber si la obra avanza como dicen, y tener que perder medio día o depender de un familiar para verificar (ensayo sintético: Paula, Luisa, Lina, Valentina).
- Gain created: ver el avance real, con fecha y lugar, desde el celular y sin pedírselo a nadie.
- Replaces: las fotos sueltas por WhatsApp y las visitas sin avisar; la familia lo cambia porque hoy verificar le cuesta tiempo, favores o plata.
- Deliberately does not: ligar el avance a los pagos (eso es A3, aparcada), dar acceso a terceros (A4, aparcada) ni ser una app que haya que descargar.

## Beliefs
Registradas en `product/overview.md` (#7 a #11).
- [opportunity: confianza-plata-obra] [value] (#2 del overview, referenciada)
- [opportunity: confianza-plata-obra] [viability] (#3 del overview, referenciada; weakened)
- [feature: cambios-con-precio] [value] Cuando cada cambio llega con su valor y días extra antes de aprobarse, la familia decide sin roce y al terminar la obra no reclama sobrecostos por cambios.
- [feature: cambios-con-precio] [feasibility] El constructor puede dar el valor y los días de un cambio en menos de 24 horas sin frenar la obra.
- [feature: avances-verificables] [value] Con avances con fecha, hora y ubicación en el portal, la familia deja de mandar a su veedor y pregunta por el avance menos de una vez por semana.
- [feature: avances-verificables] [usability] Las familias abren el portal al menos una vez por semana sin que se les recuerde por WhatsApp.
- [feature: avances-verificables] [feasibility] Subir los avances con fecha y ubicación le toma al constructor menos de 10 minutos por día de obra.

## Discarded or parked
- A3, pagos por hito: parked. El ensayo dice que los atrasos son por caja. Vuelve si las entrevistas reales muestran pagos frenados por falta de evidencia.
- A4, veedor invitado: parked. Es barata de agregar después; primero hay que ver si A1 reduce la necesidad del veedor.
- A5, pagos según la caja: parked. Es una política que el constructor puede adoptar sin herramienta, pero resuelve más su caja que la confianza del cliente.

## Outcome
(Lo agrega /analyze-solution-tests.)
