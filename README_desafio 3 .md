# 📚 Desafío 3 — LSTM para generación de texto

Entrega correspondiente al Desafío 3 del curso de PLN. Este proyecto implementa un modelo LSTM para generación carácter por carácter, con control de temperatura y visualización de métricas.

## 📦 Contenido del archivo `Entrega_LSTM_Marisa_Canovas.zip`

- `Desafío 3 LSTM Cánovas.ipynb` — Notebook con todo el desarrollo, entrenamiento, visualización y generación.
- `best_model_lstm.keras` — Modelo entrenado guardado en la época con menor perplejidad.
- `history_ppl.npy` — Historial de perplejidad por época.
- `loss_history.npy` — Historial de pérdida por época.
- `best_epoch.npy` — Índice de la mejor época (mínima PPL).
- `best_ppl.npy` — Valor mínimo de perplejidad alcanzado.
- `grafico_loss_y_perplejidad_lstm.png` — Visualización de métricas de entrenamiento y validación.

## 🧠 Notas técnicas

- Se utilizó `temperature` para controlar la creatividad en la generación.
- El modelo se entrenó con callbacks personalizados para calcular PPL.
- Se implementó guardado automático del mejor modelo y sus métricas.
- El gráfico final muestra la evolución de `loss` y `PPL`, marcando la mejor época.
