# Examen Parcial - nicolascrespo-dotcom

**Usuario GitHub:** nicolascrespo-dotcom
**Fecha:** 4 de noviembre de 2025
**Retos tenidos en cuenta:** Reto 003

---

## Instrucciones

A continuación encontrarás fragmentos de código extraídos de tus entregas. Cada fragmento contiene una o más situaciones relacionadas con los conceptos vistos en clase.

Para cada pregunta debes:
1) Identificar a qué se refiere la observación
2) Explicar si es o no un error y por qué
3) Proponer la corrección

Nota: Responde 5 de las 10 preguntas (en función a lo indicado en el examen).


---

## Pregunta 1

Archivo: `reto-003.java` — [Ver archivo](https://github.com/mmasias/25-26-PRG1/blob/2a6e8b6dfca704a09231d5ccc0d8dec2d30f3111/entregas/CrespoNicolas/reto-003.java) (Reto 003)

```java
for (int hora = 0; hora < 24; hora++) {
    System.out.print("Son las " + hora + "del dia " + dia);
    // ...
}
```

¿Qué observas en este código?

---

## Pregunta 2

Archivo: `reto-003.java` — [Ver archivo](https://github.com/mmasias/25-26-PRG1/blob/2a6e8b6dfca704a09231d5ccc0d8dec2d30f3111/entregas/CrespoNicolas/reto-003.java) (Reto 003)

```java
if (columna == 3) {
    System.out.print(SEPARADOR);
} else {
    System.out.print(LADRILLOS + (!abierta ? VENTANA_CERRADA : (encendida ? VENTANA_ABIERTA_CON_LUZ : VENTANA_ABIERTA_SIN_LUZ)) + LADRILLOS);
}
```

¿Qué observas en este código?

---

## Pregunta 3

Archivo: `reto-003.java` — [Ver archivo](https://github.com/mmasias/25-26-PRG1/blob/2a6e8b6dfca704a09231d5ccc0d8dec2d30f3111/entregas/CrespoNicolas/reto-003.java) (Reto 003)

```java
final String VENTANA_ABIERTA_SIN_LUZ = "[º]";
final String VENTANA_ABIERTA_CON_LUZ = "[*]";
final String SEPARADOR = "[   ]";
final String LADRILLOS = ":";
```

¿Qué observas en este código?

En este codigo se puede identificar como se definen 4 variables final string, las cuales consiten en cadenas de texto que nun ca seran modificadas bajo ningun concepto, su notacion en screaming snake es correcta, el unico problema que les podria ver es que los nombres de las 2 primeras quizas son demasiado largos, pero a mi parecer no son errores como tal, mas bien es una cuestion de gustos.

---

## Pregunta 4

Archivo: `reto-003.java` — [Ver archivo](https://github.com/mmasias/25-26-PRG1/blob/2a6e8b6dfca704a09231d5ccc0d8dec2d30f3111/entregas/CrespoNicolas/reto-003.java) (Reto 003)

```java
System.out.println("               __/\\__\n" +
                  "  |    |    |  |####|  |    |    |  \n" +
                  "====================================");
// ...
System.out.println("------------------------------------\n" +
                   "     ==========================\n" +
                   "   ==============================\n" +
                   " ==================================");
```

¿Qué observas en este código?

Este fragmento de codigo se pueden observar 2 comandos iguales "System.out.println()"  los cuales son utilizados comunmente para imprimir  datos o texto en la termiinal, el ln de el final se utiliza para que los imprima en la linea siguiente. Estos tambien son comunmente escritos como sout en modo de abreviacion. Concretamente aqui estan imprimiendo el techo y suelo de un hotel respectivamente, y esto lo se porque el ejercicio lo hice yo, porque de haberlo hecho otra persona no entenderia lo que hacen, y ahi es donde yo considero que radica el error de este fragmento.Como solucion creo que seria adecuado meter ambas cadenas de texto en 2 final string, ya que estas son fijas y no cambiaran nunca y ponerlas un nombre identificativo en el formato screamig snake, que es el adecuado para las variables finales,y que consiste en escribir las palabras totalmente en mayusculas y separadas por guiones bajos, unos nombres adecuados serian "TEJADO_HOTEL" y "PLANTA_BAJA"  respectivamente, y valdria con despues de crear las variables meterlas sin entrecomillar dentro de los sout.

---

## Pregunta 5

Archivo: `reto-003.java` — [Ver archivo](https://github.com/mmasias/25-26-PRG1/blob/2a6e8b6dfca704a09231d5ccc0d8dec2d30f3111/entregas/CrespoNicolas/reto-003.java) (Reto 003)

```java
public class HotelDeLaAgonia {
    public static void main(String[] args) {
        // ...
    }
}
```

¿Qué observas en este código?

---

## Pregunta 6

Archivo: `reto-003.java` — [Ver archivo](https://github.com/mmasias/25-26-PRG1/blob/2a6e8b6dfca704a09231d5ccc0d8dec2d30f3111/entregas/CrespoNicolas/reto-003.java) (Reto 003)

```java
for (int dia = 1; dia <= 7; dia++) {
    for (int hora = 0; hora < 24; hora++) {
        System.out.print("Son las " + hora + "del dia " + dia);
        System.out.println();
        System.out.println("               __/\\__\n" + //
                "  |    |    |  |####|  |    |    |  \n" + //
                "====================================");
        for (int planta = 1; planta <= 7; planta++) {
            for (int columna = 1; columna <= 6; columna++) {
```

¿Qué observas en este código?

---

## Pregunta 7

Archivo: `reto-003.java` — [Ver archivo](https://github.com/mmasias/25-26-PRG1/blob/2a6e8b6dfca704a09231d5ccc0d8dec2d30f3111/entregas/CrespoNicolas/reto-003.java) (Reto 003)

```java
for (int columna = 1; columna <= 6; columna++) {
    abierta = Math.random() < PERSIANA_ABIERTA;
    encendida = Math.random() < LUZ_ENCENDIDA;
    if (columna == 3) {
        System.out.print(SEPARADOR);
    }else {System.out.print(LADRILLOS+(!abierta ? VENTANA_CERRADA: (encendida ? VENTANA_ABIERTA_CON_LUZ : VENTANA_ABIERTA_SIN_LUZ))+LADRILLOS);}
}
```

¿Qué observas en este código?

---

## Pregunta 8

Archivo: `batalla` — [Ver archivo](https://github.com/mmasias/25-26-PRG1/blob/319e41ca940d686ce0fc460f8ff2d4117acf3e53/batalla) (Reto 002)

```java
if (Math.random() < posibilidadExitoGuerrero && numeroArmaEscogida != 4) {
    System.out.println("El vampiro se lleva un golpe");
    vidaVampiro = vidaVampiro - dañoGuerrero;
} else if (Math.random() < posibilidadExitoGuerrero && numeroArmaEscogida == 4) {
    System.out.println("Te defiendes exitosamente del vampiro!!");
} else if (Math.random() > posibilidadExitoGuerrero && numeroArmaEscogida == 4) {
    System.out.println("No logras defenderte del vampiro!!");
} else {
    System.out.println("El vampiro ha esquivado el golpe");
}
```
¿Qué observas en este código?

El error mas significativo en este fragmento de codigo, a mi parecer es esa implementecion de un "numero magico", ese 4 que representa , lo cual se por que yo hice ese codigo es el escudo de el guerrero, pero esto no queda claro, asi que sugeriria cambiar ese 4 por una variable final con ese valor dado, la cual se podria llamr algo como ESCUDO o similar, para que el lector podria identificar que esa parte.
En cuanto a la logica de el codigo las condiciones if/else if son largas y tienen operadores lógicos (&&, ||), lo que las hace difíciles de seguir de un vistazo. La condición Math.random() < posibilidadExitoGuerrero se repite en las dos primeras ramas. Si la lógica de éxito cambia, debe actualizarse en dos lugares. Ademas al leer la segunda condición (else if (Math.random() < posibilidadExitoGuerrero && numeroArmaEscogida == 4)), el lector tiene que procesar tanto la probabilidad de éxito como la identificación del arma. Sería más claro manejar primero la decisión principal (el tipo de acción basada en el arma) y luego el resultado secundario (el éxito).

---

## Pregunta 9

Archivo: `batalla` — [Ver archivo](https://github.com/mmasias/25-26-PRG1/blob/319e41ca940d686ce0fc460f8ff2d4117acf3e53/batalla) (Reto 002)

```java
} else {
    System.out.println("Troleas y el vampiro se pica");
    posibilidadExitoGuerrero = 0;
    dañoGuerrero = 0;
    dañoVampiro = vidaGuerrero;
    probabilidadExitoVampiro = 1;
}
```

¿Qué observas en este código?

En este fragmento de codigo se puede observar el contenido de un else, que es un comando que necesariamente requiere de que anterior a el , halla un if, y que este mismo sirve para que cuando el if no pueda ser ejecutado ya sea por que su condicion no se cumpla o diversos motivos mas, este mismo pase el relevo de la accion al else, el cual se ejecutara en su lugar. Dentro de el mismo se puede observar  un sout (System.out.println) el cual imprime un mensaje que en el contexto dado no se entiende, pero leyendo el programa completo si que se puede denotar su sentido, ya que este else funcionaba principalmente para cuando el dato proporcionadfo por el usuario no era coherente con el contexto de el programa en si. por lo que considero que a pesar de poderse meter en un final string para una mejor contextualizacion, este no es el problema principal de este fragmento de codigo.
Donde creo que si podria haber lugar a confusiones y dudas seria  en los valores numericos que se dan a las variables descritas, que hacen que pierdas el juego pero para alguien que no haya hecho el mismo el codigo podria llegar a ser lioso o incomprensible. Lo que se podria hacer es asignarle variables final a los numeros dados  como SIEMPRE_FALLA para el primer 0, NO_HACE_DAÑO para el segundo, y para el 1 se podria definir una que fuese EXITO_ASEGURADO. Incluso tambien se podria cambiar la variable vidaGuerrero por una tal como INFINITO, con un valor asignado que siempre asegurase la muerte de el mismo, dejando todo muchgo mas claro.

---

## Pregunta 10

Archivo: `reto-003.java` — [Ver archivo](https://github.com/mmasias/25-26-PRG1/blob/2a6e8b6dfca704a09231d5ccc0d8dec2d30f3111/entregas/CrespoNicolas/reto-003.java) (Reto 003)

```java
        }
    }
}System.out.println("------------------------------------\n" + //
                                        "     ==========================\n" + //
                                        "   ==============================\n" + //
                                        " ==================================");
```

¿Qué observas en este código?
El error presente en este fragmento, a mi criterio es el mismo que el de el ejemplo 4, no obstante, he decidido corregir esta pregunta ya que lo considero un error garrafal que viola completamente todas las nociones impartidas en clase sobre el codigo limpio, ya que es especialmente llamativo y ensucia el codigo en grandes cantidades. El problema de este codigo es que se ha metido dentro de un sout(System.out.println) una cadena de texto que claramente deberia ser una final string ya que es algo que no cambia en ningun contexto. En este caso es utilizada para pintar el suelo de un edificio, lo que podria ser claramente representado en una variable final de nombre "PLANTA_BAJA" o algo similar que ayudase a identificarla
