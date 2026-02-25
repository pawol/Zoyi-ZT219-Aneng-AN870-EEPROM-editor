# Zoyi ZT219 / Aneng AN870 EEPROM Editor (forked by pawol)

Zoyi ZT219 / Aneng AN870 EEPROM Editor written in client-side JavaScript embedded in a single HTML page, fully offline.

![editor_screenshot](doc/editor_screenshot.png)

This editor works fully offline. You can download [the editor file](src/index.html) and just open it locally in a browser on your computer (in a modern browser).


## Inner workings

This project was created to alleviate the pain of hand-editing the hex dump and to explore contemporary JavaScript syntax along with API supported by the modern Chrome browser (other browsers not tested - pull requests fixing possible issues are welcomed!).

Should you notice any errors, want to add missing range, update the description, etc. feel free to open an issue or submit a pull request.

It should be rather easy task to modify the source code to support any other `EEPROM` - the page is generated dynamically based on [the `bin_ranges` variable]

### Hardware improvements

I suggest to introduce some hardware modifications.
The most important is to replace existing transil 6,8V onto 5 diodes bridge to ensure better protection of 1 ohm shunt in case of accidential connection of ammeter (200mA range)
directly into 230 VAC socket. The bridge does not impact a measurement precision on uA and mA range.  Capacitors improve readout stability.

![hardware_mods](doc/Aneng_AN870_mods.jpg)

