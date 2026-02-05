# LENGUAJES-DE-PROGRAMACION
# Sistemas de Navegación, Autocompletado y Recomendación

1. Sistema de navegación de páginas web  
2. Función de autocompletar  
3. Sistema de recomendación de productos  

Cada problema incluye:
- Explicación del diseño
- Estructuras de datos utilizadas
- Métodos principales
- Manejo de casos de uso
- Implementación en Python  
---

## Problema 1: Sistema de Navegación de Páginas Web

### Descripción
- Cargar páginas
- Retroceder a páginas anteriores
- Avanzar a páginas siguientes

se uso **dos pilas (stacks)** para manejar el historial de navegación.

---

### Diseño y estructura
- `back_stack`: historial de páginas anteriores  
- `forward_stack`: historial de páginas siguientes  
- `current_page`: página actual  
  (replica el funcionamiento de un navegador)
---

### Métodos principales
- `loadPage(url)`: carga una nueva página  
- `goBack()`: retrocede a la página anterior  
- `goForward()`: avanza a la página siguiente  
se tienen en cuenta casos de uso
---
## Problema 2: Función de Autocompletar

### Descripción
Este sistema implementa una función de autocompletar similar a la de los motores de búsqueda, que dado un prefijo devuelve todas las palabras que comienzan con él.

Para garantizar eficiencia, se utiliza una estructura de datos **Trie (árbol de prefijos)**.

---

### Diseño y estructura
Cada nodo del Trie contiene:
- Un diccionario de hijos (`children`)
- Un indicador de fin de palabra (`is_end_of_word`)

Este enfoque permite búsquedas rápidas por prefijo.

---

### Métodos principales
- `insert(word)`: inserta una palabra en el Trie  
- `autocomplete(prefix)`: devuelve las palabras que comienzan con el prefijo dado  

---

## Problema 3: Sistema de Recomendación de Productos

### Descripción

El modelo se basa en un **grafo bipartito Usuario–Producto** 

---

### Diseño y estructura

- Evitar duplicados
- Comparar usuarios fácilmente
- Generar recomendaciones relevantes

---

### Métodos principales
- `addPurchase(usuario, producto)`: registra una compra  
- `getRecommendations(usuario)`: devuelve productos recomendados  

Las recomendaciones se ordenan por frecuencia de aparición.

