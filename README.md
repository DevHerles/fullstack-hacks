# 0. Disable a laptop's internal keyboard

```
⬢  ~
❯ xinput list
⎡ Virtual core pointer                          id=2    [master pointer  (3)]
⎜   ↳ Virtual core XTEST pointer                id=4    [slave  pointer  (2)]
⎜   ↳ Logitech K230                             id=10   [slave  pointer  (2)]
⎜   ↳ SynPS/2 Synaptics TouchPad                id=13   [slave  pointer  (2)]
⎜   ↳ TPPS/2 IBM TrackPoint                     id=14   [slave  pointer  (2)]
⎣ Virtual core keyboard                         id=3    [master keyboard (2)]
    ↳ Virtual core XTEST keyboard               id=5    [slave  keyboard (3)]
    ↳ Power Button                              id=6    [slave  keyboard (3)]
    ↳ Video Bus                                 id=7    [slave  keyboard (3)]
    ↳ Video Bus                                 id=8    [slave  keyboard (3)]
    ↳ Sleep Button                              id=9    [slave  keyboard (3)]
    ↳ Integrated Camera: Integrated C           id=11   [slave  keyboard (3)]
    ↳ AT Translated Set 2 keyboard              id=12   [slave  keyboard (3)]
    ↳ Logitech K230                             id=16   [slave  keyboard (3)]
∼ ThinkPad Extra Buttons                        id=15   [floating slave]

⬢  ~
❯ xinput float 12

⬢  ~
❯ xinput list
⎡ Virtual core pointer                          id=2    [master pointer  (3)]
⎜   ↳ Virtual core XTEST pointer                id=4    [slave  pointer  (2)]
⎜   ↳ Logitech K230                             id=10   [slave  pointer  (2)]
⎜   ↳ SynPS/2 Synaptics TouchPad                id=13   [slave  pointer  (2)]
⎜   ↳ TPPS/2 IBM TrackPoint                     id=14   [slave  pointer  (2)]
⎣ Virtual core keyboard                         id=3    [master keyboard (2)]
    ↳ Virtual core XTEST keyboard               id=5    [slave  keyboard (3)]
    ↳ Power Button                              id=6    [slave  keyboard (3)]
    ↳ Video Bus                                 id=7    [slave  keyboard (3)]
    ↳ Video Bus                                 id=8    [slave  keyboard (3)]
    ↳ Sleep Button                              id=9    [slave  keyboard (3)]
    ↳ Integrated Camera: Integrated C           id=11   [slave  keyboard (3)]
    ↳ Logitech K230                             id=16   [slave  keyboard (3)]
∼ AT Translated Set 2 keyboard                  id=12   [floating slave]
∼ ThinkPad Extra Buttons                        id=15   [floating slave]

⬢  ~
❯ xinput reattach 12 3

⬢  ~
❯ xinput list
⎡ Virtual core pointer                          id=2    [master pointer  (3)]
⎜   ↳ Virtual core XTEST pointer                id=4    [slave  pointer  (2)]
⎜   ↳ Logitech K230                             id=10   [slave  pointer  (2)]
⎜   ↳ SynPS/2 Synaptics TouchPad                id=13   [slave  pointer  (2)]
⎜   ↳ TPPS/2 IBM TrackPoint                     id=14   [slave  pointer  (2)]
⎣ Virtual core keyboard                         id=3    [master keyboard (2)]
    ↳ Virtual core XTEST keyboard               id=5    [slave  keyboard (3)]
    ↳ Power Button                              id=6    [slave  keyboard (3)]
    ↳ Video Bus                                 id=7    [slave  keyboard (3)]
    ↳ Video Bus                                 id=8    [slave  keyboard (3)]
    ↳ Sleep Button                              id=9    [slave  keyboard (3)]
    ↳ Integrated Camera: Integrated C           id=11   [slave  keyboard (3)]
    ↳ AT Translated Set 2 keyboard              id=12   [slave  keyboard (3)]
    ↳ Logitech K230                             id=16   [slave  keyboard (3)]
∼ ThinkPad Extra Buttons                        id=15   [floating slave]

⬢  ~
❯
```
