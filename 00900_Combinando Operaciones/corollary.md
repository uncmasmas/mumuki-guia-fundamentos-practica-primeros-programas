Ahora que combinamos operaciones, la cosa se pone un poco mas complicada, porque hay que tener **más cuidado con el orden**.

Por ejemplo, mirá el programa que escribiste:

```puppet
program {
  Poner(Rojo)
  Mover(Este)
  Poner(Negro)
  Mover(Norte)
  Poner(Verde)
}
```

Operacionalmente:

1. pone una roja
1. luego se mueve al este
1. luego pone una negra

Es decir: pone una roja el la posicion inicial, y una negra al este

Y ahora mirá este otro:

```puppet
program {
  Mover(Este)
  Poner(Rojo)
  Poner(Negro)
  Mover(Norte)
  Poner(Verde)
}
```

Operacionalmente:

1. se mueve al este
1. luego pone una roja
1. luego pone una negra

Es decir: pone una roja y una negra al este de la posición inicial.

Moraleja: ¡no hacen lo mismo! Cambiar el orden nos cambió el _qué_.

