# Curso de fundamentos de Python
## Introducción
### ¿Por qué aprender Python?
1. Python ocupa siempre los primeros puestos de los lenguajes mas queridos.
1. Es fácil de aprender.
1. Esta en el top 20 de los lenguajes de programación mejor pagos.
1. Puede ser utilizado en diferentes áreas, especialmente en Análisis de datos (51%) y 1. desarrollo web (45%).
1. Tiene una demanda laboral muy grande en el mundo de la tecnología.

### Tu primer programa en Python

Dentro del entorno encontraremos los archivos con la extensión .py en donde se encuentra nuestro codigo de Python a ejecutar y también encontraremos 2 archivos: poetry.lock y pyproject.toml, en los cuales se encuentran las dependencias del proyecto. En la consola se mostrará la salida o resultado de nuestro programa. Para imprimir utilizamos el comando print:

- **Imprimir un texto:**

print(“Hola mundo!”)

- **Imprimir el calculo de operaciones matematicas:**

```
print(2+20)
print(50-10)
print(3*2)
print(10/5)
```

- **Comentarios:**
Para agregar comentarios que permiten documentar nuestro programa podemos hacerlos de 2 formas:

- Comentario de una sola línea, agregamos un # antes de la línea a comentar

```
# Este es una operación matemática
```

  - Comentario varias lineas, agregamos el comentario entre “”” ó ‘’’

```
“”” comentario mas
Largo ”””
```
```
''' Otro comentario
largo''' 
```

### Variables
Las variables son Espacios de memoria en donde se almacenan un tipo de dato y las cuales se identifican con un nombre, para entender mejor su concepto puede compararse con una caja que almacena un tipo de objetos y que esta marcada con un nombre relacionado a lo que contiene.

Las variables en python se declaran así:
```
nombre_variable = "valor"
```
Las variables pueden ser declaradas, consultadas o modificadas a lo largo de nuestro programa.

Para recibir un dato del usuario podemos usar el comando `input`:
```
input(“¿Cuál es tu nombre?”)
```

Se puede guardar en una variable:
```
nombre = input(“¿Cuál es tu nombre?”)
```

## Tipos de datos en Python
### Tipos de datos
Existen varios tipos de datos en Python, los 3 mas conocidos son:

- String: Cadenas de texto
```
nombreVariable = “texto”
nombreVariable = ‘texto’
```
- Int: números enteros.
```
nombreVariable = 12
```
- Boleanos: Tiene dos estados True(verdadero) ó False(falso).
```
nombreVariable = True
```
> [!NOTE]
> Para saber cual es el tipo de una variable podemos usar la función type(variable) y se puede imprimir usando print().
```
print(type(variable))
```

### Strings
Para declarer una variable tipo string podemos usar “ ” ó ‘ ’.
```
nombre_variable = “texto” 
# Cuando el texto tenga: ‘

nombre_variable = ‘texto’ 
# Cuando el texto tenga: “
```
Podemos unir o concadenar varios String utilizando el operador `+`.
```
nombre = ‘Pepito’
apellido = “ Perez”
nombre_completo = nombre + “ ” + apellido
```
> [!TIP]
> String con formato: Nos permite concatenar de manera fácil y legible nuestro texto con nuestras variables las cuales se colocan entre {}, hay dos formas de hacerlo, pero la segunda es mas legible.

- Primera forma
```
template = "Hola, mi nombre es " + first_name + ", y mi apellido es " + last_name
```
- Segunda forma
```
template = "Hola, mi nombre es {}, y mi apellido es {}".format(first_name, last_name)
```
- Tercera forma
```
template = f"Hola, mi nombre es {first_name}, y mi apellido es {last_name}"
```

### Numbers
Las variables tipo número pueden ser enteras(que no tienen decimales) o flotantes(que tienen decimales), y siempre se declaran sin estar encerradas entre comillas ya que de lo contrario serían de tipo string. 

- **Int:**
```
lives = 3
print(type(lives)) # <class 'int'>
```

- **Float:**
```
temperature = 12.12
print(type(temperature)) # <class 'float'>

```

Las variables numéricas nos permiten realizar cálculos matemáticos y obtener resultados, utilizando operadores matemáticos.

```
lives = 12 + 15
```

Podemos realizar operaciones con la misma variable y para esto tenemos 2 formas de hacerlo, la cual la segunda es la forma simplificada en la cual se utilizan operadores de asignacion.

```
lives = lives - 1
lives -= 1
```

Python nos muestra en notación científica números cuyo valor es muy grande o muy pequeño.

```
number = 4500000000000000000.1
print(number) # 4.5e+18

number_b = 0.0000000000000001
print(number_b) # 1e-16
```
