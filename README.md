# Simulación del Juego Yahtzee - Método de Montecarlo

**Materia:** Simulación  
**Estudiante:** Santiago Sanchez Salazar

Este proyecto implementa un simulador del juego Yahtzee para 2 jugadores utilizando el **Método de Montecarlo**, permitiendo observar el comportamiento de los puntajes y la frecuencia de las jugadas tras múltiples iteraciones.

## Reglas del Juego Implementadas

- 5 dados de 6 caras (distribución uniforme)
- Hasta 3 lanzamientos por turno
- 2 jugadores compitiendo
- Análisis estadístico de los resultados

## Estructura del Notebook

1. **Definición de funciones base** - Generación de números pseudoaleatorios con distribución uniforme
2. **Lógica de puntuación** - Evaluación de jugadas (Yahtzee, Poker, Full House, Trio, Escalera)
3. **Simulación del turno con estrategia** - El jugador conserva los dados repetidos para maximizar puntos
4. **Ejecución de Montecarlo** - Simulación masiva de partidas para obtener datos estadísticos
5. **Visualización de resultados** - Histogramas y estadísticas descriptivas

## Requisitos

```bash
pip install pandas matplotlib
```

## Uso

Ejecuta las celdas del notebook `SanchezSalazar_Santiago_Montecarlo.ipynb` en orden para:

1. Generar lanzamientos de dados
2. Calcular puntuaciones según las categorías del juego
3. Ejecutar la simulación de Montecarlo (configurable con `n_partidas`)
4. Visualizar la distribución de puntajes y estadísticas

## Ejemplo de Resultados

Con 1000 partidas simuladas:
- Puntaje promedio Jugador 1: ~258 puntos
- Puntaje promedio Jugador 2: ~257 puntos
- Total de Yahtzees conseguidos: ~1221
