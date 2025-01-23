# Wire, Busses , Signals (Schematics)
#### Wire

Schematics are logical, 1 wire in schematic =! 1 real wire

#### Bus

Bus = multiple wires bundled together

Busses must have an entry and exit point:

dat0 ----- !   <- bus entry

dat1 ----- !

                 (0) <- bus

dat0 -----^

dat1 -----^  <- bus exit

#### Signals (More common than busses)

Signals are logical named nodes

**If a signal has the same name they are connected**