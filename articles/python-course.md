---
layout: default
title: "Curso de Python - HackingUtils.c"
permalink: /posts/languages/python-course
date: 09-03-2025 
---

Python es un lenguaje de programación de alto nivel y multiparadigma, también es multiplataforma por lo que este es fácilmente usable para múltiples entornos; como lo son el desarrollo de escritorio, el desarrollo web, desarrollo móvil, entre otros.  Es un lenguaje con un tipado dinámico, esto no es un detalle importante por ahora.

Python es multiparadigma ya que soporta parcialmente la programación orientada a objetos, la programación imperativa y la programación funcional. La programación imperativa es la que vamos a aprender primero como paradigma de programacion ya que es la más sencilla de entender y es con la que todos empiezan (aunque muchas veces ni siquiera lo saben); se trata de una forma de programar que sigue un principio simple: “Dale instrucciones al computador línea por línea”. Esto quiere decir que vamos a programar de modo de que cuando la computadora ejecute nuestro código este haga una instrucción a la vez según le vamos indicando. Esto quiere decir que si queremos que sume 2 + 2 y luego lo multiplique por 10, tenemos que tener la linea 1 donde se sumara 2 + 2 y se va a guardar el resultado y luego hacemos la otra operación del multiplicación, así iremos haciendo eso con todo el programa.

Un paradigma de programación es un conjunto de reglas sobre como desarrollar un software, es casi como un manual de instrucciones que te va diciendo que debes de hacer en ciertos casos para mantener una estructura igual en todo tu código. Los paradigmas no se deben considerar dogmas debido a que no son reglas universales y ni tampoco se debe programar sí o sí tal cual dicta un paradigma, si no que son herramientas que, en caso de que nos sea provechoso, podemos usar en nuestro software para mantenerlo estructurado. El paradigma de programación imperativa no es el más eficiente para software grande pero de igual manera encuentra un buen uso a la hora de programar scripts pequeños.

Un script es un programa que da instrucciones a un sistema, generalmente son sumamente pequeños y no son sistemas, pero pueden formar parte de uno, para el paradigma imperativo este es un excelente caso de uso.

El lenguaje de programación Python se usa ampliamente en ciencia de datos, inteligencia artificial, servidores, software como servicio, seguridad y informática, redes, ciber seguridad y muchísimas áreas mas. Por su facilidad de uso y gran alcance es un gran lenguaje por el cual empezar.

## Descargar Python

