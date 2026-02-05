# LENGUAJES-DE-PROGRAMACION
# Sistemas de Navegación, Autocompletado y Recomendación

Este repositorio contiene la implementación y el diseño de tres sistemas fundamentales utilizados en aplicaciones modernas:

1. Sistema de navegación de páginas web  
2. Función de autocompletar  
3. Sistema de recomendación de productos  

Cada problema incluye:
- Explicación del diseño
- Estructuras de datos utilizadas
- Métodos principales
- Manejo de casos extremos
- Implementación en Python  

Los diagramas de diseño y flujo se incluyen para facilitar la comprensión del funcionamiento interno de cada sistema.

---

## 📌 Problema 1: Sistema de Navegación de Páginas Web

### 🧠 Descripción
Este sistema simula el comportamiento de un navegador web moderno, permitiendo:
- Cargar páginas
- Retroceder a páginas anteriores
- Avanzar a páginas siguientes

Se utiliza un enfoque basado en **dos pilas (stacks)** para manejar el historial de navegación.

---

### 🧱 Diseño y estructura
- `back_stack`: historial de páginas anteriores  
- `forward_stack`: historial de páginas siguientes  
- `current_page`: página actual  

Este diseño permite un manejo eficiente del historial y replica el comportamiento real de los navegadores.

---

### 🔧 Métodos principales
- `loadPage(url)`: carga una nueva página  
- `goBack()`: retrocede a la página anterior  
- `goForward()`: avanza a la página siguiente  

Se manejan casos extremos como intentar retroceder o avanzar sin historial disponible.

---

### 📐 Diagramas

**Diagrama de flujo – Sistema de navegación**

<img width="806" height="385" alt="image" src="https://github.com/user-attachments/assets/e6468775-9f46-434b-b164-96e2c846b3c4" />


---

### 🧪 Implementación
La implementación completa se encuentra en el archivo correspondiente dentro del repositorio.

---

## 📌 Problema 2: Función de Autocompletar

### 🧠 Descripción
Este sistema implementa una función de autocompletar similar a la de los motores de búsqueda, que dado un prefijo devuelve todas las palabras que comienzan con él.

Para garantizar eficiencia, se utiliza una estructura de datos **Trie (árbol de prefijos)**.

---

### 🧱 Diseño y estructura
Cada nodo del Trie contiene:
- Un diccionario de hijos (`children`)
- Un indicador de fin de palabra (`is_end_of_word`)

Este enfoque permite búsquedas rápidas por prefijo.

---

### 🔧 Métodos principales
- `insert(word)`: inserta una palabra en el Trie  
- `autocomplete(prefix)`: devuelve las palabras que comienzan con el prefijo dado  

---

### 📐 Diagramas

**Diagrama de estructura – Trie**

<img width="580" height="475" alt="image" src="https://github.com/user-attachments/assets/1e8c8d67-4545-49a2-8c88-dbcdb767902b" />


---

### 🧪 Implementación
La implementación en Python se encuentra en el archivo correspondiente del repositorio.

---

## 📌 Problema 3: Sistema de Recomendación de Productos

### 🧠 Descripción
Este sistema recomienda productos a los usuarios basándose en relaciones de compra del tipo:

> “Usuarios que compraron X también compraron Y”

El modelo se basa en un **grafo bipartito Usuario–Producto** y en el conteo de co-ocurrencias.

---

### 🧱 Diseño y estructura
Se utiliza una estructura:
Esto permite:
- Evitar duplicados
- Comparar usuarios fácilmente
- Generar recomendaciones relevantes

---

### 🔧 Métodos principales
- `addPurchase(usuario, producto)`: registra una compra  
- `getRecommendations(usuario)`: devuelve productos recomendados  

Las recomendaciones se ordenan por frecuencia de aparición.

---

### 📐 Diagramas

**Diagrama de relaciones – Usuario / Producto**

<img width="603" height="398" alt="image" src="https://github.com/user-attachments/assets/086e0301-4e75-406f-a737-dae92af82617" />


---

### 🧪 Implementación
La implementación completa del sistema de recomendaciones está disponible en el repositorio.

---

## ⚙️ Tecnologías utilizadas
- Python 3
- Estructuras de datos: listas, pilas, conjuntos, diccionarios
- PlantUML para diagramas

---
