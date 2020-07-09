# German XKB keyboard layout with French enhancements

The `de_fr` layout file adds the following enhancements over the `de` layout:

* The small capital `œ` letter to `<Alt Gr> + ö`
  and the capital `Œ` letter to `<Alt Gr> + <Shift> + ö`

* The small capital `ç` letter to `<Alt Gr> + c`
  and the capital `Ç` letter to `<Alt Gr> + <Shift> + c`

* Deadtilde charachters like ñ and Ñ are by default available if one enables "deadtilde"
  for example:

```bash
    setxkbmap de deadtilde
```

  In this case the `<Alt Gr> + <+>` and then `n` will result in `ñ`
  and `<Alt Gr> + <+>` and then `<Shift> + n` will result in `Ñ` respectively.

* One not French specific change, but more like French teaching specific change is that
  `<Alt Gr> + j` will result in `≠`, which is useful for correcting assignments etc.

Installation/usage:

```bash
    cp de_fr /usr/share/X11/xkb/symbols/
    cp de /usr/share/X11/xkb/symbols/
    dpkg-reconfigure xkb-data
    setxkbmap de_fr
```

Further reading:
 * [creating-custom-keyboard-layouts-x11-using-xkb](https://www.linux.com/news/creating-custom-keyboard-layouts-x11-using-xkb/)
 * [Ubuntu Custom keyboard layout definitions](https://help.ubuntu.com/community/Custom%20keyboard%20layout%20definitions)
