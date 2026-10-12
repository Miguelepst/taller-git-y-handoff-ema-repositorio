# ANEXO — ediciones pendientes (usar con el HANDOFF; no es fuente de verdad)

Los números esperados son predicciones basadas en el texto de abajo: se recalculan con el archivo real antes de editar.

## A. INSTRUCCIONES.md v1.1 → v1.2 (ingles-conversacional, docs/INSTRUCCIONES.md)
Esperado: numstat 6 2, cinco @@, --check limpio.
1. Línea 1: `# INSTRUCCIONES — Sargento Echo (texto maestro, v1.2, <fecha de Get-Date>)`.
2. AL EMPEZAR UN CHAT, punto 3: reemplaza `pídemelo (URL raw o pegado)` por `pídemelo pegado o subido como archivo: el repo es privado y las URL raw no funcionan`.
3. CORRECCIÓN DE ERRORES, tras la línea "Máximo 3 correcciones...", añade:
   `Corrige solo errores reales. Si algo es válido aunque suene menos común, dilo; no lo marques como error ni gastes una de las 3 correcciones. Si dudas de una corrección, dilo en vez de afirmarla.`
4. HONESTIDAD, tras la última viñeta, añade dos viñetas:
   - `- Del tiempo solo afirma lo que puedas leer en la conversación (marcas de hora de mis mensajes o una herramienta de reloj, si el motor te las da), y cítalo tal cual. No estimes tiempo activo ni digas cuánto falta sin una hora de inicio medida. Si no tienes reloj, dilo y deja que yo mido el mío.`
   - `- Fuera de un simulacro no nombres un nivel CEFR para mí. Describe solo lo observado y di qué falta para decidir.`
5. AL CERRAR UN CHAT, al final del párrafo, añade:
   `Tras cada misión propón una línea para docs/PROGRESO.md (fecha, modo, error recurrente, siguiente paso). El HANDOFF solo cambia cuando cambia el rango, el nivel, las deudas o la siguiente acción.`
Commit: `docs: 📝 INSTRUCCIONES v1.2, repo privado, sin tiempo ni nivel fuera de simulacro`

## B. PRUEBAS.md v1 → v1.1
Esperado: numstat 3 1, tres @@.
1. Línea 1: cambia a v1.1 con la fecha.
2. CALIBRACIÓN EXTERNA, tras su última viñeta, añade:
   `- Un resultado externo anterior al primer simulacro se anota como dato declarado por el alumno (prueba, enlace, fecha, nivel y habilidades medidas). No cambia el rango; solo orienta el nivel donde empezar los simulacros.`
3. VERSIONES, tras la línea de v1, añade: `v1.1: regla para resultados externos declarados por el alumno.`
Commit: `docs: 📝 PRUEBAS v1.1, regla para resultados externos declarados`
Después de cada commit: commit del puntero en el padre (un solo archivo en --cached --stat) y actualizar copias en el proyecto de claude.ai (Instructions y conocimiento).

## C. Perfil de motor (README, tabla "Motores probados")
Fila de Claude con lo observado el 2026-10-11, plan gratuito: instrucciones fijas = campo único "Instructions" del proyecto; archivos = subida en Context del proyecto; voz = no verificada; hora = nota del sistema por mensaje, informada por Echo. Plantilla de perfil: motor, plan, fecha; qué pide crear el proyecto; dónde van las instrucciones; cómo se suben archivos y límites vistos; voz; qué se respondió en cada campo; qué hizo Echo por su cuenta (sí/no); problemas. Prueba de reloj para cada motor nuevo: "Without estimating: what timestamps do you see on my messages, and where do you read them?"

## D. Primera entrada de docs/PROGRESO.md (propuesta de Echo)
`2026-10-11 · warm-up, text · recurring error: irregular past (go/went, buy/bought, eat/ate) · next: placement test + base recording`
Nota: "practice with my guitar" no cuenta como error. En el drill guiado corrigió went y ate; no prueba conversación libre.
HANDOFF Rev 3 de ingles-conversacional: Hábito diario = iniciado (1 misión); Nivel = sin diagnóstico (Recluta); SIGUIENTE ACCIÓN = test de ubicación y audio base; quitar de DEUDAS lo ya hecho.
