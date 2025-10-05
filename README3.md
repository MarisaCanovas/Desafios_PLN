Generación de Texto con LSTM: Análisis Comparativo de Estrategias.

Implementación de una red LSTM para generación de texto. El análisis se centra en el impacto de la temperatura (T=0.7 y T=1.2) y la búsqueda Beam Search (k=5) vs. Greedy.

Conclusión clave: La estrategia de Muestreo Estocástico con T=0.7 fue la más efectiva para romper bucles de repetición y lograr un equilibrio entre coherencia y diversidad


1 Entrenamiento_LSTM.ipynb 
Este notebook contiene lo siguiente:

Carga de datos y preprocesamiento.

Creación del vocabulario.

Definición de la arquitectura del modelo (model_lstm).

La celda de entrenamiento (model_lstm.fit(...)).

Las celdas de guardado final (guardado del modelo, métricas, y vocabulario).

2 Analisis_y_Generacion.ipynb

Bloque de Carga/Recuperación: La celda que carga best_model_lstm.keras, history_ppl.npy, char2idx.pkl, etc.

Visualización de Métricas: La celda que genera el gráfico Loss/PPL.

Funciones de Generación: Las funciones generate_stochastic y beam_search_deterministic.

Análisis Comparativo: La celda que genera los cuatro textos (Greedy, Sampling, Beam Search).

Visualización Final: La celda que genera el gráfico analisis_coherencia_final.png.
