# Método de la Potencia 🔢  

Repositorio para la implementación y análisis del **método de la potencia** en álgebra lineal computacional.  

## 📌 Objetivo  
Implementar el método de la potencia y analizar su **velocidad de convergencia** mediante simulaciones con matrices aleatorias.  

## 📖 Contenido  

### 🔹 Ejercicio 1: Implementación  
Se desarrolla un programa que recibe una matriz `A ∈ Rⁿˣⁿ` y un entero `k`, aplicando `k` iteraciones del método de la potencia con un vector aleatorio inicial `v ∈ Rⁿ`.  
El resultado es un vector `a ∈ Rᵏ` con las aproximaciones del autovalor en cada iteración.  

**Recomendaciones:**  
- Normalizar el vector en cada paso.  
- Comparar resultados con `np.linalg.eigvals()`.  

### 🔹 Ejercicio 2: Convergencia en matrices aleatorias  
- Se genera una matriz `A ∈ R¹⁰⁰ˣ¹⁰⁰` aleatoria y se aplican `100` iteraciones del método.  
- Se grafica la convergencia de las aproximaciones.  

**Preguntas a responder:**  
- ¿El método converge rápidamente?  
- ¿Cómo influye la relación entre los dos mayores autovalores?  

### 🔹 Ejercicio 3: Matrices Simétricas  
- Se genera `A = ½ (C + Cᵀ)` para obtener una matriz simétrica.  
- Se define `B = A + 500I` y se aplica el método.  
- Se analiza el **error** `ei = |λmax - ai|` y su comportamiento en escala logarítmica.  

**Análisis esperado:**  
- La pendiente de `log(ei)` debe ser aproximadamente `2 log(λ₂ / λ₁)`.  
- Comparar con la función teórica `y(x) = 2 log(λ₂ / λ₁) x + log(e₀)`.  

### 🔹 Ejercicio 4: Variación con `B = A + K·I`  
- Se repite el análisis con `K = 1000, 2000, 5000`.  
- Se estudia por qué la velocidad de convergencia disminuye.  

## 🛠️ Tecnologías  
- **Python** 🐍  
- **NumPy** para cálculos matriciales  
- **Matplotlib** para visualización  

## 🔍 Notas  
- Se utilizan `np.linalg.eigvals()` y `np.linalg.eigh()` para validar resultados.  
- Se recomienda usar `sorted()` para ordenar autovalores.  

📩 **Contribuciones y sugerencias son bienvenidas!** 🚀  
