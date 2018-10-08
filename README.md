# bgg_preview_converter
TCL Converter from the BoardGameGeek condensed preview list to CSV

## Initial Usage
0. Use Firefox! (see "Known Issues" below)
1. Go to a BoardGameGeek preview list, e.g. https://boardgamegeek.com/geekpreview/6/spiel-18-preview
2. Switch to "Condensed View", e.g. https://boardgamegeek.com/geekpreview/6/spiel-18-preview?viewstyle=condensed
3. Filter your selection by clicking "View My Picks"
4. Scroll down and click "Show all"
5. Save the page as full html, e.g. as "bgg_spiel18.html"
6. Call "update_bgg_preview bgg_spiel18.html > mylist.csv"
7. Open the list in LibreOffice, OpenOffice, Excel etc. and edit it if you like

## Next Usage
1. As steps 1 to 5 as before
2. Call "update_bgg_preview bgg_spiel18.html mylist.csv > mylist.csv"
3. Open the list in LibreOffice, OpenOffice, Excel etc. and edit it if you like

## Know Issues
* Works only with Firefox because other browsers save a different kind of html
