## Markdown
### Indice de sintaxis Markdown
![Texto alternativo](/logo.PNG)

En el lenguaje Markdown encontrarás tres tipos de elementos básicos que a su vez engloban el resto de la sintaxis. Considera esto una cheat sheet con la que guiarte.

**Elementos de bloque:**
- Párrafos y saltos de línea
- Encabezados
- Citas
- Listas
- Códigos de bloque
- Reglas horizontales

**Elementos de línea**
- Énfasis
- Links o enlaces
- Código
- Código

**Elementos varios**
- Links automáticos
- Omitir Markdown

## Elementos de bloque
### Párrafos y saltos de línea

Para generar un nuevo párrafo en Markdown simplemente separa el texto mediante una línea en blanco **(pulsando dos veces intro)**
Al igual que sucede con HTML, **Markdown no soporta dobles líneas en blanco**, así que si intentas generarlas estas se convertirán en una sola al procesarse
Para realizar un salto de línea y empezar **una frase en una línea siguiente dentro del mismo párrafo**, tendrás que pulsar **dos veces la barra espaciadora antes de pulsar una vez intro.**
Por ejemplo si quisieses escribir un poema Haiku quedaría tal que así:

«Andando con sus patitas mojadas,
el gorrión
por la terraza de madera»

Donde cada verso tiene **dos espacios en blanco al final.**

## Encabezados
Las  #  **almohadillas** son uno de los métodos utilizados en Markdown para crear encabezados. Debes usarlos añadiendo **uno por cada nivel.**

Es decir,
~~~
# Encabezado 1
## Encabezado 2
### Encabezado 3
#### Encabezado 4
##### Encabezado 5
###### Encabezado 6
~~~
Se corresponde con

# Encabezado 1
## Encabezado 2
### Encabezado 3
#### Encabezado 4
##### Encabezado 5
###### Encabezado 6

También puedes cerrar los encabezados con el mismo número de almohadillas, por ejemplo escribiendo  ### Encabezado 3 ### . Pero la única finalidad de esto es un **motivo estético.**

Existe otra manera de generar encabezados, aunque este método está **limitado a dos niveles.**
Consiste en subrayar los encabezados con el símbolo = (para el encabezado 1), o con guiones - para el encabezado 2.
Es decir,
~~~
Esto sería un encabezado 1
===
Esto sería un encabezado 2
—-
~~~
No existe un número concreto = o - que necesites escribir para que esto funcione, ¡incluso bastaría con uno!

### Citas
Las citas se generar utilizando el carácter mayor que > al comienzo del bloque de texto.
~~~
> Un país, una civilización se puede juzgar por la forma en que trata a sus animales.  — Mahatma Gandhi
~~~
> Un país, una civilización se puede juzgar por la forma en que trata a sus animales. — Mahatma Gandhi

Si la cita en cuestión se compone de varios párrafos, deberás añadir el mismo símbolo > al comienzo de cada uno de ellos.
~~~
> Creo que los animales ven en el hombre un ser igual a ellos que ha perdido de forma extraordinariamente peligrosa el sano intelecto animal.
> Es decir, que ven en él al animal irracional, al animal que ríe, al animal que llora, al animal infeliz. — Friedrich Nietzsche
~~~
> Creo que los animales ven en el hombre un ser igual a ellos que ha perdido de forma extraordinariamente peligrosa el sano intelecto animal.

> Es decir, que ven en él al animal irracional, al animal que ríe, al animal que llora, al animal infeliz. — Friedrich Nietzsche

Incluso puedes concatenar varios >> para crear citas anidadas.
~~~
> Esto sería una cita como la que acabas de ver.
> 
> > Dentro de ella puedes anidar otra cita.
> 
> La cita principal llegaría hasta aquí. 
~~~
> Esto sería una cita como la que acabas de ver.
> 
> > Dentro de ella puedes anidar otra cita.
> 
> La cita principal llegaría hasta aquí.

