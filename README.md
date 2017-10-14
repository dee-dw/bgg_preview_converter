# bgg_preview_converter
TCL Converter from the BoardGameGeek condensed preview list to CSV

## Initial Usage
0. Use Firefox! (see "Known Issues" below)
1. Go to a BoardGameGeek preview list, e.g. https://boardgamegeek.com/geekpreview/4/spiel-17-preview
2. Switch to "Condensed View", e.g. https://boardgamegeek.com/geekpreview/4/spiel-17-preview?viewstyle=condensed
3. Scroll down and click "Show all"
4. Save the page as html, e.g. as "bgg_codensed_view.html"
5. Call "update_bgg_preview bgg_codensed_view.html > mylist.csv"
6. Open the list in LibreOffice or OpenOffice and edit it if you like

## Next Usage
1. As steps 1 to 4 as before
2. Call "update_bgg_preview mylist.csv bgg_codensed_view.html > mylist.csv"
3. Open the list in LibreOffice or OpenOffice and edit it if you like

## Know Issues
* Non-Ascii characteres in game or pubslisher names are not supported (they will be replaced if known, otherwise an error occurs.
* works only with Firefox because othe browsers save a different kind of html
