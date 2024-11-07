
# Mapa Mental: YAML (YAML Ain't Markup Language)

## Estructura Básica
- Formato de texto
- Legible para humanos
- Indentación sensible
- Uso de espacios, no tabulaciones

## Elementos de Datos
### Escalares
- Cadenas de texto
  - Comillas simples
  - Comillas dobles
  - Sin comillas
- Números
  - Enteros
  - Flotantes
- Booleanos
  - `true`
  - `false`
- Nulos
  - `null`
  - `~`
### Estructuras
- Listas
  - Enumeradas con `-`
- Mapas
  - Pares clave-valor

## Caracteres Especiales
- Comentarios
  - `#`
- Separadores
  - `---` (inicio de documento)
  - `...` (fin de documento)

## Referencias y Anclas
- Anclas (`&`)
- Referencias (`*`)

## Tipos de Datos Personalizados
- Etiquetas (tags)
- `!str`, `!int`, `!float`, etc.

## Multilínea
- Cadena literal (`|`)
- Cadena plegada (`>`)

## Uso Común
- Archivos de configuración
  - Aplicaciones web
  - Herramientas de desarrollo
- Automatización y orquestación
  - Ansible
  - Kubernetes
- Serialización de datos
  - Intercambio de datos entre aplicaciones

## Ventajas
- Legibilidad
- Simplicidad
- Flexibilidad

## Desventajas
- Sensibilidad a la indentación
- No tan popular como JSON o XML en ciertos contextos

## Ejemplo de YAML
```yaml
# Este es un ejemplo de un archivo YAML
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