Recuerda separar los saltos de línea con >, o >> si te encuentras dentro de la cita anidada; para crear párrafos dentro del mismo bloque de cita.

### Listas

A diferencia de lo que ocurre en HTML, generar listas en Markdown es tremendamente sencillo. Puedes encontrarte con dos tipos.

#### Listas desordenadas

Para crear **listas desordenadas utiliza * asteriscos, - guiones, o + símbolo de suma**

~~~
- Elemento de lista 1
- Elemento de lista 2
* Elemento de lista 3
* Elemento de lista 4
+ Elemento de lista 5
+ Elemento de lista 6
~~~

Da igual qué elemento escojas, incluso puedes intercambiarlos. Todos se verán igual al procesarse.

- Elemento de lista 1
- Elemento de lista 2
* Elemento de lista 3
* Elemento de lista 4
+ Elemento de lista 5
+ Elemento de lista 6

 Para generar **listas anidadas** dentro de otras, simplemente tendrás que añadir **cuatro espacios en blanco antes del siguiente *, - o +. 
~~~
- Elemento de lista 1
- Elemento de lista 2
    - Elemento de lista 3
    - Elemento de lista 4
        - Elemento de lista 5
        - Elemento de lista 6
~~~

- Elemento de lista 1
- Elemento de lista 2
    - Elemento de lista 3
    - Elemento de lista 4
        - Elemento de lista 5
        - Elemento de lista 6

#### Listas ordenadas
Para crear listas ordenadas debes utilizar la sintaxis de tipo: «número.» 1.. Al igual que ocurre con las listas desordenadas, también podrás **anidarlas** o **combinarlas**.
~~~
1. Elemento de lista 1
2.  Elemento de lista 2
    - Elemento de lista 3
    - Elemento de lista 4
        1. Elemento de lista 5
        2. Elemento de lista 6
~~~
1. Elemento de lista 1
2.  Elemento de lista 2
    - Elemento de lista 3
    - Elemento de lista 4
        1. Elemento de lista 5
        2. Elemento de lista 6

### Códigos de bloque
Si quieres crear un bloque entero que contenga código. Lo único que tienes que hacer es **encerrar dicho párrafo entre dos líneas formadas por tres ~ virgulillas**.

Tal que así:
~~~
~~~
Creando códigos de bloque.
Puedes añadir tantas líneas y párrafos como quieras.  
~~~
~~~
De esta forma, obtendrás el siguiente resultado:
~~~
Creando códigos de bloque.
Puedes añadir tantas líneas y párrafos como quieras.  
~~~

### Reglas horizontales

Las reglas horizontales se utilizan para separar secciones de una manera visual. Las estás viendo constantemente en este artículo ya que las estoy utilizando para separar los diferentes elementos de sintaxis de Markdown.

Para crearlas, en una línea en blanco deberás incluir **tres de los siguientes elementos:** asteriscos, guiones, o guiones bajos.

Es decir
~~~
***
---
___
~~~
También puedes separarlos mediante un espacio en blanco por pura estética.
~~~
* * *
- - -
_ _ _
~~~

## Elementos de línea
### Énfasis (negritas y cursivas)
Markdown utiliza **asteriscos** o **guiones bajos** para enfatizar.

Simplemente tendrás que envolver palabras o textos en éstos símbolos para conseguir *cursivas* o **negritas**.

![Texto alternativo](/markwn1.PNG)

Por supuesto si quieres utilizar los dos tipos de énfasis no tienes más que **combinar la sintaxis**, envolviendo la palabra entre tres asteriscos o tres guiones bajos.

![Texto alternativo](/markdwn2.PNG)

## Links o enlaces
Añadir enlaces a una publicación, más que común, hoy en día es algo **casi obligatorio**. Con Markdown tendrás varias formas de hacerlo.

#### Links o enlaces en línea
Son los enlaces de toda la vida. Como su nombre indica, se encuentran en línea con el texto.

Se crean escribiendo la palabra o texto enlazada entre [] **corchetes**, y el link en cuestión entre () **paréntesis**.

