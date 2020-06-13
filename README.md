# German XKB keyboard layout with French enhancements

The `de_fr` layout file adds the following enhancements over the `de` layout:

* The small capital œ letter to `<Alt Gr> + ö`
  and the capital Œ letter to `<Alt Gr> + <Shift> + ö`

* The small capital ç letter to `<Alt Gr> + c`
  and the capital Ç letter to `<Alt Gr> + <Shift> + c`

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
