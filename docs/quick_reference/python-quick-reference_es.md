## LO BÁSICO


### Print

**Descripción:** 
Imprime una cadena de texto (*text string ó string*) en la consola. 

**Sintaxis:** 
```python title="La función de print"
print("Hola Mundo")
```
***
### Input

**Descripción:** 
Imprime una cadena de texto (*`string`*) en la consola y le pide al usuario entrar una cadena de texto 
(*`string`*)

**Sintaxis:** 

```python title="La función de input"
input("¿Cuál es tu nombre?")
```
:notepad_spiral:**Notas:** 
Luego de entrar una cadena de texto (*`string`*) el usuario deberá presionar la tecla de ++enter++ para almacenar la cadena de texto (*`string`*) en memoria. 
***
### Comentarios

**Descripción:** 

1. **Comentarios sencillos (una línea):**

:pushpin: ==Los comentarios de una línea empiezan con el caracter ```#```.== 
Para crear una comentario, añadimos un caracter de ```#``` antes de la línea que queremos comentar. Los comentarios son ignorados por el `interpretador` de ***Python*** :snake:  y no se ejecutan.  

:pushpin: Los comentarios se pueden usar como herramienta para encontrar errores o probrar alternativas de implementación en nuestros programas. 

<!-- 
Cuando queremos probar si una línea de código esta causando un error o, queremos probar otra forma de implementar el código, convertimos la línea en un comentario para ver que cambios ocurren en la ejecución del programa.
-->

**Sintaxis:** 
```python title="Comentarios en línea"
#Esta línea es un comentario
print("Esto es código")
```
2. **Comentarios en bloques:**
Añade 3 comillas sencillas `'''`antes de la primera línea de código que quieres comentar y otras 3 comillas sencillas `'''` después de las última línea de código que quieras comentar. 

**Sintaxis:** 
```python title="Comentarios en bloque" 
'''
Esta línea es un comentario
y esta también... 
Al igual que esta
y aquí termina el comentario. La próxima línea también es ignorada: 
print("Esto fue un comentario en bloque")
'''
print("Esto es código")
```
***

### Declarar variables

**Descripción:** 
Las variables son objetos que residen en la memoría de la computadora. Esos objetos pueden ser cadenas de texto (*`strings`*) números enteros (*`integers`*), números con parte decimal (*`floating numbers`*) y otros. 
Imagina las variables como una caja y dentro de la caja hay una pieza de información. La caja tiene una etiqueta que nos dice como llamar esa caja. Cada variable debe tener un nombre único que no se debe repetir en todo el programa. A ese nombre se le  llama `identificador`  (*`variable identifier`*)

**Sintaxis:** 
```python title="Declarando variables"
mi_nombre = "Pepo" #variable de tipo string
mi_edad = 13 #variable de tipo int
dias = 365.25 #variable de tipo float
```
***

### El Operador +=

**Descripción:** 
Es una forma muy conveniente de decir "Toma el valor anterior y añadele (o súmale)"

**Sintaxis:** 
```python title="El operador +="
mi_edad = 13
mi_edad += 4
# Ahora la variable mi edad tiene un valor de 17
```
**Ejemplo:** 
```python title="El operador +=" hl_lines="3"
mi_edad = 13
print(mi_edad)
mi_edad += 4
print(mi_edad)
```
***

## TIPOS DE DATOS (*`DATA TYPES`*)


***
### Integers (*`int`*)

**Descripción:** 
Los integrales (*`integers`*) son números enteros (sin parte decimal)

**Sintaxis:** 
```python
cantidad_de_dias = 365
```
***

### Floating Point Numbers (*`float`*)

**Descripción:** 
Los números con coma flotante (*`float`*) son números con parte decimal. Cuando calculas una división y el resultado es una fracción ese resultado tendrá un tipo de dato (*`float`*)

**Sintaxis:** 
```python
cantidad_de_dias_exactos = 365.25
```
### Concatenar una cadena de texto (*`String concatenation`*)

