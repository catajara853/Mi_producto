# T2 · Guion del wizard-of-oz y montaje de la página

Prueba: T2 `avances-verificables` en `product/tests/2026-11-10-2054-confianza-plata-obra.md`.
La familia ve una página de avances; detrás, el constructor la actualiza a mano. No se construye ningún sistema.

## Lo que debe existir antes de arrancar (sin programar)

1. **Fotos con sello de fecha, hora y ubicación.** Una app de cámara que imprima esos tres datos sobre la foto (hay varias gratuitas del tipo "timestamp camera" [conocimiento del modelo — verificar cuál funciona bien en tu celular]). Activa el sello de fecha, hora y dirección o coordenadas.
2. **La página.** Una página privada que siga la estructura de `pagina-avances.html`: encabezado con la obra, y por cada día trabajado (el más reciente arriba) una entrada por espacio con una línea de qué se hizo y sus fotos. Opción sin código: Google Sites, publicada solo para quien tenga el enlace y con la opción de pedir a los buscadores que no la muestren activada [conocimiento del modelo — verificar que la opción exista en tu cuenta].
3. **El contador de visitas.** El enlace que se le manda a la familia pasa por un acortador de enlaces que muestre los clics por día (varios tienen plan gratuito [conocimiento del modelo — verificar]). Así cada entrada desde el chat queda contada, sin identificar a la persona.
4. **Prueba en seco.** Publica un día de ejemplo, abre el enlace corto desde otro celular y confirma que el clic aparece en el contador. Borra el clic de prueba o anótalo para restarlo.

Nada más: sin cambios, pagos, cotización, login ni app para descargar (decisión del diseño).

## Paso a paso durante la prueba

| Momento | Lo que ve la familia | Lo que pasa detrás | Tiempo |
|---|---|---|---|
| Día 0 | Nada nuevo | Llenas la línea base en `hoja-registro.md` contando el chat de las últimas 3 semanas | 30–45 min, una vez |
| Día 0 | Mensaje de consentimiento (`mensajes-familia.md`) | Esperas su sí por escrito. Sin consentimiento, la prueba no arranca | |
| Día 1 | El enlace corto, una sola vez, con su explicación de una línea | Primera publicación ya hecha antes de mandar el enlace | 2 min |
| Cada día trabajado | La página con lo del día | Al cerrar la jornada tomas las fotos con sello y publicas una entrada por espacio | Lo que tome |
| Cada día | Si pregunta por el avance, le respondes normal **sin mandar el enlace** | Anotas la pregunta en la hoja ese mismo día | |
| Fin de cada semana | Nada | Pasas el conteo de la semana a la hoja | 10 min |
| Día 21 | Nada | Cierras la hoja y la traes a `/analyze-solution-tests` | |

## Reglas para no contaminar la prueba

- No le recuerdes la página ni le reenvíes el enlace por WhatsApp después del día 1.
- No le preguntes si le gusta la página: lo que se mide es lo que hace, no lo que opina.
- Si un día no se trabaja, no se publica nada ese día. No publiques fotos de días anteriores como si fueran nuevas.
- Si la familia pide acceso para otra persona (por ejemplo, su veedor), anótalo en la hoja como observación y mándale el mismo enlace corto.
