
# Mapa Mental: Sintaxis de YAML

## Estructura Básica
- Formato de texto
  - Archivos de texto plano
- Legible para humanos
  - Enfocado en la simplicidad y claridad
- Indentación sensible
  - Uso de espacios, no tabulaciones
  - Indentación consistente

## Elementos de Datos
### Escalares
- Cadenas de texto
  - Sin comillas
    - Ejemplo: `nombre: Juan`
  - Comillas simples (`'`)
    - Ejemplo: `nombre: 'Juan'`
  - Comillas dobles (`"`)
    - Ejemplo: `nombre: "Juan"`
    - Permiten caracteres especiales: `\n`, `\t`, etc.
- Números
  - Enteros: `42`
  - Flotantes: `3.14`
- Booleanos
  - `true`
  - `false`
- Nulos
  - `null`
  - `~`
### Estructuras
- Listas
  - Enumeradas con `-`
  - Ejemplo:
    ```yaml
    frutas:
      - manzana
      - naranja
      - plátano
    ```
- Mapas
  - Pares clave-valor
  - Anidación
  - Ejemplo:
    ```yaml
    persona:
      nombre: Juan
      edad: 30
      dirección:
        calle: "Calle Falsa 123"
        ciudad: "Springfield"
    ```

## Caracteres Especiales
- Comentarios
  - `#` para comentarios
  - Ejemplo: `nombre: Juan # Esto es un comentario`
- Separadores
  - `---` (inicio de documento)
  - `...` (fin de documento)

## Referencias y Anclas
- Anclas (`&`)
  - Permiten definir y etiquetar un nodo
  - Ejemplo:
    ```yaml
    default: &default
      nombre: "Usuario"
      rol: "invitado"
    ```
- Referencias (`*`)
  - Permiten reutilizar un nodo anclado
  - Ejemplo:
    ```yaml
    usuario1: 
      <<: *default
      nombre: "Juan Pérez"
    usuario2: 
      <<: *default
      nombre: "Ana Gómez"
    ```

## Tipos de Datos Personalizados
- Etiquetas (tags)
  - Permiten definir tipos de datos específicos
  - Ejemplos:
    - `!str`: Cadena
    - `!int`: Entero
    - `!float`: Flotante
  - Ejemplo:
    ```yaml
    valor_str: !str "123"
    valor_int: !int "123"
    ```

## Multilínea
- Cadena literal (`|`)
  - Mantiene saltos de línea
  - Ejemplo:
    ```yaml
    descripción: |
      Este es un texto
      con saltos de línea
    ```
- Cadena plegada (`>`)
  - Une líneas en una sola línea con espacios
  - Ejemplo:
    ```yaml
    descripción: >
      Este es un texto
      plegado en una sola línea
    ```

## Uso Común
- Archivos de configuración
  - Aplicaciones web: `config.yaml`
  - Herramientas de desarrollo: `.travis.yml`
- Automatización y orquestación
  - Ansible: `playbook.yml`
  - Kubernetes: `deployment.yml`
- Serialización de datos
  - Intercambio de datos entre aplicaciones: `data.yaml`

## Ventajas
- Legibilidad
  - Formato limpio y claro
- Simplicidad
  - Sintaxis mínima
- Flexibilidad
  - Compatible con múltiples lenguajes y herramientas

## Desventajas
- Sensibilidad a la indentación
  - Errores difíciles de detectar
- Menos popular en ciertos contextos comparado con JSON o XML
  - Menos soporte en algunas herramientas

## Ejemplo de YAML
```yaml
# Este es un ejemplo de un archivo YAML complejo
nombre: Juan Pérez
edad: 30
casado: true
hijos:
  - nombre: Ana
    edad: 10
  - nombre: Luis
    edad: 7
dirección:
  calle: "Calle Falsa 123"
  ciudad: "Springfield"
  país: "USA"
empleo:
  puesto: "Desarrollador"
  empresa: "Tech Solutions"
  duración: 
    años: 5
    meses: 2
