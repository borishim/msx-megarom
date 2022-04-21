# msx-megarom
MSX megarom cartridge pcb (kicad)

There are three jumpers to set:
- P8: put a jumper for 8kB bank, otherwise 16kB
- P7 and P2: bank selection bits (WA and WB). Depends on the mapper type.

For example,
```
                           8kB WA  WB
                     ASC8: YES A11 A12
                    ASC16: NO  A12 0
                 Generic8: YES A13 A15
                Generic16: NO  A15 0
               Konami SCC: YES A13 A15
            Konami no SCC: YES A13 A15
Super Game World 30/64/80: YES A0  A1
            Super Pierrot: NO  A12 0
```
Also take a look https://www.msx.org/wiki/MegaROM_Mappers
