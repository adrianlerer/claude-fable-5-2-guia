# Claude Fable 5.2: Guía Completa

**Por Alejo (@ecommartinez) - 14 de noviembre de 2026**

Anthropic lanzó Claude Fable 5.2 el 9 de noviembre de 2026. En 48 horas, X se llenó de juegos, cortos de animación y escenas 3D hechos con un único prompt.

Fable 5.2 es el modelo más potente que Anthropic ofrece al público. Comparte el mismo modelo base con Claude Mythos 5.2, reservado a organizaciones verificadas por Anthropic.

En esta guía tienes dónde activarlo, cuánto cuesta, los trucos de la guía oficial de Anthropic, prompts listos para copiar y las demos que más se han compartido en X.

## Dónde usarlo y cuánto cuesta

Fable 5.2 está en todos los planes de pago de Claude. El plan gratuito no tiene acceso.

- En la app de Claude (web, escritorio y móvil): elige "Fable 5.2" en el selector de modelo.
- En Claude Code: necesitas la versión 2.1.321 o superior. Cambia de modelo con /model claude-fable-5-2.
- En la API: el identificador es claude-fable-5-2. También está en Amazon Bedrock, Google Cloud y Microsoft Foundry.

Según tu plan, el acceso cambia:

- Pro y Team estándar: Fable va con créditos de uso, a precio de API. Por el lanzamiento, Pro lo incluye sin coste extra hasta el 16 de noviembre.
- Max, Ultra y Team premium: incluido hasta el 50% de tu límite semanal. Gasta ese límite más rápido que otros modelos.
- API: 8 $ por millón de tokens de entrada y 40 $ por millón de salida. Es más barato que Fable 5.1, que costaba 10 $ y 50 $.

Trabaja con un contexto de 1 millón de tokens y genera hasta 128.000 tokens por respuesta. Tiene cinco niveles de esfuerzo: low, medium, high, xhigh y max.

## 9 trucos sacados de la guía oficial de Anthropic

Fable 5.2 no se maneja como los modelos anteriores. Estos ajustes vienen de las pruebas internas de Anthropic.

1. Sube el esfuerzo a high. En Claude Code y en la app arranca en medium. Escribe /effort high en Claude Code. Según Anthropic, la mayor parte de la mejora llega en high. Deja xhigh para tareas largas de código y max para problemas abiertos de ciencia o matemáticas.
2. Para que piense menos, baja el esfuerzo. Frases como "responde directo sin pensar" ya no frenan su razonamiento en medium o más. Pasa a low para tareas rápidas y bien definidas.
3. Dile quién es dueño del código. Si el proyecto es tuyo y quieres que ordene la estructura, díselo (tienes la frase en los prompts de abajo). En las pruebas de Anthropic, juntó el código duplicado en un 75% de los casos con la frase y en menos del 10% sin ella. A cambio gasta entre un 70% y un 80% más de tokens y toca cosas que no pediste.
4. Aprueba con frases concretas. Cambia "sigue" o un pulgar por "Sí, lanza la migración en la base de datos de pruebas".
5. Cuidado con la palabra "nunca". La toma al pie de la letra. Escribe "pide permiso antes de borrar archivos" en lugar de "nunca borres archivos".
6. No le pidas que escriba su razonamiento en la respuesta. Lo trata como una extracción de razonamiento y rechaza la petición.
7. Limpia tus prompts antiguos. Sigue las reglas de estilo al milímetro. Un límite como "una idea por frase, 20 palabras máximo" vuelve su texto entrecortado. Borra también las notas de memoria que ya no sirven.
8. Si para antes de terminar, pídele que siga hasta el final. Pasa más en low y medium. Tienes el prompt de persistencia abajo.
9. Prueba Opus primero. Anthropic aconseja empezar con Opus y pasar a Fable 5.2 cuando Opus en esfuerzo alto no llega. Fable cuesta más por token, así que guárdalo para lo difícil.

## 7 prompts listos para copiar

Cambia lo que va entre corchetes. Los dos primeros siguen las recomendaciones de Anthropic. Los demás se inspiran en las demos que han triunfado en X.

### 1. Para que termine la tarea sin pararse (agentes y tareas largas)

