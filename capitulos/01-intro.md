# Introducci�n

Ruby es un lenguaje de programaci�n de uso general, que ejecuta en m�ltiples plataformas. Es un lenguaje
interpretado, lo que posibilita que sea din�mico: incluso podemos tener programas que se modifican a s�
mismos en ejecuci�n. Tiene muchas caracter�sticas en com�n con otros lenguajes tipo scripting, como Perl y
Python. Ruby tiene palabras claves en ingl�s, lo cual lo hace parecer a un Pascal moderno. Es orientado
objetos y se nota la influencia de Smalltalk en su dise�o interno. El lenguaje Ruby fue creado por
Yukihiro Matsumoto (conocido en el ambiente como Matz). Su primera versi�n fue liberada en 1995. El mismo
reconoce en sus presentaciones que los lenguajes que influyeron en el dise�o de Ruby fueron Smalltalk, Lisp
y Perl. Tambi�n se menciona como influencias a Eiffel y Ada.

Pero como programadores, �qu� podemos encontrar hoy en Ruby? Bueno, en mi opini�n, Ruby tiene caracter�sticas
que es dif�cil de encontrar juntas en otros lenguajes:

- Es f�cil de aprender
- Es f�cil de escribir
- Es flexible
- Es poderoso
- Tiene un gran ecosistema de librer�as (gemas) y frameworks
- Una comunidad activa

Espero que al leer estas p�ginas, les pueda transmitir por qu� aseguro lo de arriba.

## Instalaci�n

Ya les cont� que Ruby es multiplataforma. Lo que en la pr�ctica se traduce que pueden programar en Windows, Linux
y Mac OS/X usando Ruby, y con un poco de cuidado, usar el mismo c�digo en todas esas plataformas. Eso lo convierte
en un excelente lenguaje para aprender y practicar: cuando uno escribe un sitio web, por ejemplo, en Windows, luego
lo puede desplegar en un servidor Linux sin mayor problema (bueno, siempre el diablo puede poner la cola ;-).

Este curso fue escrito usando Ruby 2.0, y espero seguir actualiz�ndolo para cuando aparezcan nuevas versiones. Y fue
escrito y probado principalmente en m�quinas con Windows. Pero todo lo que veremos se puede ejecutar con
Ruby 1.9.x, y en otras plataformas. Si encuentra algo que no es as�, por favor reportarlo en los [issues de GitHub](https://github.com/ajlopez/AprendiendoRuby/issues)
de este repo.

(A completar)

## Ruby Interactivo

Con la instalaci�n de Ruby viene un programa `irb` (de Interactive Ruby) que se puede invocar
desde la l�nea de comando. Por ejemplo

- Si estamos en **Mac OS X** abrimos `Terminal` e ingresamos `irb` y enter
- Si estamos en **Linux** abrimos un shell e ingresamos `irb` y enter
- Si estamos en **Windows** abrimos una caja de DOS e ingresamos `irb` y enter

Entonces aparece algo como

```
irb(main):001:0>
```

Y ahora �qu� hacemos? Seamos educados, y saludemos al programa. Simplemente ingresamos `"Hola IRB"` y obtenemos

```
irb(main):001:0> "Hola IRB"
=> "Hola IRB"
```

Hasta podemos usarlo como una calculadora con esteroides :-)
```
irb(main):001:0> 1+2
=> 3
irb(main):002:0> 3/4
=> 0
```
Vean que en el �ltimo caso la divisi�n es entera.

Y tenemos funciones predefinidas
```
irb(main):001:0> puts "Hola IRB"
Hola IRB
=> nil
```
Noten que una cosa es el resultado de invocar a la funci�n predefinida `puts`, que termina
imprimiendo en la consola el mensaje que le pasamos como par�metro, y otra cosa es lo que
esa funci�n devuelve, el valor `nil`, que podemos por ahora asimilar al `null` de otros lenguajes
como C#, Java o JavaScript

> Nota: no hace falta verlo ahora, pero les adelanto que `nil` es un objeto, tiene m�todos asociados y hasta una clase, la clase `NilClass`, cosa que no
asombrar� a los programadores Smalltalk

Podr�amos ingresar varias l�neas, y definir funciones, e invocarlas. Vamos a ir viendo estos temas
pero si quieren, pueden probar cosas como:

```ruby
irb(main):001:0> n = 1
=> 1
irb(main):002:0> m = 2
=> 2
irb(main):003:0> def twice(a)
irb(main):004:1>    a*2
irb(main):005:1> end
=> nil
irb(main):006:0> twice(2)
=> 4
irb(main):007:0>
```

El `def twice(a)` hasta el `end` es la forma que tenemos en Ruby para definir
una funci�n. En la l�nea 6 la invocamos, pas�ndole como �nico par�metro a `2`.

## Ejecutando Archivos Ruby

(A completar)

## Probando Ruby en L�nea

(A completar)

## Fuente consultadas:

- [Ruby in Twenty Minutes](http://www.ruby-lang.org/en/documentation/quickstart/)
