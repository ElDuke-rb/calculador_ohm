# calculador_ohm

Esta aplicación está echa para apoyar con los cálculos que se requieran hacer en electricidad relacionados con la **Ley de Ohm**, esto de manera amigable y a la vez eficiente para que el usuario pueda con confianza apoyarse de esta.

## ¿Qué es la Ley de Ohm?

La **Ley de Ohm** estudia la interacción en un circuito eléctrico entre la corriente, la resistencia y el voltaje, ya que al modificar una de las tres, las otras dos reaccionan también. Esta ley consta de tres fórmulas para calcular cada elemento eléctrico.

1. V = I × R (Voltaje = Corriente × Resistencia)
2. I = V / R (Corriente = Voltaje / Resistencia)
3. R = V / I (Resistencia = Voltaje / Corriente)

donde:

- **Voltaje:** Es la diferencia de potencial eléctrico que "impulsa" la corriente a través del circuito (se mide en voltios).
- **Resistencia:** Es la oposición al paso de la corriente que tienen ciertos materiales (se mide en ohmios).
- **Intensidad de corriente:** Cantidad de corriente que pasa por un punto en una unidad de tiempo (se mide en amperios)

## Requerimientos

Para ejecutar esta aplicación es requerido tener Ruby instalado, para verificar si se tiene instalada alguna de sus versiones, se puede ejecutar el siguiente comando en la una terminal:

```bash
ruby --version
```

Si se tiene alguna versión instalada de Ruby, se retornará algo como:

```bash
ruby 4.0.4 (2026-05-12 revision b89eb1bcbf) +PRISM [x86_64-linux]
```

En el caso contrario se debe instalar alguna versión, para esto se tienen los recursos en la siguiente ruta:

https://www.ruby-lang.org/es/downloads/

## Aplicación

El directorio de la aplicación contiene los siguientes elementos:

```bash
├── README.md
├── calcular_ohm.rb
├── main.rb
└── ui.rb
```

1. `README.md`: Es este archivo en el cual está la documentación de la aplicación.
2. `calcular_ohm.rb`: Contiene los métodos que calculan cada incógnita.
3. `main.rb`: Es el Archivo principal donde convergen todos los componentes de la aplicación.
4. `ui.rb`: contiene los elementos requeridos para interactuar con el usuario, así como la lógica para recibir y validar los datos ingresados por el usuario.

## Modo de uso

- Hay un archivo main.rb dentro del directorio que debe ser ejecutado de la siguiente manera desde una consola de comandos:

```bash
ruby main.rb
```

Al hacer esto se mostrará un menú donde el usuario deberá elegir la variable que necesita calcular:

```bash
###    Bienvenido    ###

¿Qué necesita calcular?

1 -> La intensidad
2 -> La resistencia
3 -> El voltaje
4 -> Salir

Escriba la opción y presione enter:
|
```

Al escribir el número correspondiente a lo que se desea calcular, a continuación se le solicitará los valores de las dos variables restantes, estos son requeridos para aplicar la fórmula. Por ejemplo si lo que se necesita es calcular el valor de la intensidad:

- El usuario escribiría el número `1` y dará enter.
- Lo que a continuación verá es lo siguiente:

```bash
Por favor indique los valores que se le solicitan y presione enter:

I = V / R

¿Cual es el valor del voltaje(V)?
|


¿Cual es el valor de la resistencia(R)?
|
```

- Una vez sean ingresados los dos valores, la aplicación aplicará la fórmula y mostrará al usuario el resultado:
  Suponiendo que el valor que se indicó para el voltaje fuera 3 y el valor indicado para la resistencia fuera 10.

```bash
~#~#~#~#~#~#~#~#~#~#~#~#~#~#~#~#~#~#~#~#~#~

I = 3.0 / 10.0

El valor que corresponde a I es: 0.3 amperios.

V = 3.0 voltios
R = 10.0 ohmios
I = 0.3 amperios

~#~#~#~#~#~#~#~#~#~#~#~#~#~#~#~#~#~#~#~#~#~
```

Seguido de esto se mostrará de nuevo el menú para que si el usuario requiere calcular otro valor, lo indique, de modo contrario puede ingresar el número 4 para salir:

```bash
¿Requiere realizar algún otro cálculo?

###    Bienvenido    ###

¿Qué necesita calcular?

1 -> La intensidad
2 -> La resistencia
3 -> El voltaje
4 -> Salir

Escriba la opción y presione enter:
|
```
