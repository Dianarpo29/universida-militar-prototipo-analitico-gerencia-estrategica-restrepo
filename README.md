## Contenido para Copiar y Pegar (Fila 2)

### **Columna A: Causa**
> Estrategia de despliegue abrupta (Migración sin fases que retiró el acceso a las secretarias sin un periodo de transición de roles).

### **Columna B: Fase DT origen (E/D/I)**
> D (Definir)

### **Columna C: Insight de empatía**
> Las secretarias sienten frustración al perder el control de un proceso que dominaban, mientras que los vicepresidentes experimentan sobrecarga operativa y demoras al gestionar Tikelia directamente sin preparación previa.

### **Columna D: Supuesto central**
> Implementar un modelo de despliegue por fases (donde las secretarias co-asistan transitoriamente a los usuarios en las primeras legalizaciones) estabilizará el proceso más rápido que la migración abrupta actual.  
*(Corrige el punto 1: El supuesto ahora responde directamente a solucionar la causa raíz de la falta de fases).*

### **Columna E: Pregunta analítica**
> ¿Existe una diferencia estadísticamente significativa en el tiempo promedio de legalización de gastos entre las áreas con despliegue por fases asistido y aquellas con migración abrupta?

### **Columna F: Variables (nombres exactos)**
> `tiempo_legalizacion_dias`, `modelo_despliegue`, `volumen_gastos_mes`, `vicepresidencia_id`  
*(Corrige el punto 2: Todas las variables se listan juntas horizontalmente dentro de esta celda).*

### **Columna G: Tipo (Outcome / Explic / Control / Segmento)**
> `tiempo_legalizacion_dias` (Outcome)  
> `modelo_despliegue` (Explicativa)  
> `volumen_gastos_mes` (Control)  
> `vicepresidencia_id` (Segmento)  
*(Corrige el punto 3: Clasifica estrictamente cada variable dentro de la misma celda usando saltos de línea).*

### **Columna H: Cálculo / Transformación**
> `tiempo_legalizacion_dias`: Fecha de aprobación final de la legalización menos Fecha de emisión del gasto.  
> `modelo_despliegue`: Categórica [0 = Abrupto, 1 = Por Fases].  
> `volumen_gastos_mes`: Conteo total de facturas cargadas por usuario en el mes.

### **Columna I: Métrica (nombre + fórmula)**
> Tiempo Promedio de Legalización (TPL). Fórmula: Sumatoria de días transcurridos de todas las solicitudes / Número total de solicitudes de legalizaciones en el mes.

### **Columna J: Periodo / Segmento**
> Primeros 30 días calendario posteriores a la fecha de corte de la migración, segmentado por las Vicepresidencias seleccionadas para el piloto.

### **Columna K: Patrón esperado (si cierta)**
> Reducción del >= 25% en el Tiempo Promedio de Legalización (`tiempo_legalizacion_dias`) en las áreas con despliegue por fases comparado con el grupo de migración abrupta al cabo de 30 días.  
*(Corrige el punto 4: Establece una meta numérica de negocio explícita).*

### **Columna L: Condición refutación**
> Si la reducción del Tiempo Promedio de Legalización en el grupo de fases es <= 5% en comparación con el grupo abrupto al finalizar la semana 4.  
*(Corrige el punto 5: Elimina el párrafo cualitativo por un umbral matemático e innegociable).*

### **Columna M: Valor esperado para usuario/ciudadano**
> Disminución de la carga administrativa para los vicepresidentes y mitigación de la fricción tecnológica en la adopción de la plataforma Tikelia.

### **Columna N: Riesgo si falsa**
> Costo hundido en horas de co-asistencia de secretarias y retraso innecesario en la obligatoriedad total del autoservicio en la plataforma.

### **Columna O: Acción si confirma**
> Escalar el modelo de despliegue por fases asistido a todas las demás vicepresidencias y gerencias de la compañía pendientes por migrar.

### **Columna P: Acción si refuta**
> Suspender de inmediato la estrategia de fases asistidas, unificar a toda la organización en migración directa (abrupta) y reorientar los recursos a mesas de soporte técnico en vivo (Help Desk).

---