No te detengas mientras quede trabajo pendiente de lo que te pedí. Si encuentras errores, tiempos de espera o herramientas que fallan, analiza la causa y busca otra vía antes de parar. Si algo está bloqueado a propósito, déjalo, explícame qué encontraste y sigue con el resto. Pide confirmación antes de cualquier acción arriesgada o irreversible.

### 2. Para que ordene tu propio código

Eres el dueño de este proyecto y lo mantendrás a largo plazo. Las decisiones de diseño son tuyas. [Tarea]. Al final, lista todos los archivos que tocaste y por qué.

### 3. Un juego 3D jugable en el navegador

Haz un juego 3D jugable en el navegador, en un único archivo HTML con Three.js. La idea es [descripción del juego]. Incluye pantalla de inicio, controles con teclado y ratón, sonidos generados por código y una dificultad que suba poco a poco. No uses archivos externos.

### 4. Un vídeo de lanzamiento hecho en código

Haz un vídeo de lanzamiento de 30 segundos para [producto] usando HTML, CSS y JavaScript. Quiero tipografía animada, transiciones al ritmo de la música y una escena final con el logo. Prepáralo para grabarlo en 1080p.

### 5. Una escena 3D en Blender (con el MCP de Blender conectado)

Construye en Blender, con un script de Python, una escena de [descripción]: modelos, materiales, luces y un movimiento de cámara de 10 segundos. Renderiza una vista previa, revísala y corrige lo que no quede bien antes de darme el resultado.

### 6. Rediseñar tu web

Aquí tienes la URL de mi web: [URL]. Rediseña la página de inicio para [objetivo: más ventas, más registros]. Explícame en 5 puntos qué cambias y por qué, y luego dame el código completo.

### 7. Un documento largo con fotos

Te paso [contrato, informe o presupuesto] y estas fotos. Dime en lenguaje sencillo qué puntos me afectan, qué riesgos ves y qué preguntas debería hacer antes de firmar.

## Las demos más virales de X (con vídeo)

Estos posts muestran lo que la gente ya hace con Fable 5.2. Abre cada uno para ver el vídeo.

### Lo oficial de Anthropic

- La película de lanzamiento de Fable 5.2.
- Un pódcast sobre las pirámides de Egipto con cada fotograma dibujado en código.
- Un monumento centenario modelado a partir de 40 fotos e impreso en 3D en una pieza.

### Juegos jugables en el navegador

- @kevin_t_ngo hizo un combate contra un jefe al estilo souls, jugable en el navegador. Superó las 113.000 visualizaciones en un día.
- El mismo creador hizo un paseo en barca por 8 mundos de sueño.
- @theo dejó a Fable 5.2 trabajar 76 minutos en un juego, por unos 42 $ de tokens.
- @petergyang hizo un juego de karts en 3D.
- @mattshumer_ sacó un motor de vóxeles con un único prompt.

### Escenas 3D en Blender y Three.js

- @rileybrown pidió en directo una habitación completa en Blender. Fable 5.2 escribió el código que construye el escritorio, el portátil y la luz.
- @higgsfield_ai montó un bazar de Bombay en 6 planos, todo en código con Three.js.
- @deedydas simuló miel fotorrealista en WebGL.

### Vídeo y motion design

- @midudev hizo el tráiler de un producto en 10 minutos.
- @Stargridcompass convirtió 26 años del Nasdaq en un gráfico animado al ritmo de la música.

### Música

- @kloss_xyz dejó que Fable 5.2 escribiera su propia canción, la produjera en Suno y rodara el videoclip.

### Comparativas con el mismo prompt

- @petergyang enfrentó Fable 5.2 y Opus 5.5 en 5 casos de uso. Fable ganó 4 de 5.

### Para verlo todo de golpe

- @The_Alex publicó 2 horas de pruebas: Zelda, Halo, edición de vídeo, Photoshop y más.
- @EricBuess recopiló en un hilo los vídeos, juegos y mundos 3D de la comunidad.

## Fuentes

- Anthropic, What's new in Claude Fable 5.2
- Anthropic, Prompting Claude Fable 5.2
- Claude Help Center, Claude Fable 5.2 launch offers
- Claude Help Center, Claude Fable models on your plan
- Recopilación de vídeos hechos con Fable 5.2 en X (GitHub)

---

Artículo original publicado en X por @ecommartinez
