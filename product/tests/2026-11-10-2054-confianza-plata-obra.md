---
opportunity: confianza-plata-obra
solutions: product/solutions/2026-11-10-2038-confianza-plata-obra.md
status: ready
---

# Solution tests for: Confianza con la plata durante la obra

## Why test
Se prueban A2 (cambios-con-precio) y A1 (avances-verificables), más la condición del sponsor de usar un portal web. Para las dos alternativas, el dolor solo está evidenciado en el ensayo sintético e investigación secundaria: nadie ha reaccionado todavía a una orden de cambio con precio ni a avances con fecha y ubicación.

## Cambio de diseño (2026-11-10, antes de correr)
El sponsor consideró demasiado larga la versión original (cerca de 6 semanas: una prueba de 3 semanas en la obra en curso y sesiones que dependían de la encuesta) y eligió una versión de **1 semana**: una tarde de sesiones de 20 minutos con 6 familias, en las que se muestran la orden de cambio (T1) y una página de avances de ejemplo (T2), y se pide un compromiso concreto por cada una. La IA había recomendado una versión de 2 semanas que medía uso real (registrado en `product/corrections.md`).
**Lo que se pierde:** las dos pruebas miden interés con un compromiso, no uso real. T3 (¿entran al portal sin recordatorio?) no se puede medir en una sesión y queda aplazada. Las versiones largas quedan como siguiente paso si estas pasan.

