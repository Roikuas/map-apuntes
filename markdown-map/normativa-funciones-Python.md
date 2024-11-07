
# Mapa Mental: Normativas, Buenas Prácticas y Profesionalismo en el Uso de Funciones en Python

## 1. Normativas

### 1.1 PEP 8
- **Propósito**: Guía de estilo para el código Python.
- **Reglas Clave**:
  - Uso de 4 espacios por nivel de indentación.
  - Líneas no deben exceder 79 caracteres.
  - Espacios alrededor de operadores y después de comas.
  - Uso de comillas simples o dobles para cadenas, pero consistente en todo el código.
  - Nombres de funciones en minúsculas y con guiones bajos (snake_case).

### 1.2 Documentación
- **Docstrings**:
  - Describir la función y sus parámetros.
  - Uso de triple comillas dobles """.
  - Módulos como Sphinx o pdoc para generar documentación automática.

## 2. Buenas Prácticas

### 2.1 Nombres Claros y Descriptivos
- **Funciones**:
  - Nombres que describan claramente la acción realizada.
  - Evitar abreviaturas y nombres vagos.

### 2.2 Parámetros y Retornos
- **Parámetros**:
  - Usar nombres descriptivos.
  - Orden lógico (de lo más general a lo más específico).
- **Retornos**:
  - Documentar claramente qué retorna la función.
  - Utilizar tuplas o diccionarios para múltiples valores.

### 2.3 Modularidad y Reutilización
- **Funciones Pequeñas y Específicas**:
  - Cada función debe realizar una única tarea.
  - Facilita la prueba y el mantenimiento.
- **Reutilización**:
  - Evitar duplicar código.
  - Crear funciones reutilizables.

### 2.4 Manejo de Errores
- **Try/Except**:
  - Capturar excepciones específicas.
  - Proveer mensajes de error claros.
- **Validación de Entradas**:
  - Asegurarse de que los parámetros sean del tipo esperado.

## 3. Profesionalismo

### 3.1 Pruebas Unitarias
- **Propósito**:
  - Verificar que las funciones se comporten según lo esperado.
- **Frameworks**:
  - Uso de `unittest` o `pytest`.
  - Crear pruebas para casos bordes y entradas inválidas.

### 3.2 Control de Versiones
- **Git**:
  - Comentar cambios en el código.
  - Uso de ramas para desarrollar nuevas funciones.
  - Revisiones de código antes de hacer merges.

### 3.3 Code Reviews
- **Revisiones de Código**:
  - Realizar revisiones periódicas del código de los compañeros.
  - Dar y recibir feedback constructivo.

### 3.4 Actualización Continua
- **Aprendizaje Continuo**:
  - Mantenerse actualizado con las nuevas versiones de Python.
  - Participar en la comunidad (foros, conferencias, meetups).

### 3.5 Ética Profesional
- **Código Limpio y Eficiente**:
  - Priorizar la legibilidad y eficiencia del código.
  - Evitar prácticas deshonestas como el plagio de código.
