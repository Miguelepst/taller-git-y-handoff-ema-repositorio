# HANDOFF — Taller Git y handoff (fuente de verdad: este archivo, no el chat)

Actualizado: <generar con Get-Date -Format 'yyyy-MM-dd HH:mm'> (UTC-5) · Rev 1. Traspaso desde el chat largo inicial.

## CONTEXTO
Miguel. Windows 11, PowerShell 7.6.6, Git portable, CudaText. Dos líneas de trabajo:
(A) aprender y auditar con Git: diffs quirúrgicos, commits atómicos, instrucciones dadas por otras IAs.
(B) construir el proyecto ingles-conversacional: repo privado, submódulo del repo padre privado ema-ecosistema, con instructor de IA "Sargento Echo".
Repos y estado:
- flujo-handoff-SSOT-externo-repositorio (público, método de handoff): main = 80d28af (HANDOFF Rev 7, METODO P-02 v2, INCIDENCIAS I-09), publicado.
- ingles-conversacional (privado): main = 2ac35a4 (HANDOFF Rev 2), publicado.
- ema-ecosistema (padre, privado): remotos origin y local-bare. El marco EMA vive al lado de cada repo hijo y no lo contamina (.ema_ecosistema en su .gitignore).
Fuentes: usuario de GitHub Miguelepst; no hay memoria de Claude activada.

## OBJETIVO ACTUAL
Cerrar la v1.2 de las reglas de Echo y registrar la primera evidencia real del proyecto de inglés, en chats cortos de un solo paso.

## ESTADO
- ingles-conversacional, commits publicados: 90b5dd5 .gitattributes (LF), d1569b7 .gitignore, c8077cf HANDOFF Rev 1, 6c2c477 INSTRUCCIONES v1, 19f3a1d PRUEBAS v1, 0d5f6f0 INSTRUCCIONES v1.1, 1c7b99d README, 2ac35a4 HANDOFF Rev 2.
- Padre: submódulos registrados en commits 0ef2fa9 (proyecto 10) y 1206d68 (inglés); último puntero 365f33a (apunta a 2ac35a4). Sin publicar: verificar con git status -sb (mis cuentas: unos 8 commits por delante; antes dije 6 y 7 y estaba contando mal). Hay cambios ajenos en rojo (01_IDEAS.md, BOVEDA.md x2, comandos.md, k.md, submódulo 10 con commits nuevos en ci-prueba, carpetas EMA sin seguimiento): no tocar.
- flujo-handoff: el bloque de arranque v2 copiado desde el campo Instructions corrió sin error. Sigue abierta la verificación en un chat nuevo (cierra I-07). Su siguiente acción oficial sigue siendo la pieza 2 (botón).
- Prueba de Echo en un proyecto de claude.ai (plan gratuito): pasó 6 de 6 comprobaciones. Leyó el HANDOFF Rev 2 y PRUEBAS.md, se negó dos veces a ascender, corrigió con el formato pedido y dijo que no evalúa voz.
- Fallos observados en Echo: inventó "2 minutos restantes"; estimó un nivel ("early A2") fuera de simulacro; marcó como error "practice with my guitar", que es válido (se corrigió al ser desafiado).
- Dato del motor: las marcas de hora de los mensajes le llegan a Echo como nota del sistema. Es dato informado por Echo, no visto en pantalla. El formulario de crear proyecto tiene tres campos; Instructions es un solo campo editable; no hay opción de estilo.
- Fuentes de PRUEBAS: CEFR leído en el sitio del Consejo de Europa. ACTFL solo en resúmenes universitarios. Sin verificar: CEFR Companion Volume 2020, correspondencia ACTFL–CEFR y los exámenes externos.

## DECISIONES VIGENTES
- SSOT = HANDOFF en Git; la copia en Context se re-sube tras cada cambio.
- Chats cortos: un paso por chat; el hilo vive en este archivo, no en el chat.
- Ramas: no se usan en ingles-conversacional (commits atómicos a main). En flujo-handoff sí hay rama por pieza.
- Cada archivo, un commit; después, un commit solo del puntero en el padre.
- Ritual de edición: lectura, edición, verificación (numstat, @@, --check, bytes CR, marcadores, ls-files --eol), commit.
- ingles-conversacional: repo privado; audios fuera de Git; LF por .gitattributes; commits con emoji tras los dos puntos.
- Proyecto de inglés: mínimo 5 min diarios; rangos Recluta→Comandante ligados a CEFR A1–C2; ascenso con dos simulacros aprobados en sesiones distintas con 7 días de diferencia; criterios observables; umbrales marcados "(propuesta)"; el tono de Echo no suaviza la nota.
- Regla de tiempo (v1.2): del tiempo solo se afirma lo que se lee en la conversación; no se estima tiempo activo. El temporizador de misión queda para una versión posterior, porque las pausas lo falsean.
- Regla de cierre: cada misión deja una línea para PROGRESO.md; el HANDOFF solo cambia con rango, nivel, deudas o siguiente acción.

## RESTRICCIONES
- Plan gratuito: chats cortos, archivos pequeños. Este archivo y el anexo deben mantenerse breves.
- Leer cada bloque antes de ejecutarlo. El asistente no ve mi terminal: pego las salidas.
- Repo público (flujo-handoff): sin rutas locales ni secretos. Repo de inglés: sin datos de terceros.
- No fiarse de cifras esperadas del asistente: se contrastan con la salida real.

## DEUDAS / PENDIENTES
1. Aplicar INSTRUCCIONES v1.2 (ANEXO A) y PRUEBAS v1.1 (ANEXO B), con un commit por archivo y puntero en el padre. Después, actualizar ambos en el proyecto de claude.ai.
2. Registrar en el README la fila de Claude y decidir si el perfil de motores vive allí o en docs/MOTORES.md (ANEXO C).
3. Crear docs/PROGRESO.md con la primera entrada (ANEXO D) y subir el HANDOFF a Rev 3.
4. Test de ubicación gratuito, audio base de 2 minutos, tema fijo de la grabación mensual y registrar el resultado externo "B1" que Miguel dice haber obtenido (nombre, enlace, fecha, habilidades).
5. Práctica de git add -p en una rama de prueba (no consta si se creó practica/add-p). Escenario: separar formato y contenido en un diff mezclado.
6. Decidir dónde vive este HANDOFF (propuesta: repo padre privado; no en el repo público).
7. Pendiente de flujo-handoff: verificar el bloque v2 en un arranque real y cerrar I-07; pieza 2.
8. Publicar el padre cuando yo lo decida (arrastra commits de otros proyectos).
9. Opcional: chat aparte para que me expliquen el sistema de handoff parte por parte, y plantilla mínima para otros usos (bootcamp, Android).

## SIGUIENTE ACCIÓN
Aplicar el punto 1 en un chat nuevo: editar INSTRUCCIONES v1.2 con el ANEXO A, verificar y commitear solo ese archivo. Un paso por chat.

## APRENDIZAJES DEL MÉTODO
- Un solo @@ no es la meta. Con -U0 los hunks cercanos no se fusionan; el texto tras @@ es contexto.
- Pegar sin salto de línea final borra la línea en blanco siguiente; copiar de más duplica viñetas.
- Los errores recurrentes del asistente fueron de expectativa (cifras mal calculadas), no de ejecución: contrastar con la salida real.
- Una corrección de IA que suene rara se desafía y se verifica en un diccionario o corpus.
