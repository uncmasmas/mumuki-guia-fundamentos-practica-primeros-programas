Ahora que conocemos a `Poner` y `Mover`, ya estamos en condiciones de combinarlos. :hushed:

Por ejemplo el siguiente programa coloca una bolita roja en la posición inicial y una negra al este.

```puppet
program {
  Poner(Rojo)
  Mover(Este)
  Poner(Negro)
}
```

> Probá copiar y ejecutar este programa. Te mostraremos el resultado al ejecutarlo en un tablero de 2x2, y en otro de 3x2, ambos con el cabezal inicialmente en el origen.