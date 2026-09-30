# Bitacora de tecnicas avanzadas
Laboratorio 07: Tecnicas Avanzadas de Prompting.
Herramienta de IA usada: ChatGPT

## Ejercicio 2: Zero-shot, one-shot y few-shot

| Tipo | Aciertos (de 5) | Formato de la respuesta | Todas con el mismo formato (Si/No) |
|------|-----------------|-------------------------|------------------------------------|
| Zero-shot | 5 | Tabla con emojis e introducción | No |
| One-shot | 5 | Lista enumerada con categoría primero | No |
| Few-shot | 5 | "Comentario" -> Etiqueta directa | Sí |

### Observaciones
El método few-shot permite mantener un formato homogéneo y estricto, ideal para automatizaciones o exportación de datos.

## Ejercicio 3: Chain of Thought

| Pedido | Respuesta de la IA | Muestra los pasos (Si/No) | Correcta (Si/No) |
|--------|--------------------|---------------------------|------------------|
| Directo | 318.6 | No | Sí |
| Paso a paso | Muestra el cálculo del descuento (S/ 90), IGV (S/ 106.20) y total de 3 unidades (S/ 318.60) | Sí | Sí |

### Explicación
Pedir a la IA que resuelva paso a paso (Chain of Thought) nos ayuda a auditar cada cálculo y evitar errores matemáticos o explicaciones erróneas.

## Ejercicio 4: Role prompting

| Enfoque | Tono de la respuesta | Claridad del ejemplo | Incluye consejo practico (Si/No) |
|---------|----------------------|----------------------|----------------------------------|
| Sin rol | Formal e informativo | Estándar / genérico | No |
| Con rol | Didáctico, cercano y académico | Usa analogías sencillas y paso a paso | Sí |

### Observaciones
Asignar un rol específico (Role Prompting) ajusta el tono, la perspectiva y el nivel de profundidad de las respuestas de la IA, haciéndolas mucho más adecuadas para el público objetivo deseado.

## Ejercicio 5: Descomposicion

| Estrategia | Profundidad del contenido | Control sobre el resultado | Facilidad de revision (Alta/Media/Baja) |
|------------|---------------------------|----------------------------|-----------------------------------------|
| Prompt unico | General / Superficial | Bajo | Media |
| Descompuesto | Detallado y estructurado | Alto | Alta |

### Observaciones
Descomponer una tarea compleja en pasos secuenciales ayuda a que la IA no omita detalles importantes ni acorte las respuestas por límite de contexto. Permite ajustar y corregir cada fase antes de pasar a la siguiente[cite: 1].

## Ejercicio 6: Prompt estructurado y autocritica

| Elemento del prompt | Presente en la respuesta (Si/No) | Calidad de la autocritica (Alta/Media/Baja) |
|---------------------|-----------------------------------|---------------------------------------------|
| Rol asignado | Sí | Alta |
| Componentes clave | Sí | Alta |
| Puntos de falla / Autocrítica | Sí | Alta |

### Observaciones y Conclusión General
* **Prompt estructurado y autocrítica:** Solicitar expresamente a la IA que revise y critique sus propios resultados obliga al modelo a identificar vulnerabilidades o sesgos que de otro modo pasaría por alto.
* **Conclusión del laboratorio:** A lo largo del laboratorio se evidenció cómo técnicas como Few-shot, Chain of Thought y Prompting Estructurado mejoran sustancialmente el control, la precisión y la calidad de las respuestas generadas por los modelos de lenguaje.
