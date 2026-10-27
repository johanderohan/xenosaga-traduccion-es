# Xenosaga I・II — Traducción al español

[![Invítame a un café en Ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/johanderohan)

Ficha del proyecto, capturas y más traducciones al castellano en **[Parches en Castellano](https://parchesencastellano.com/traducciones/nintendo-ds/xenosaga-i-ii)**.

Traducción al **español de España** de *Xenosaga I・II* (Nintendo DS, 2006),
la adaptación de Monolith Soft y Tom Create de los episodios I y II de
*Xenosaga*, publicada por Namco solo en Japón.

La traducción se distribuye como **parche**: no incluye el juego. Para aplicarlo
necesitas tu propia copia.

## Estado

Última versión: **[v1.0.2 — Teclado latino por defecto](../../releases/tag/v1.0.2)**.

Está traducido del japonés todo el texto del juego que se ha localizado:

| Parte | Estado |
|---|---|
| Guion (episodios I y II, historias secundarias y minijuegos) | **17.111 textos traducidos**: todos los que se han encontrado |
| Objetos, técnicas, éteres, enemigos, descripciones, correos y menús | **6.666 textos traducidos** |
| Glosario del juego (U.M.N.) | Traducido entero y reordenado alfabéticamente |
| Texto dentro de imágenes | **311 rótulos e iconos traducidos** (menús, combate, tarjetas de capítulo, minijuegos) |
| Caracteres españoles | **á é í ó ú ü ñ Á É Í Ó Ú Ü Ñ ¡ ¿ « »** |

Los rótulos grandes de marca y los que ya venían en inglés o en alemán en el
original (pantallas de título, «RESULT», los subtítulos alemanes de los
capítulos…) se mantienen como en el juego japonés.

### Comprobaciones y limitaciones

- La traducción se ha hecho desde el japonés con una biblia de términos, y cada
  bloque ha pasado una revisión editorial cruzada. Ha sido **asistida por IA**
  y **no ha tenido revisión humana independiente**.
- La v1.0.1 corrige los gráficos de opciones y museo. Solo cambia cuatro recursos respecto a v1.0; el menú de opciones se ha vuelto a probar en melonDS. La revisión del museo es estática.
- Se ha probado en emulador:
  - **melonDS**: una partida nueva desde el título (prólogo, tutorial de
    combate, menús de campo y de la U.M.N., tienda, guardado, carga y un combate
    normal hasta la pantalla de resultados), sin cuelgues; y **57 escenas**
    repartidas por los dos episodios, cargadas directamente y revisadas página a
    página con capturas.
  - **DeSmuME**: arranque, partida nueva y una escena del episodio II.
- **No se ha jugado de principio a fin.** Puede haber escenas que no se han
  visto en pantalla.
- **En consola real (DS, DSi o 3DS con flashcard) todavía no se ha probado.**
  El parche amplía un búfer interno para que quepan los diálogos en español;
  en emulador funciona, pero en hardware está pendiente de confirmar. Si lo
  pruebas en consola, abre una incidencia y cuéntame cómo ha ido.
- Al nombrar a la observadora de la serie 100, el teclado abre en letras latinas.
  X cambia de alfabeto. Se conserva el límite de siete caracteres, sin tildes ni ñ.
- Se ha recibido un aviso de nombres de hablante demasiado pequeños en consola;
  su mejora de legibilidad está pendiente.

## Cómo aplicar el parche

1. Descarga el parche `.xdelta` de la sección **[Releases](../../releases)**.
2. Consigue tu copia del juego en versión **japonesa**. El parche solo funciona
   con esa versión exacta.
3. **Antes de nada, comprueba que tu copia es la correcta**:

   | | |
   |---|---|
   | Archivo | `Xenosaga I & II (Japan).nds` |
   | Tamaño | 67.108.864 bytes (64 MB) |
   | MD5 | `6a94137d9ff8441c6f88b356409fd305` |

   ```bash
   md5sum "Xenosaga I & II (Japan).nds"     # Linux
   md5 "Xenosaga I & II (Japan).nds"        # macOS
   CertUtil -hashfile "Xenosaga I & II (Japan).nds" MD5   # Windows
   ```

   Si no coincide, el parche fallará o dará un resultado corrupto.
4. Aplica el parche con una de estas herramientas:
   - **Windows**: [Delta Patcher](https://github.com/marco-calautti/DeltaPatcher/releases)
   - **Linux / macOS**: `xdelta3 -d -s "Xenosaga I & II (Japan).nds" parche.xdelta "Xenosaga I & II (ES).nds"`
5. Para **v1.0.2**, la ROM resultante debe tener MD5 **`27313bd3762a23ae93e1f8ddc09ed323`**.
6. Carga la ROM resultante en tu emulador o flashcard.

Aplica cada versión sobre la **ROM japonesa original**, nunca sobre una ROM ya
traducida.

## Cambios

- **v1.0.2 (27-10-2026)** — Teclado latino seleccionado al abrir y ayuda «X: alfabeto». Probados escritura, borrado, cambio de alfabeto y confirmación en melonDS. Se conserva el formato de las partidas.

- **v1.0.1 (21-10-2026)** — Traduce el menú de opciones, sus valores y los rótulos del museo, que se habían omitido en v1.0. Comprobados en melonDS los ajustes, el resaltado de filas, restaurar valores y guardar/salir. Las partidas de v1.0 conservan su formato.

- **v1.0** — Primera versión: guion completo, datos del juego, glosario y
  rótulos de menús y combate.

## Aviso

Este proyecto es una traducción hecha por afición, sin ánimo de lucro y sin
relación alguna con Monolith Soft, Tom Create, Namco ni Bandai Namco. Aquí no se
distribuye el juego ni ninguna parte de él: solo un parche que modifica una copia
que ya tengas.

Si eres el titular de los derechos y quieres que retire esto, abre una incidencia
y lo hago.
