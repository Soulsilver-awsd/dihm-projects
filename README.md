# Taller: Sistema de Monitoreo Meteorológico Inteligente

## Información del Proyecto
- **Asignatura:** Diseño Interfaz Hombre Máquina  
- **Instructor:** MsC. Daniel Quirumbay Y.  
- **Autor:** Paulo Orrala Arriaga  
- **Fecha:** 10/14/2025 
- **Plataforma:** Google Colab  

---

## Actividad 1: Configuración del entorno y estructura base

### Objetivos
- Configurar el entorno de desarrollo en Google Colab
- Instalar las bibliotecas necesarias
- Crear estructura base del proyecto
- Definir dataset de ciudades

### Tareas
1. Abrir Google Colab y crear nuevo notebook
2. Instalar bibliotecas: `requests`, `pandas`, `matplotlib`, `scikit-learn`, `ipywidgets`
3. Implementar clases y funciones base para gestión de datos
4. Definir lista de ciudades con coordenadas geográficas

---

## Actividad 2: Conexión a API pública (Open-Meteo)

### Objetivos
- Establecer conexión con API de Open-Meteo
- Obtener datos meteorológicos en formato JSON
- Transformar y validar datos en DataFrame

### Tareas
1. Identificar endpoint: `https://api.open-meteo.com/v1/forecast`
2. Definir parámetros requeridos: latitude, longitude, hourly, timezone
3. Construir URL de consulta
4. Realizar petición HTTP con `requests.get(url)`
5. Validar respuesta (`status_code == 200`)
6. Cargar JSON en DataFrame con pandas
7. Convertir tipos de datos (fechas y valores numéricos)
8. Visualizar primeros registros con `df.head()`

---

## Actividad 3: Componentes inteligentes (reglas y alertas)

### Objetivos
- Implementar sistema de reglas para análisis meteorológico
- Generar alertas automáticas por condiciones extremas
- Cuantificar frecuencia de alertas

### Tareas
1. Implementar reglas de análisis para:
   - Temperatura
   - Humedad  
   - Velocidad del viento
2. Generar alertas automáticas según umbrales predefinidos
3. Crear columna adicional con cantidad de alertas por hora

---

## Actividad 4: Visualización dinámica

### Objetivos
- Crear visualizaciones interactivas de datos meteorológicos
- Identificar patrones y tendencias
- Presentar información de alertas de manera clara

### Tareas
1. Utilizar matplotlib para graficar:
   - Temperatura vs tiempo
   - Humedad vs tiempo
   - Velocidad del viento vs tiempo
2. Crear gráfico de barras para número de alertas por hora
3. Analizar visualmente patrones de comportamiento

---

## Actividad 5: Interacción con el usuario (ipywidgets)

### Objetivos
- Desarrollar interfaz interactiva para selección de ciudades
- Implementar actualización dinámica de visualizaciones
- Mejorar experiencia de usuario

### Tareas
1. Crear menú desplegable con `ipywidgets.Dropdown()`
2. Implementar funcionalidad de actualización al cambiar ciudad
3. Mostrar resultados dinámicamente en pantalla
4. Sincronizar gráficas con selección del usuario

---

## Actividad 6: API sencilla — Paso a paso detallado

### Objetivos
- Documentar proceso completo de integración con API
- Establecer mejores prácticas para consumo de APIs
- Garantizar calidad y confiabilidad de datos

### Proceso Detallado
1. **Identificación**: API y recurso específico
2. **Parámetros**: Definir latitude, longitude, hourly, timezone
3. **Construcción**: Ensamblar URL correctamente
4. **Petición**: Enviar con `requests.get()`
5. **Verificación**: Validar respuesta (status 200)
6. **Conversión**: Transformar a DataFrame
7. **Limpieza**: Validar y limpiar datos
8. **Persistencia**: Guardar resultados si es necesario

---

## Actividad 7: Predicción simple (Regresión Lineal)

### Objetivos
- Implementar modelo predictivo básico
- Evaluar precisión del modelo
- Visualizar predicciones futuras

### Tareas
1. Utilizar scikit-learn para modelo de regresión lineal
2. Entrenar modelo con serie temporal de temperatura
3. Calcular error MAE (Mean Absolute Error)
4. Graficar predicción de próximas horas
5. Comparar valores reales vs predichos

---

## Actividad 8: Reporte breve

### Objetivos
- Documentar proceso y resultados
- Analizar efectividad del sistema
- Proponer mejoras futuras

### Contenido del Reporte
1. **Descripción de reglas** de componentes inteligentes
2. **Resumen del proceso** de conexión y análisis de API
3. **Capturas de pantalla** de gráficas y predicciones
4. **Propuestas de mejora**:
   - Modelos LSTM para predicción
   - Integración con dashboards web
   - Alertas por notificaciones push
   - Análisis de datos históricos

---

## Entregables Esperados
- Código funcional en Google Colab
- Visualizaciones interactivas
- Sistema de alertas operativo
- Modelo predictivo implementado
- Reporte completo de actividades

## Criterios de Evaluación
- Funcionalidad del código
- Calidad de visualizaciones
- Efectividad de alertas
- Precisión de predicciones
- Documentación y reporte