Para descargar Python debemos a su página web, y entraremos al enlace de descarga para windows (https://www.python.org/downloads/windows/). De este modo, pasaremos a descargar el ejecutable, una vez que lo tengamos, debemos abrirlo y empezar con la instalación de dicho lenguaje de programación. Recalcar, solo estamos descargando el interprete de Python. Un interprete es, para los lenguajes de programación, lo que ejecuta cada instrucción que escribimos; se podría considerar un traductor ya que pasa nuestro código fuente a byte code, este no es interpretado directamente por la CPU o procesador si no que es interpretado por la maquina virtual del interprete, que es por asi decirlo una computadora virtual, además, el interprete detecta errores en tiempo real, este tipo de comportamiento de interprete con maquinas virtuales también lo tiene Java. Hay otra alternativa que es instalar Python desde la Microsoft Store, si luego al seguir el curso usted tiene algún problema relacionado a Python (al ejecutar, por ejemplo), intente con esa alternativa, de lo contrario póngase en contacto con su maestro.

## Entrada y salida

Una vez instalado Python correctamente y entendido su principio de funcionamiento básico podremos pasar a las operaciones básicas. Presionamos la tecla Windows+R y escribimos *cmd*, esto nos abrirá una ventana negra, el cual se le conoce como cmd. Seguido de esto teclearemos Python y daremos enter; ahí se nos va a abrir el interprete de Python, en este interprete podremos escribir nuestras primeras líneas de código.

En una computadora existen dos tipos de operaciones exclusivamente, estas son las operaciones de entrada y salida. Las operaciones de entrada son las mas sencillas de entender, simplemente se refiere a cuando estamos mandándole información a la computadora, esto engloba incluso el simple hecho de dar un click o de usar su teclado, por otro lado, las operaciones de salida se refiere a cuando la computadora nos da información o más bien, *nos presenta un resultado,* con esto quiero decir que cuando imprimimos un documento, vemos una imagen, reproducimos un video o consumimos contenido, estamos haciendo operaciones de salida.

En Python existen dos funciones principales para realizar este tipo de operaciones, para las operaciones de salida tenemos `print()` y para las operaciones de entrada tenemos `input()` . La función `print()` tiene muchísimas formas de usarse y puede personalizarse hasta limites inesperados, pero a grandes rasgos solo lo usaremos para imprimir objetos en la terminal, dichos objetos pueden tener cualquier tipo de dato, `print()` dentro de sus paréntesis debe tener el texto u objeto que queremos imprimir, este puede ser cualquier texto, con la consideración de que debe estar entre comillas, como aquí `print("Hola mundo")` , esto imprime tal cual el texto que pasamos y nada mas; por otro lado, `input()` no necesariamente necesita que le pasemos información, pero si es apropiado agregar un prefijo o indicacion al usuario para que sepa que esperamos que introduzca información: `input("Ingrese su edad: ")` este puede ser un ejemplo de input, lo que hace esta función es pausar todo el programa hasta que el usuario teclea enter, cuando eso pase el programa seguirá su curso normal independientemente de si se introdujo información o no.

## Tipos de datos

Dependiendo del tipo de dato viene su comportamiento, esto quiere decir que no podemos interactuar con los datos de tipo de texto igual que como lo hacemos con los numéricos, ya que su comportamiento y forma de tratarlos es diferente. 

Los tipos de datos basicos de Python son int, string (str), float (flotante o decimal), bool (booleano) y None.

### Explicación por tipo de dato

1. Los tipos de datos int abarcan los números enteros, esto incluye los números negativos, positivos y el cero. Estos se comportan como los números que conocemos de toda la vida. Ejemplos: 0, -1222, 8000, 24
2. Los tipos de datos string, str o cadenas de texto, son como su nombre lo sugiere, texto, en Python esos se representan siempre entre comillas, cada cosa que vean entre comillas dobles o simples se considera de tipo string. Por esta misma razón es que les pasábamos información entre comillas a `print()` e `input()`, como queríamos que imprimiera un texto en el cmd tuvimos que pasarle un string. Ejemplos: ‘a’, “Hola mundo”, ‘Hola mundo’, “”, ‘’
3. Los tipos de datos float o flotantes son un tipo de dato que hace referencia a los números decimales, desde 1.0 hasta cualquier numero con incontables decimales. Se comportan similar a un int, pero con algunos cambios para que el programador pueda tener control sobre los decimales que se le han agregado. Ejemplos: 33.3333, 0.0, -9.4
4. Bool o booleano hace referencia a un tipo de dato que toma el concepto de funcionamiento básico de una computadora. Las computadoras solo tiene dos respuestas posibles, 1 o 0, verdadero o falso y justamente eso son los booleanos, True o False en Python hacen referencia a si una instrucción debe ejecutarse o no, eso lo veremos mas adelante con las condiciones. Son palabras reservadas por lo que donde se vea True o False Python lo interpreta como un bool.
5. None es un tipo de dato nulo, no tiene valor y no se puede interactuar con el como con los demás tipos. Es una palabra reservada también.

## Variables

Las variables son la forma que todos los lenguajes de programación nos dan para guardar información en la RAM de la computadora, esto quiere decir que sus variables solo existen mientras se ejecuta el programa, inmediatamente se cierra el programa su información se desvanece, por lo que no deben usarse variables para guardado de información persistente, porque no es posible. Las variables se guardan en una dirección de memoria.

La estructura para *definir* una variable en Python es simple, consta de un indentificador o nombre y un valor, por lo que la sintaxis es la siguiente: `Indentificador = Valor` 

Entonces, pueden usar el nombre que deseen para sus variables en Python y ademas, pueden guardar cualquier tipo de dato en las mismas. 

```python
mensaje = "Hola mundo"
print(mensaje)
```

En este ejemplo, estoy usando una variable para guardar un mensaje y luego imprimirlo con la función `print()`. ¿De qué tipo de dato viene siendo la variable mensaje?

```python
mensaje = input("Introduzca lo que quiere decir: ")
print(mensaje)
```

Este código usa lo que hemos aprendido hasta ahora para guardar lo que el usuario escribe en una variable, por lo que esto nos abre un mar de posibilidades, debido a que ahora el usuario puede interactuar con nuestro programa y nosotros podremos interpretar las operaciones de entrada. 

Ahora que podemos guardar información, es importante recalcar que el nombre *variable* viene justamente porque es un valor que siempre puede cambiar, en todos los lenguajes los valores de las variables pueden cambiar (a menos que el programador defina que no debe ser así), lo que no puede cambiar es su tipo en los lenguajes de tipado estático, por lo que aprovecharemos la capacidad de Python de cambiar entre tipos de datos para hacer software mas sencillo de entender y mantener.

Además, podemos usar la función `del()` en Python para liberar las direcciones de memoria, en otras palabras *borramos* los datos o variables.

```python
x = 100
x # True
del(x)
x # ERROR
```

## Operadores

Los operadores son como en las matemáticas, aunque hay algunos que directamente son exclusivos del lenguaje, pasemos con los operadores aritméticos primero.

1. `+` o adición: Suma dos valores, ya sea int, float o str. Los tipos de dato a sumar deben ser compatibles, str es compatible consigo mismo, pero int y float son compatibles entre ellos ademas de ser compatibles consigo mismo. `5 + 3`
2. `-` o sustracción: Resta dos valores. Los tipos de dato deben ser int o float. `1 - 1` 
3. `*` o multiplicación: Multiplica dos valores. Los tipos de dato deben ser int o float. `100 * 10` 
4. `/` o división: Divide dos valores. Los tipos de datos deben ser int o float y si intentan dividir `0 / 0` da error automáticamente. `100 / 2.7832`
5. `%` o modulo. Nos da el resto de la división, no su consiente como el operador `/`. `100 % 2.7832` 
6. `**` o potencia: Potencia el primer numero (el de la izquierda, que toma como base) al numero que indique en el segundo lugar (el de la derecha, que toma de numerador). `10**2`
7. `//` división entera: Esta división es lo mismo que la `/` pero se redondea por si misma, haciendo que el resultado siempre sea un entero y no un float. `100 // 2.7832`

Por otro lado, existen los operadores de comparación, estos devuelven booleanos dependiendo si la comparación es cierta o no.

1. `==` es igual a: Este operador indica si un valor x es igual a un valor y. `5 == 3 # False`
2. `!=` es diferente a: Este operador es lo contrario a la igualdad, evalúa la diferencia entre dos valores. `5 != 3 # True`
3. `>, <, =>, <=` Estos operadores son tal cual como en las matemáticas. Mayor que: `5 > 3 # True` , Menor que: `5 < 3 # False` , Mayor o igual `5 => 3 # True` `5 => 5 # False` `5 => 6 # False` , Menor o igual `5 <= 3 # False` `5 <= 5 # True` `5 <= 6 # True`   

Los operadores lógicos son condiciones extras.

1. `and` (Y lógico), es para evaluar que dos o mas operaciones sean verdaderas, si al menos una de todas estas es falsa, devuelve falso, si todas son verdadero, devuelve True. `10 > 3 and 10 <= 15 # True` `10 > 15 and 10 > 20 # False`
2. `or` (O lógico), es para evaluar muchas condiciones tambien, pero en este caso solo con que una sea verdadera ya es suficiente para que devuelva True, por lo que para conseguir un False, todas las condiciones deben ser Falsas. `5 == 0 or 60 < 1 or 1 == 1 # True`
3. `not` (Negación lógica), invierte el valor que conseguimos de las condiciones, es decir, vuelve a True un False y a False un True. `not 5 == 5 # False` 

Los operadores de asignación son operadores que se usan para interactuar sobre variables junto a ciertas operaciones matemáticas.

1. `=` (Asignación), ya lo vimos en la parte de arriba, simplemente signa un valor a un identificador.
2. `+=` (Asignación por adición), suma el valor de la variable al valor que se le pase y hace que la variable sea igual a ese resultado. `x += 5 # La variable va a ser igual 15 luego de la asignacion, suponiendo que su valor original era 10`
3. `-=` (Asignación por sustracción), Lo mismo que con la asignacion por adision pero con resta. `x -= 5 # La variable va a ser igual 5 luego de la asignacion, suponiendo que su valor original era 10`
4. `*=` (Asignación por multiplicación), `x *= 5 # La variable va a ser igual 50 luego de la asignacion, suponiendo que su valor original era 10`
5. `/=` (Asignación por división), `x /= 5 # La variable va a ser igual 2.0 luego de la asignacion, suponiendo que su valor original era 10`
6. `%=` (Asignación por modulo), `x %= 5 # La variable va a ser igual 0 luego de la asignacion, suponiendo que su valor original era 10`
7. `//=` (Asignación por division entera), `x //= 5 # La variable va a ser igual 2 luego de la asignacion, suponiendo que su valor original era 10`
8. `**=` (Asignacion por potencia), `x **= 5 # La variable va a ser igual 100,000 luego de la asignacion, suponiendo que su valor original era 10`

El operador de identidad es para evaluar si dos valores son un mismo objeto, dos valores van a ser el mismo objeto mientras estén en la misma dirección de memoria:

```python
x = 100
y = x
x is y # True

y = 100
x is y # False
```

Podemos ver que aunque `y` sea igual a 100 (el valor de `x`) Python retorna un False, esto es porque su dirección de memoria no es igual; lamentablemente en Python no tenemos forma de interactuar con la memoria directamente, por lo que no podemos ver la dirección de memoria real, lo que sí podemos ver es el id del objeto, que es la abstracción o simplificación que tiene Python para la dirección de memoria.

```python
x = 100
y = x
id(x) == id(y) # True
id(x)
id(y)

y = 100
id(x) == id(y) # False
id(y)
```

Como pueden ver el id o dirección de memoria de la variable `y` cambia y cuando redefinimos su valor, además, cuando `y` es igual a `x` tiene el id de `x`.

En Python cada variable que declare va a estar en espacio de memoria diferente, es decir, cada uno va a tener una dirección de memoria única, por lo que aunque tenga dos variables con el mismo valor, no son el mismo objeto.

## Comentarios y doc strings

Como parte de ser un buen programador y para crear código mas mantenible con el tiempo, hay que saber manejar el dejar notas en nuestro código. Para esto, Python no deja dos herramientas sumamente útiles.

Los comentarios son partes de su código que a la hora de ejecutar su programa simplemente son ignorados, por lo que afecta su ejecución, un ejemplo de un comentario es `# Esto es un comentario` , como podrán observar, la sintaxis es simplemente agregar el símbolo `#` delante de su texto. 

Los docstrings son texto que se excribe entre tres comillas simples o dobles, este puede ser usado como texto en bloque por lo que al contrario de los comentarios, con solo un doc string pueden escribir varios parrafos.

```python
"""
Este es un docstring.
Puedo usar párrafos en el.
"""
```

## Condicionales

En programación, las condicionales son como en el mundo real, si una condición se cumple pueden pasar varias cosas, es igual en el código. A la hora de trabajar con condicionales entra el tema de los booleanos y los operadores de comparación que ya vimos anteriormente , primero empezaremos con el tipo de condicional mas sencillo.

La condicional o cláusula `if` es una palabra reservada que del inglés se traduce literalmente como *si…*, es decir, “Si pasa esto”, es como una suposición, esto lo podemos usar a nuestro favor para hacer uso de un bloque de código solo cuando algo específico pasa. `if` espera que le pasemos una condición o evaluación, la cual si es `True`, va a ejecutar el código que le pasemos.

```python
clave = "12345"
intento = input("Introduzca la clave: ")

if clave != intento: # La condicional devuelve True cuando se cumple
	print("Clave incorrecta, intenta de nuevo.")
```

En este ejemplo de código esperamos que el usuario introduzca una clave, la cual se va a comparar con la clave correcta que esta guardada en una variable. Si la clave es diferente a la que tenemos guardada, nos dira que la clave es incorrecta. En ese espacio que tiene el if para poner condicionales podemos usar los operadores lógicos y de comparación a nuestro antojo, tal cual estábamos haciendo hace un momento.

Esto esta bien, pero tenemos aun el caso donde debemos darle un mensaje de éxito al usuario si introduce la clave correcta, esto lo podríamos hacer con este código.

```python
clave = "12345"
intento = input("Introduzca la clave: ")

if clave != intento:
	print("Clave incorrecta, intenta de nuevo.")
	
if clave == intento:
	print("Clave correcta")
```

Este codigo funciona, pero en realidad, no es lo mas eficiente, ya que ambos `if` estan estrechamente relacionados entre ellos y si se fijan en las comparaciones, el de abajo solo actua cuando el de arriba es `False`, para estos casos donde queremos que cuando un `if` sea `False` haya otro que se ejecute tenemos la cláusula `else`, la cual solo se ejecuta cuando el `if` no lo hace.

```python
clave = "12345"
intento = input("Introduzca la clave: ")

if clave != intento:
	print("Clave incorrecta, intenta de nuevo.")
else:
	print("Clave correcta")
```

Este codigo hace lo mismo que el de arriba, pero ahora no se debe evaluar la condición de nuevo, ya que el `else` se va a ejecutar solo cuando el `if` sea `False`. Un `else` necesita si o si tener un `if` por encima, si no seria un error de sintaxis y su programa no funcionaria, por lo que esto seria invalido.

```python
clave = "12345"
intento = input("Introduzca la clave: ")

else: # No se evalua nada y falta el if
	print("Clave correcta")
```

Siguiendo con las condicionales nuevas, en caso de que quieran evaluar múltiples casos de uso relacionados entre si, pueden hacer uso de `elif`, `elif` es la combinación de `else` e `if`, si el la condicional que tiene arriba no se cumple, el pasa a evaluar algo y si es `True`, pasa a ejecutarse.

```python
clave = "12345"
segunda_clave = "123456"
intento = input("Introduzca la clave: ")

if clave != intento:
	print("Clave incorrecta, intenta de nuevo.")
elif clave != segunda_clave:
	print("La segunda clave tambien es incorrecta."
else:
	print("Clave correcta")
```

En este codigo, el usuario puede fallar introduciendo la primera clave y la segunda, pero si no falla con ninguna de las dos es porque sabe la clave, evidentemente, así que el `else` se ejecuta en ese caso de que las claves introducidas no sean diferentes a las guardadas.

Continuando, en otros lenguajes existe algo llamado `switch`, Python no lo tiene pero tiene algo muy parecido (por no decir identico) llamado `match` . Su sintaxis es la siguiente.

```python
match variable_a_evaluar:
	case "Posible valor":
		print("Codigo")
	case _: # este es el else del los match
		print("Codigo")
```

Como pueden ver es casi el mismo código de antes, en el parámetro del `match` se espera que se pase una variable (la que queremos evaluar) y los `case` son todos los posibles valores que puede tener. No es recomendado usar `match`.

## Métodos y funciones

Es importante que en este punto diferenciemos lo que es un método y una función, ya que son muy similares pero no son lo mismo. Una función es un bloque de código reutilizable, esta realiza una tarea en específico, mientras que un método es una función asociada a un objeto, es decir, una función que se relaciona a un objeto específico. Esto lo acabarán de entender más adelante cuando estemos trabajando con objetos y funciones.

## Estructuras de datos, manipulación y métodos

Las estructuras de datos son un conjunto de datos ordenados de una manera que permite interpretar y organizar la información de mejor manera, ya que estas siguen un orden o patrón designado.

Este tema existe en todos los lenguajes de programación por igual, pero no existen las mismas estructuras, en el caso de Python existen las listas, diccionarios, tuplas y conjuntos, cada cual tiene sus características especiales por si mismos.

Las listas son el tipo mas usado de estructura de datos en Python, estas son una lista desordenada de datos, se pueden  repetir datos aquí y su manipulación no es complicada. La sintaxis es simple, solo debemos poner un identifcador y un valor, como si fuera una variable, solo que a la hora de designar el valor, deben ser dos llaves, como en este ejemplo.

```python
lista = [] # Lista vacia
lista2 = [19, "Hola", True] # Lista con elementos
```

Las listas pueden declararse vacias o con elementos dentro, ademas, pueden tener dentro cualquier tipo de dato, mezclados o no.

En Python todo es un objeto, las listas no son la excepcion, por lo que tenemos los llamadas *metodos* para editar este objeto.

```python
lista = []
lista.append("Metodo Append")
print(lista)
```

Como pueden ver la sintaxis de los metodos es `objeto.metodo` , en este codigo el metodo `append()` agrega un elemento al final de la lista. 

Las listas se organizan e interpretan por indices, es decir, no van a conseguir un valor de una lista introduciendo simplemente el valor, deben indicar el indice o posición donde esta. El primer elemento de una lista esta en la posición 0, por lo que el 2 esta en el índice o posición 1 y así con todos los demás.

```python
lista_nums = [1, 2, 3, 4, 5]
print(lista_nums[0], "-", lista_nums[4]) # 1-5
```

Los métodos mas comunes para editar listas son los siguientes.

```python
mi_lista = [1, 2, 3, 4, 5]
mi_lista.append(6)  # Añadir un elemento al final
# Insertar un elemento en una posición específica
# El primer argumento es la posicion (que recuerden va a partir del 0)
# Y el segundo es el valor a introducir, puede ser lo que sea
mi_lista.insert(2, 9) 
# Eliminar el primer elemento cuyo valor sea 9
mi_lista.remove(9)  
# Eliminar y devolver el último elemento
# Devolver significa retorno, osea que si guardan el pop
# En una variable van a ver el elemento en su variable
# Dentro de los parentesis tambien pueden pasarle un argumento
# Para borrar el elemento de una posicion especifica
retorno = mi_lista.pop() 
print(retorno)
mi_lista.pop(1) # Elimina el valor de la posicion 1
# Ordenar la lista
# En numeros, por defecto es en orden ascendente
# En el texto depende del parametro key que se le pase
# key=len, por ejemplo, ordena todo en base a su tamaño
mi_lista.sort() 
# Invertir los elementos de la lista 
mi_lista.reverse()  
# Para conocer el indice de un elemento puede usar el metodo index
# Este metodo se comparte con las tuplas
indice = mi_lista.index(3)

# Para editar una lista solo tiene que llamar a la lista por su indice
# En este caso el valor de la posicion 2 es editado
mi_lista[2] = "Nuevo valor"
```

Las tuplas son un tipo de estructura de dato que es inmutable, es decir, estas no pueden ser editadas, por lo que una vez definidas siguen siendo iguales siempre. Los metodos comunes, por lo tanto, son practicamente nulos. Las tuplas se definen igual que las listas, pero en vez de usar `[]` se usan parentesis. Ademas, las tuplas son mas rapidas para acceder a su contenido y ocupan menos memoria.

```python
mi_tupla = (1, 2, 3, 4, 5)  # Crear una tupla
print(mi_tupla.count(3))  # Contar el número de veces que aparece un valor
print(mi_tupla.index(4))  # Obtener el índice de un valor
```

Esto es todo por parte de las tuplas.

Otro tipo de dato muy importante son los diccionarios, estos son tal cual como los diccionarios que conocemos, tienen una palabra que se llama clave y un valor asignado a dicha clave, se declaran entre llaves (`{}`), estos son una estructura desordenada tambien. Las claves no se pueden repetir, pero los valores si.

```python
diccionario = {"clave":"valor", "a":1, "b":False}
```

La forma en la que se interactua con ellos es la siguiente.

```python
mi_diccionario = {"a": 1, "b": 2, "c": 3}

# Esta primera parte es similar a los indices de las listas
# Añadir un nuevo par clave-valor
mi_diccionario["d"] = 4  
# Actualizar el valor de una clave existente
mi_diccionario["a"] = 10 

# Obtener el valor asociado a una clave
valor = mi_diccionario.get("a") # Este mas seguro porque devuelve None
# si no encuentra nada, en cambio este otro da un error y detiene el programa.
valor = mi_diccionario["a"]

mi_diccionario.pop("b")  # Eliminar un par clave-valor por su clave

mi_diccionario.update({"e": 5, "f": 6})  # Actualizar el diccionario con otro diccionario

claves = mi_diccionario.keys()  # Obtener todas las claves del diccionario
valores = mi_diccionario.values()  # Obtener todos los valores del diccionario
items = mi_diccionario.items()  # Obtener todos los pares clave-valor del diccionario

mi_diccionario.clear()  # Eliminar todos los elementos del diccionario
```

Puedes crear un conjunto usando llaves `{}` o la función `set()`. Los conjuntos o sets son una estructura de datos que es ordenada y donde sus elementos no pueden repetirse, por lo tanto es buena para almacenar id unicos.

```python
# Crear un conjunto vacío
mi_conjunto = set()

# Crear un conjunto con elementos
mi_conjunto = {1, 2, 3, 4, 5}

# Crear un conjunto a partir de una lista
mi_lista = [1, 2, 2, 3, 4, 4, 5]
mi_conjunto = set(mi_lista)  # {1, 2, 3, 4, 5}

```

### Métodos Comunes

- **`add(x)`**: Añade un elemento al conjunto.
    
    ```python
    mi_conjunto.add(6)  # {1, 2, 3, 4, 5, 6}
    ```
    
- **`remove(x)`**: Elimina un elemento del conjunto. Lanza un `KeyError` si el elemento no existe.
    
    ```python
    mi_conjunto.remove(6)  # {1, 2, 3, 4, 5}
    ```
    
- **`discard(x)`**: Elimina un elemento del conjunto si existe. No lanza un errores si el elemento no existe.
    
    ```python
    mi_conjunto.discard(5)  # {1, 2, 3, 4}
    ```
    
- **`pop()`**: Elimina y devuelve el primer elemento del conjunto.
    
    ```python
    elemento = mi_conjunto.pop()  # Devuelve un elemento y elimina del conjunto
    ```
    
- **`clear()`**: Elimina todos los elementos del conjunto.
    
    ```python
    mi_conjunto.clear()  # set()
    ```
    
- **`union(conjunto2)`**: Devuelve un nuevo conjunto con la unión de dos conjuntos.
    
    ```python
    otro_conjunto = {4, 5, 6, 7}
    union = mi_conjunto.union(otro_conjunto)  # {1, 2, 3, 4, 5, 6, 7}
    ```
    
- **`intersection(conjunto2)`**: Devuelve un nuevo conjunto con los elementos comunes a ambos conjuntos. Es decir, los que se repiten en ambos conjuntos.
    
    ```python
    interseccion = mi_conjunto.intersection(otro_conjunto)  # {4}
    ```
    
- **`difference(conjunto2)`**: Devuelve un nuevo conjunto con los elementos del primer conjunto que no están en el segundo. El conjunto que se pasa como parametro es el segundo conjunto.
    
    ```python
    diferencia = mi_conjunto.difference(otro_conjunto)  # {1, 2, 3}
    ```
    
- **`symmetric_difference(conjunto2)`**: Devuelve un nuevo conjunto con los elementos que están en uno de los conjuntos, pero no en ambos.
    
    ```python
    diferencia_simetrica = mi_conjunto.symmetric_difference(otro_conjunto)  # {1, 2, 3, 6, 7}
    ```
    
- **`issubset(conjunto2)`**: Devuelve `True` si todos los elementos del conjunto están en `conjunto2`.
    
    ```python
    es_subset = mi_conjunto.issubset(otro_conjunto)  # False
    ```
    
- **`issuperset(conjunto2)`**: Devuelve `True` si todos los elementos de `conjunto2` están en el conjunto.
    
    ```python
    es_superset = otro_conjunto.issuperset(mi_conjunto)  # True
    ```
    

## Slicing

El slicing (segmentación) es una característica de Python que permite extraer sublistas, subtuplas, o subcadenas de secuencias como listas, tuplas y cadenas. El proceso de acceder a la informacion de listas mediante slicing o bucles es llamada iteracion.

### Slicing en Listas

```python
# Crear una lista
mi_lista = [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]

# Sintaxis básica: lista[inicio:fin:paso]
sub_lista = mi_lista[2:7]  # [2, 3, 4, 5, 6]
sub_lista_con_paso = mi_lista[2:7:2]  # [2, 4, 6]

# Omitir el índice de inicio
inicio_a_5 = mi_lista[:6]  # [0, 1, 2, 3, 4, 5]

# Omitir el índice de fin
de_5_en_adelante = mi_lista[5:]  # [5, 6, 7, 8, 9]

# Slicing con paso negativo (invertir la lista)
invertida = mi_lista[::-1]  # [9, 8, 7, 6, 5, 4, 3, 2, 1, 0]
```

### Slicing en Cadenas

```python
# Crear una cadena
mi_cadena = "abcdefghij"

# Sintaxis básica: cadena[inicio:fin:paso]
sub_cadena = mi_cadena[2:7]  # "cdefg"
sub_cadena_con_paso = mi_cadena[2:7:2]  # "ceg"

# Omitir el índice de inicio
inicio_a_5_cadena = mi_cadena[:6]  # "abcdef"

# Omitir el índice de fin
de_5_en_adelante_cadena = mi_cadena[5:]  # "fghij"

# Slicing con paso negativo (invertir la cadena)
invertida_cadena = mi_cadena[::-1]  # "jihgfedcba"
```

### Slicing en Tuplas

```python
# Crear una tupla
mi_tupla = (0, 1, 2, 3, 4, 5, 6, 7, 8, 9)

# Sintaxis básica: tupla[inicio:fin:paso]
sub_tupla = mi_tupla[2:7]  # (2, 3, 4, 5, 6)
sub_tupla_con_paso = mi_tupla[2:7:2]  # (2, 4, 6)

# Omitir el índice de inicio
inicio_a_5_tupla = mi_tupla[:6]  # (0, 1, 2, 3, 4, 5)

# Omitir el índice de fin
de_5_en_adelante_tupla = mi_tupla[5:]  # (5, 6, 7, 8, 9)

# Slicing con paso negativo (invertir la tupla)
invertida_tupla = mi_tupla[::-1]  # (9, 8, 7, 6, 5, 4, 3, 2, 1, 0)
```

### Ejemplo Completo con Comentarios

```python
# Listas
mi_lista = [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]
print(mi_lista[2:7])  # [2, 3, 4, 5, 6]
print(mi_lista[:6])  # [0, 1, 2, 3, 4, 5]
print(mi_lista[5:])  # [5, 6, 7, 8, 9]
print(mi_lista[::2])  # [0, 2, 4, 6, 8]
print(mi_lista[::-1])  # [9, 8, 7, 6, 5, 4, 3, 2, 1, 0]

# Cadenas
mi_cadena = "abcdefghij" # Asi es, los string tambien son iterables
print(mi_cadena[2:7])  # "cdefg"
print(mi_cadena[:6])  # "abcdef"
print(mi_cadena[5:])  # "fghij"
print(mi_cadena[::2])  # "acegi"
print(mi_cadena[::-1])  # "jihgfedcba"

# Tuplas
mi_tupla = (0, 1, 2, 3, 4, 5, 6, 7, 8, 9)
print(mi_tupla[2:7])  # (2, 3, 4, 5, 6)
print(mi_tupla[:6])  # (0, 1, 2, 3, 4, 5)
print(mi_tupla[5:])  # (5, 6, 7, 8, 9)
print(mi_tupla[::2])  # (0, 2, 4, 6, 8)
print(mi_tupla[::-1])  # (9, 8, 7, 6, 5, 4, 3, 2, 1, 0)
```

### Descripción del Slicing

- **`inicio:fin`**: Selecciona elementos desde `inicio` hasta `fin-1`. El final es variable, representado por el final o longitud de la lista, el inicio generalmente es 0, pero podemos cambiarlo a lo que queramos.
- **`inicio:fin:paso`**: Selecciona elementos desde `inicio` hasta `fin-1`, saltando `paso` elementos. El paso son los saltos que debe dar la lista mientras se va recorriendo, es decir, si vamos a leer los elementos de la lista 1 a 1 o si vamos a dar saltos entre ellos. `[1, 2, 3, 4, 5, 6]` ⇒ `[0:5:1] # 1, 2...` ⇒ `[::2] # 1, 3, 5`
- **`[:fin]`**: Selecciona elementos desde el principio hasta `fin-1`. En Python cuando no se especifica  una posicion se obvia y se pone automaticamente, en este caso como el primer elemento no esta especificado el inicio, por lo que se toma como que es 0. `[:] = [0:5]`
- **`[inicio:]`**: Selecciona elementos desde `inicio` hasta el final. En este caso la representacion seria la misma `[:]`
- **`[::-1]`**: Invierte la secuencia. Esto porque el paso es negativo, por lo que va desde el ultimo elemento hacia el primero.

# Parte 2 (+1 hora)

## Conversion de datos

Para convertir datos se pueden usar funciones como `int()` , `float()`, `str()`,`list()`, `bool()`, `dict()` . Las funciones de conversión de datos no sirven para hacer comparaciones o para transformar variables a otros tipos de datos datos.

## Funciones

Una funcion es un bloque de codigo que sigue la estructura de tener un identificador o nombre, datos de entrada llamados parametros o argumento y finalmente, este tiene una salida o retorno dependiendo de lo que haga esa funcion. A la hora de definir esta funcion debemos definir lo que va a hacer, el codigo que va a contener. 

Para declarar una funcion el nombre puede empezar por una letra o guion bajo, pero no puede ser igual a una palabra reservada por python, la cantidad de codigo que esta puede almacenar es ilimitada, pero lo recomendable es que sean lo menos posible, generalmente las funciones no deberian tener mas de 60 lineas (esto no es un dogma, depende el caso pueden usar esto o no). Las funciones nos sirven para guardar el codigo que es recurrente en nuestro codigo, hace que evitemos repetir lo mismo multiples veces en nuestro codigo. 

Aqui podemos ver de nuevo el concepto de entrada y salida. Al definir una funcion se definen sus parametros, que son variables; estos parametros de la funcion pueden ser de cualquier tipo segun se necesite, esta seria la operacion de entrada de la que tenemos control en la funcion. Con el uso de la palabra reservada `return` podemos retornar informacion, siendo una operacion de salida dentro de nuestro programa. 

## Argumentos en las funciones

### `args`

- `args` se utiliza para pasar un número variable de argumentos no nombrados (posicionales) a una función.
- `args` agrupa todos los argumentos posicionales adicionales en una tupla.

### Ejemplo:

```python
pythonCopy code
def suma(*args):
    total = 0
    for num in args:
        total += num
    return total

# Llamadas a la función
print(suma(1, 2, 3))       # Output: 6
print(suma(10, 20, 30, 40)) # Output: 100

```

### `*kwargs`

- `*kwargs` se utiliza para pasar un número variable de argumentos nombrados (clave-valor) a una función.
- `*kwargs` agrupa todos los argumentos con nombre adicionales en un diccionario.

### Ejemplo:

```python
pythonCopy code
def mostrar_info(**kwargs):
    for key, value in kwargs.items():
        print(f"{key}: {value}")

# Llamadas a la función
mostrar_info(nombre="Juan", edad=25, ciudad="Madrid")
# Output:
# nombre: Juan
# edad: 25
# ciudad: Madrid
```

## Bucles

Los bucles son estructuras de control usadas en la programacion para repetir varias veces acciones repetitivas, estos bucles tienen una sintaxis propia y se usan dependiendo lo que deseen. Los bucles que podemos usar en Python son el bucle `for` y `while` . Palabras reservadas: `break`, `continue`

## Formateo de texto

En el formateo de texto encontramos una serie de códigos agregados para hacer que los textos tengan cierto formato. 

## Generadores

Sirven para hacer iteradores y guardan su estado entre asignaciones.

## Lambda o anónimas

Funciones de una sola línea.

## Excepciones y manejo de errores

`try` , `except`, `finally`.