**Descripción:** 
[Concatenar significa unir](https://dle.rae.es/concatenar "Haz clic para leer la definición de la palabra  'concatenar' en el Diccionaro de la Real Academia Española."). En el caso de cadenas de texto (*`strings`*) quiere decir que puedes unir 2 o más cadenas de texto (*`strings`*) y el resultado será una cadena de texto (*`string`*)
nueva. 
 
**Sintaxis:** 
```python
"Hola" + "Mundo" 
#Se convierte en HolaMundo
```
**Ejemplos:** 

1.`Concatenando` 2 cadenas de texto `strings` **sin dejar espacios entre las palabras.** 
```python hl_lines="4"
# Concatenando 2 strings. El resultado no tiene espacio entre las 2 palabras. 
string1 = "Hola"
string2 = "Mundo"
print(string1+string2) 
```

2.`Concatenando` 2  `strings` **dejando un espacio entre las palabras**. 
```python hl_lines="4"
# Concatenando 2 strings. El resultado TIENE un espacio entre las 2 palabras. 
string1 = "Hola"
string2 = "Mundo"
print(string1+" "+string2) #El espacio lo crean las " "
```
***
### Escapando de una cadena de texto (*`Escaping a string`*)

**Descripción:** 
Hay veces que mientras programamos necesitamos incluir en nuestros `strings` algún caracter que está reservado para uso especial en ***Python*** :snake: 

  Un ejemplo de esto lo son las ***" "*** que se usan para indicarle a ***Python*** :snake: cuál es el texto que se va a imprimir (usando la función de `print`) en pantalla. Para esos casos usamos un caracter que rompe la secuencia de la instrucción y nos permite incluir los caracteres especiales sin dañar el mensaje escrito. El caracter es **`\`** 

**Sintaxis:** 
```python hl_lines="1"
dialogo = "Ella dijo: \"Hola\""
print(dialogo)
#prints: Ella dijo: "Hola"
```
***
### F-Strings 

:spiral_notepad: **(Calma...la "F" 😌 es de `Formatting`)**

**Descripción:** 
En ***Python*** :snake: puedes incluir variables dentro de cadenas de texto (*`strings`*). Dentro de un `string` usamos los corchetes `{ }` para  indicar en que posición deber ir la variable. Cuando se imprime el texto en la consola, el contenido de la variable sustituye las `{ }`

**Sintaxis:** 
```python hl_lines="2"
total_de_dias = 365
print(f"Hay un total de {total_de_dias} en un año.")
```
**Ejemplos:** 
```python hl_lines="3-5"
bolsas = 3
mangos_por_bolsa = 12
print(f"Hay {bolsas} bolsas con mangos")
print(f"En cada bolsa hay {mangos_por_bolsa} mangos")
print(f'Para un total de {bolsas * mangos_por_bolsa} mangos')
```
***
### Conversión entre `Data types`

**Descripción:** 
En ***Python*** :snake: es posible cambiar el `Data Type` de un pedazo de información o de un dato en particular. Por ejemplo un número puede cambiar de `int` a `float` y vice versa. 

|  Función  | Acción                                              |
|:---------:|-----------------------------------------------------|
| `int()`   | Convierte la variable a un número entero            |
| `float()` | Convierte la variable a un número con parte decimal |
| `str()`   | Convierte la variable a un `string`                 |

**Sintaxis:** 
```python 
cantidad_dias = 365
editar_cantidad_dias = float(cantidad_dias)
```
```python 
cantidad_dias = 365.25
editar_cantidad_dias = int(cantidad_dias)
```
```python 
cantidad_dias = 365.25
editar_cantidad_dias = str(cantidad_dias)
```

**Ejemplos:** 

1. Conversión de `int` a `float` 
```python hl_lines="2"
cantidad_dias = 365
editar_cantidad_dias = float(cantidad_dias)
print(editar_cantidad_dias) #El resultado será 365.0.
```
2. Conversión de `float` a `int` 
```python hl_lines="2"
cantidad_dias = 365.0
editar_cantidad_dias = int(cantidad_dias)
print(editar_cantidad_dias) #El resultado será 365
```
***
### Verificando el `Data type`

**Descripción:** 
  Para verificar cuál es el `Data type` de una variable en particular usamos la función `type`

**Sintaxis:** 
```python 
pi = 3.14159
type(pi) #El resultado será <class 'float'>
```
**Ejemplos:** 

  1. Validando un `int`
```python  hl_lines="2"
pi = 3.14159
print(type(pi)) #El resultado será  <class 'float'>
```
  2. Validando un `float`
```python hl_lines="2"
pi = 3
print(type(pi)) #El resultado será  <class 'int'>
```
  3. Validando un `str`
```python  hl_lines="2"
pi = "Tres"
print(type(pi)) #El resultado será  <class 'str'>
```
***

## MATEMÁTICAS


En ***Python*** :snake: puedes hacer operaciones matemáticas usando los ***operadores matemáticos*** básicos. 
  
### Suma
**Expresión:** (3 + 4)

**Sintaxis:** 
```python
suma = num1 + num2 
```
```python
suma = 3 + 4 
```
### Resta
**Expresión:** (3 - 4)

**Sintaxis:** 
```python
resta = num1 - num2 
```
```python
resta = 3 - 4 
```
### Multiplicación 
**Expresión:** (3 * 4)

**Sintaxis:** 
```python
multiplicacion = num1 * num2 
```
```python
multiplicacion = 3 * 4
```
### División 
**Expresión:** ($^3/_4$)

**Sintaxis:** 
```python
division = num1 / num2 
```
```python
division = 3 / 4
```
### Exponentes
**Expresión:** ($3^4$)

**Sintaxis:** 
```python
exponente = num1 ** num2 
```
```python
exponente = 3 ** 4 
```

### El Operador +=

**Descripción:** 
Es una forma muy conveniente de decir, "Toma el valor anterior y añadele (o súmale)."

**Sintaxis:** 
```python
mi_edad = 13
mi_edad += 4
# Ahora la variable mi edad tiene un valor de 17
```
**Ejemplo:** 
```python hl_lines="3"
mi_edad = 13
print(mi_edad)
mi_edad += 4
print(mi_edad)
```

:spiral_notepad: ***Notas:*** 

1. También lo puedes usar con el Operador de Resta. Entonces estarías diciendo, "Al valor anterior restale."
>```python
>mi_edad -= 4
>```
>**Ejemplo:** 
>```python hl_lines="3"
>mi_edad = 13
>print(mi_edad)
>mi_edad -= 4
>print(mi_edad)
>```

2. Y con el Operador de Multiplicación
>```python
>mi_edad *= 4
>```
>**Ejemplo:** 
>```python hl_lines="3"
>mi_edad = 13
>print(mi_edad)
>mi_edad *= 4
>print(mi_edad)
>```
***

### El Operador Módulo

**Descripción:** 
Hay situaciones en las que necesitamos conocer el residuo que queda luego de una operación de división, por ejemplo: 
>`4 ÷ 2 = 2` tiene un residuo de 0
> pero, `5 ÷ 2 = 2` tiene un residuo de 1.

El Operador de `Módulo` no devuelve el resultado de la división, solamente el residuo. 
El `Módulo` puede ser muy útil en situaciones como por ejemplo, determinar si un número es par o es impar.  

**Sintaxis:** 
```python
modulo = 3 % 4 
#El resultado es 1
```
**Ejemplo:**
```python hl_lines="3"
num1 = float(input("Favor de entrar un número: "))

residuo = num1 % 2
if residuo > 0:
    print("El número entrado es IMPAR.")
else:
    print("El número entrado es PAR.")
```
***
## FUNCIONES


**Descripción:** 
Las funciones en ***Python*** :snake: (y en cualquier otro lenguaje de programación) cumplen 2 propósitos: 

  * Organizar el código para que sea más fácil de leer y comprender
    
  * Organizar el código en unidades que se puedan utilizar más de una vez. 

### Cómo crear una función 

Cuando definimos una función hacemos que el programa sea más fácil de leer. Para definir una función empezamos usando el comando `def`. Luego del comando `def` viene el nombre la función. 

>##### :pushpin:***Cómo nombrar funciones***
>Las mismas reglas que se usan para los nombres de las variables aplican para los nombres de las funciones. 

**Sintaxis:** 
```python 
def nombre_de_la_funcion(lista_de_parametros):
  ...  
  instrucciones
  ...
  return [expresion] 
```


>##### :pushpin:***Cómo escribir funciones*** 
>==Las líneas de código dentro de la función TIENEN que estar indentadas== para que ***Python*** :snake: entienda que son parte del contenido de la función. Para indentar las líneas de código presiona la tecla de ++tab++ antes de comenzar cada línea. 

**Ejemplos:** 

  1. Este ejemplo usa el módulo `turtle`. Creamos la función `dibujar_cuadrado` *(líneas de la 3 a la 11)* para reusar el código que dibuja  un cuadrado.
```python hl_lines="3-11 13 19"
from turtle import *

def dibujar_cuadrado():
  forward(100)
  left(90)
  forward(100)
  left(90)
  forward(100)
  left(90)
  forward(100)
  left(90)

dibujar_cuadrado()

rt(90)
penup()
fd(25)
pendown()
dibujar_cuadrado()
```


Luego la [invocamos](https://dle.rae.es/invocar "Haz clic para leer la definición de la palabra  'invocar' en el Diccionaro de la Real Academia Española.") (*en las líneas 13 y 19*). Ahora se pueden crear cuadrados con solo llamar o ***invocar*** la función por su nombre;  `dibujar_cuadrado()`


### Cómo llamar una función

>Llamamos una función usando su nombre. Esto lo hacemos
escribiendo el nombre de la función (según se escribio en la declaración) seguido por un par de paréntesis ```()```.


**Sintaxis:** 
```python
dibujar_cuadrado()
```
<!--python title="Cómo invocar una función" hl_lines="5" -->
**Ejemplos:** 

```{.py3 title=" :material-file-code: My Cool Header"} 

right(90)
penup()
forward(25)
pendown()
dibujar_cuadrado()
```

***

## CONDICIONALES

## RECURSIÓN (*`LOOPS`*)

## LISTAS (*`LIST METHODS`*)

## FUNCIONES ESTÁNDAR

## MÓDULOS

## CLASES & OBJETOS (*`OOP`*)

Las clases y los objetos son parte del paradigma de programación conocido cómo OOP, Object Oriented Programming. 

## MENSAJES DE ERROR

<!---------- Abbreviations ----------> 
*[OOP]: Object Oriented Programming o Programación Orientada a Objetos


<!---------- Template ---------->
<!--
***
### Título de la sección

##### Título de la sub-sección

**Descripción:** 
Texto que describe una función de  ***Python*** :snake: 

**Sintaxis:** 
```python title="titulo del código aquí" hl_lines="1"
#El código va aquí
```

**Ejemplos:** 

```python title="titulo del código aquí" hl_lines="1"
#El código va aquí
```

***
-->