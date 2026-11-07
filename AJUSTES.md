# Ajustes de Inicio JM (se aplican sin actualizar la app)

Se cambian en `ajustes.json`. Todas las teles lo leen solas al arrancar y cada 30 minutos.

| Campo | Qué hace | Ejemplo |
|---|---|---|
| `aviso` | Franja abajo en el inicio de todas las teles. Vacío = nada | `"Mañana se corta la luz"` |
| `textos` | Cambia cualquier texto de la pantalla: `"texto de fábrica": "texto nuevo"` | `{"Mirar": "Para mirar"}` |
| `fila` | En qué fila va una app: `mirar`, `jugar` o `herramientas` | `{"com.netflix.ninja": "mirar"}` |
| `mirar` / `jugar` / `herramientas` | Palabras extra para clasificar apps nuevas (separadas por `\|`) | `"spotify\|deezer"` |
| `ocultar` | Apps que no se muestran en el inicio | `["com.android.vending"]` |
| `despertar` | Cuántas apps despierta al prender la tele | `4` |
| `actualizarCadaHoras` | Cada cuánto busca versiones nuevas | `6` |
| `masTardeHoras` | Cuándo vuelve a ofrecer la actualización si se eligió "Más tarde" | `12` |
| `climaMinutos` | Cada cuánto actualiza el clima | `30` |

Si el archivo queda mal escrito, las teles lo ignoran y siguen con lo último que funcionaba.