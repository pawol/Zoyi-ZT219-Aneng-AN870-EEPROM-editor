# Zoyi ZT219 / Aneng AN870 EEPROM Editor (by pawol)

Zoyi ZT219 / Aneng AN870 EEPROM Editor written in client-side JavaScript embedded in a single HTML page, fully offline.

![UT210E Editor Screenshot 01](doc/editor_screenshot.png)

This editor works fully offline. You can download [the editor file](src/index.html) and open it in a browser from your computer (in a modern browser), no server is required.


## Inner workings

This project was created to alleviate the pain of hand-editing the hex dump and to explore contemporary JavaScript syntax along with API supported by the modern Chrome browser (other browsers not tested - pull requests fixing possible issues are welcomed!).

Should you notice any errors, want to add missing range, update the description, etc. feel free to open an issue or submit a pull request.

It should be rather easy task to modify the source code to support any other `EEPROM` - the page is generated dynamically based on [the `bin_ranges` variable]
