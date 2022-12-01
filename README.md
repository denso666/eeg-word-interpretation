# eeg-word-interpretation-wiht-dl

1. denso666
2. Guminola
3. 

## Circuito EEG
1. Electrodos
2. Preamplificación
3. Eliminar DC
4. Filtro y amplificacion (0 - 3.5/5v) (5Hz/40Hz)

## Lectura en el esp32
1. ADC (interno o externo)
2. Comunicación con pc (matlab/python)

## Preprocesado
> (1 y 2 se pueden empezar con señales simuladas)
1. Filtrado digital
2. Gráfica en tiempo real
3. Registrar las señales reales
4. Extraer frecuencias y armónicos
5. Superponer señales extraídas
6. Observar que señales, regiones  y/o parámetros tienen cambios más significativos
7. Repetir pasos 3 a 6

## Modelo de deep-learning
1. Acondicionar data y etiquetas a un tensor (normalizar)
2. Generar data aumentada
3. Separa data en entrenamiento y testeo
4. Crear modelo categorización binaria (summary)
5. Graficar límite de decisión
6. Graficar curvas de pérdida
7. Graficar matriz de confusión
8. Generar nuevo modelo y compara resultados
9. Repetir pasos 4 a 8
10. Guardar modelo como código c/c++

## Programación c++
1. Cargar modelo a la esp32
2. Generar filtrado digital en c++
3. Función de predicción

### Pendientes
1. Seguridad y eficiencia del circuito
2. Comunicar el esp32 con python o matlab sin arduino
3. Graficar en tiempo real tipo ECG (single time frame)
4. Qué forma tendrá la señal cuando se transforme en tensor
5. Cargar el modelo a la esp32 sin darle en la torre al código para extraer y pre-procesar las señales
6. COMO SE HACE UNA PREDICCIÓN EN TIEMPO REAL CON DATOS CONTINUOS