# Clase: Análisis de Sistemas en Lazo y Diagrama de Flujo de Señales
En esta clase se abordó el análisis de sistemas representados por diagramas de bloques y diagramas de flujo de señales. Se analizaron diferentes trayectorias en diagramas complejos, se calcularon funciones de transferencia aplicando la regla de Mason y se redujeron estructuras en lazos. Este tema es fundamental en el estudio de sistemas de control, donde se busca determinar la relación entrada-salida de sistemas lineales.
## 1. Subtítulos

1.1 Definición y utilidad del diagrama de flujo de señales

1.2 Caminos hacia adelante (Paths)

1.3 Lazos individuales y lazos no tocados

1.4 Aplicación de la regla de Mason

1.5 Reducción de sistemas con retroalimentación

## 2. Definiciones
🔑 Camino hacia adelante: Es una ruta desde la entrada a la salida sin pasar dos veces por el mismo nodo.

🔑 Lazo: Cualquier ruta cerrada en el grafo donde se regresa al mismo nodo inicial sin repetir nodos.

🔑 Lazos no tocados: Lazos que no comparten nodos entre sí.

🔑 Determinante de Mason ($\Delta$): Valor que se usa para calcular la función de transferencia total del sistema.

## 9. Ejercicios
📚Ejemplo 1: Cálculo de la función de transferencia con Mason: haga este sistema:

📌 Paso 1: Identificar trayectorias hacia adelante
Analizamos los caminos desde la entrada hasta la salida:

$P_1$: $1 \to 2 \to 3 \to \text{Salida}$

Ganancia: $1 \cdot 1 \cdot (-1) = -1$

$P_2$: $1 \to 3 \to \text{Salida}$

Ganancia: $-14 \cdot (-1) = 14$

📌 Paso 2: Identificar los lazos individuales
Los lazos (loops) cerrados son:

$L_1$: $3 \to 3$ con ganancia: $-1/4$

$L_2$: $1 \to 3 \to 1$ con ganancia: $(-14) \cdot (-0.2) = 2.8$

$L_3$: $1 \to 3 \to 1$ (vía otro camino) con ganancia: $(-0.25)(-0.2) = 0.05$

📌 Paso 3: Identificar lazos no tocantes
No hay lazos que no se crucen entre sí (todos comparten nodos). Entonces:

$\Delta = 1 - (\text{suma de las ganancias de lazos})$

## 10. Conclusiones

La regla de Mason es una herramienta poderosa para calcular la función de transferencia sin necesidad de reducir manualmente los diagramas.

Los lazos no tocados afectan el determinante $\Delta$, permitiendo mejorar la precisión del resultado.

En sistemas de bloques, conocer las configuraciones básicas como serie, paralelo y retroalimentación simplifica los cálculos.

## 11. Referencias

Apuntes de clase: Diagramas de flujo de señales y bloque

Ogata, K. Ingeniería de control moderna

Dorf, R. & Bishop, R. Modern Control Systems


