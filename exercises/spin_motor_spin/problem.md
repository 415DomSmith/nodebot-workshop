__Attach a motor to pin 9 and start it spinning!__

* Spin the motor at **200** mph
* Use `board.wait` to stop the motor spinning after **2 seconds**
* Start it spinning again after another second
* Ensure this loop repeats infinitely

note : we will use a bjt npn type transistor for this circuit, they are common in starter kits (P2N2222AG, BC547), other type of transistor exists but may require different wiring.

Hint: You could use the motor `start` and `stop` events to stop/start the motor.

check what type of transistor you have by googleling it's reference.

## Circuit diagram

```
                     ----o  GND
                     |
            330    |>
Pin 9  o---/\/\/---|   NPN Transistor
                   |\
                     |
                     |
               ------.
               |     |
               |     _
               |    / \
        Diode  v   ( o )  Motor
               -    \_/
               |     |
               |     |
   +5  o-------.------
```

## Components

- Motor - http://node-ardx.org/electronics-primer#dcmotor
- bjt npn transistor - http://node-ardx.org/electronics-primer#transistor

> Spins when a current is passed through it.

## Docs

- Board - https://github.com/rwaldron/johnny-five/wiki/Board#api
- Motor - https://github.com/rwaldron/johnny-five/wiki/Motor#api

---