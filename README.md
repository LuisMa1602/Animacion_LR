# Simulación de Parsing LR(1)

Este proyecto muestra una simulación del análisis sintáctico **LR(1)** utilizando **HTML, CSS y JavaScript**.

## 📌 Descripción
El programa permite visualizar de forma animada cómo funciona un analizador LR(1).  
Se incluyen dos ejemplos básicos de gramáticas y sus correspondientes tablas LR(1).  
La animación muestra en cada paso el contenido de la **pila**, la **entrada restante** y la **acción realizada**.

## 🚀 Tecnologías utilizadas
- **HTML** → estructura de la página.
- **JavaScript** → lógica de la animación paso a paso.

## 📂 Estructura del proyecto
- `index.html` → Contiene la implementación principal con las tablas y la animación.
## ▶️ Ejecución
1. Clona este repositorio en tu máquina local:
   ```bash
   git clone https://github.com/LuisMa1602/Animacion_LR
   ```
2. Abre el archivo `index.html` en tu navegador.
3. Haz clic en los botones **Iniciar Animación** para observar el proceso paso a paso.

## 📖 Ejemplo de salida
Ejemplo 1 (entrada `a+b$`):
```
Pila: $0 | Entrada: a+b$ | Salida: d2
Pila: $0a2 | Entrada: +b$ | Salida: d3
Pila: $0a2+3 | Entrada: b$ | Salida: d4
Pila: $0a2+3b4 | Entrada: $ | Salida: r1 E→id+id
Pila: $0E1 | Entrada: $ | Salida: acept
```

Ejemplo 2 (entrada `a$`):
```
Pila: $0 | Entrada: a$ | Salida: d2
Pila: $0a2 | Entrada: $ | Salida: r1 E→id
Pila: $0E1 | Entrada: $ | Salida: aceptación
```

## ✅ Conclusión
Este proyecto es una herramienta educativa para comprender cómo funcionan los analizadores **LR(1)**.  
La implementación modular en JavaScript facilita la extensión a más gramáticas y ejemplos.