## T1. cambios-con-precio: orden de cambio mostrada con compromiso
- **Test status:** ready
- **Belief under test:** "Cuando cada cambio llega con su valor y días extra antes de aprobarse, la familia decide sin roce y al terminar la obra no reclama sobrecostos por cambios." (#7)
- **Risk:** [value]
- **Test type:** prototype-shown
- **What we do:** en la primera parte de una sesión de 20 a 25 minutos (videollamada o en persona):
  1. La familia recuerda el último cambio que pidió en su obra.
  2. Se le muestra ese mismo cambio escrito como orden de cambio: qué cambia, valor, días extra, fecha límite y "Apruebo / No apruebo".
  3. Se le ofrece una sola vez, con las mismas palabras para todas, la plantilla para usarla con su constructor o en su próxima obra.
- **With whom:** 6 familias del segmento (no supervisan a diario; obra en curso o terminada hace menos de 2 años; Medellín, Rionegro u oriente). Se reclutan esta semana, sin esperar la encuesta: referidos de los contactos del constructor y mensajes directos en el grupo de propietarios. Los contactos que ya son clientes del constructor solo entran si no hay más, y se marcan en la hoja porque tienden a responder a favor. Se excluye al cliente de la obra en curso.
- **Material needed:** la orden de cambio de una página, la plantilla (mensaje de WhatsApp y cláusula), el guion de la sesión, la hoja de registro y el mensaje de reclutamiento. Se deja por fuera a propósito: el portal, la marca del constructor y cualquier precio de la obra completa.
- **Material:** [product/tests/materials/t1-cambios-con-precio/](materials/t1-cambios-con-precio/): guion y hoja de registro compartidos con T2.
- **Duration:** 1 semana (las 6 sesiones)
- **Signal and threshold:** al menos 3 de 6 familias del segmento **piden la plantilla** al final de la parte de T1.
- **Decision rule:**
  - **continue** si 3 o más la piden.
  - **change** si la piden exactamente 2: el mecanismo atrae a algunos; se revisa el formato (cláusula vs. mensaje) antes de la siguiente prueba.
  - **discard** si 1 o ninguna la pide.
- **Expected provenance:** real. Mide interés con compromiso, no uso: si pasa, la creencia queda prometedora, no confirmada.
- **Next step if it passes:** concierge en la obra en curso y en la próxima: todo cambio pasa por orden de cambio con precio y días antes de ejecutarse, y al cierre de obra se cuentan los reclamos por sobrecostos de cambios (meta: 0). Incluye el seguimiento de uso que esta versión dejó por fuera.

## T2. avances-verificables: página de avances de ejemplo con compromiso
- **Test status:** ready
- **Belief under test:** "Con avances con fecha, hora y ubicación en el portal, la familia deja de mandar a su veedor y pregunta por el avance menos de una vez por semana." (#8)
- **Risk:** [value]
- **Test type:** prototype-shown
- **What we do:** en la segunda parte de la misma sesión, después de T1:
  1. La familia cuenta cómo se enteraba del avance de su obra y si mandaba a alguien a revisar.
  2. Se le muestra en el celular una página de avances de ejemplo, armada con fotos reales de la obra en curso del constructor (con sello de fecha y hora; sin la dirección exacta ni datos de esa familia).
  3. Se le ofrece una sola vez, con las mismas palabras para todas, un mensaje listo para pedirle a su constructor (o al de su próxima obra) avances así.
- **With whom:** las mismas 6 familias de T1.
- **Material needed:**
  - La página de ejemplo con fotos reales, siguiendo la estructura de `pagina-avances.html`, con permiso escrito del cliente de la obra en curso para mostrar las fotos.
  - El mensaje para pedirle avances al constructor.
  - La parte de T2 en el guion y en la hoja de registro compartidos con T1.
  - Se deja por fuera a propósito: cambios, pagos, cotización, login y app para descargar.
- **Material:** [product/tests/materials/t2-avances-verificables/](materials/t2-avances-verificables/) (página de ejemplo y mensaje para pedir avances) y [product/tests/materials/t1-cambios-con-precio/](materials/t1-cambios-con-precio/) (guion y hoja de registro compartidos). Los archivos de la prueba de 3 semanas (guion de montaje, hoja de línea base, mensajes para el cliente) quedan para el siguiente paso.
- **Duration:** 1 semana (las mismas 6 sesiones)
- **Signal and threshold:** al menos 3 de 6 familias del segmento **piden el mensaje** para pedirle avances a su constructor.
- **Decision rule:**
  - **continue** si 3 o más lo piden.
  - **change** si lo piden exactamente 2, o si en lo que dicen aparece que seguirían mandando a su veedor igual: se prueba A4 (veedor invitado) sobre la misma página.
  - **discard** si 1 o ninguna lo pide.
- **Expected provenance:** real. Mide interés con compromiso, no si la familia deja al veedor: si pasa, la creencia queda prometedora, no confirmada.
- **Next step if it passes:** el wizard-of-oz de 3 semanas en la obra en curso, con línea base y conteo de preguntas, visitas y envíos de veedor (material listo en `materials/t2-avances-verificables/`).

## T3. portal: ¿la familia entra sin que se lo recuerden?
- **Test status:** ready (aplazada: no cabe en la versión de 1 semana; corre junto con el siguiente paso de T2)
- **Belief under test:** "Las familias abren el portal al menos una vez por semana sin que se les recuerde por WhatsApp." (#9)
- **Risk:** [usability]
- **Test type:** usage-observation (misma corrida del siguiente paso de T2)
- **What we do:** durante las 3 semanas del wizard-of-oz de T2, se cuentan las visitas a la página. Después del primer envío del enlace no se manda ningún recordatorio ni enlace por WhatsApp. Si la familia pregunta por el avance, se le responde, pero sin el enlace.
- **With whom:** la familia de la obra en curso (n=1).
- **Material needed:** el contador de visitas de la página (por día, sin identificar a la persona) y una columna en la hoja de registro.
- **Material:** [product/tests/materials/t3-portal/](materials/t3-portal/): hoja de registro. Reutiliza el contador y el guion de montaje de T2.
- **Duration:** las mismas 3 semanas del siguiente paso de T2
- **Signal and threshold:** al menos 1 visita en cada una de las semanas 2 y 3, sin recordatorios.
- **Decision rule:**
  - **continue** si se cumple.
  - **change** si solo entra en la semana 1, o entra cuando se le manda el enlace: el formato web no se adopta solo, y los avances se llevan dentro de WhatsApp (un enlace por actualización).
  - **discard** del portal como formato si no entra nunca.
- **Expected provenance:** real. Con n=1 es direccional.
- **Next step if it passes:** usability-test con 5 familias del segmento haciendo una tarea real en la página (encontrar qué se hizo un día dado y aprobar un cambio), antes de construir más.

## Results

### Corte parcial 2026-11-10 (1 de 6 sesiones)
- **T1 cambios-con-precio:** 1 familia (cliente del constructor; obra terminada hace < 2 años en Medellín; supervisión a diario: sin dato). Pidió la plantilla. Provenance: real. Result: inconclusive (1 de 6; participante cliente del constructor, cuya respuesta se lee aparte; segmento sin confirmar). Decision: ninguna; completar las 5 sesiones restantes como está diseñado, priorizando familias que no sean clientes.
- **T2 avances-verificables:** la misma familia. Antes mandaba a su papá a revisar la obra. Pidió el mensaje. Provenance: real. Result: inconclusive (mismas razones). Decision: ninguna; completar las sesiones.
- **T3 portal:** not run (aplazada en la versión de 1 semana).
- Nota: la sesión mostró que la prueba se puede hacer como está diseñada. Faltan en la hoja las frases textuales y si la familia supervisaba la obra a diario.

## Decision
(Lo agrega /analyze-solution-tests.)
