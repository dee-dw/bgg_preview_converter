# bgg_preview_converter
TCL Converter from the BoardGameGeek condensed preview list to CSV

## Prerequisites
1. Install Tcl: https://www.tcl.tk/software/tcltk/
2. Use Firefox (see "Known Issues" below)
3. Download the BGG Preview Converter and unzip it to some folder

## Initial Usage
1. Go to a BoardGameGeek preview list, e.g. https://boardgamegeek.com/geekpreview/6/spiel-18-preview
2. Switch to "Condensed View", e.g. https://boardgamegeek.com/geekpreview/6/spiel-18-preview?viewstyle=condensed
3. Optional: Filter your selection by clicking "View My Picks"
4. Scroll down and click "Show all"
5. Save the page as full html, e.g. as "bgg_spiel18.html", in the folder of the unzipped BGG Preview Converter
6. Open a terminal and navigate to the folder where you stored the the html and the converter
7. Call "update_bgg_preview bgg_spiel18.html > mylist.csv" (on Windows) or "./update_bgg_preview bgg_spiel18.html > mylist.csv" (on Linux)
8. Import mylist.csv in LibreOffice, OpenOffice, Excel etc., edit and save it if you like

## Next Usage
1. As steps 1 to 6 as before
2. Call "update_bgg_preview bgg_spiel18.html mylist.csv > mylist.csv" (on Windows) or "./update_bgg_preview bgg_spiel18.html mylist.csv > mylist.csv" (on Linux)
3. Import mylist.csv in LibreOffice, OpenOffice, Excel etc., edit and save it if you like

## Know Issues
* Works only with Firefox because other browsers save a different kind of html.
* Do not add or remove new columns in the csv! Do not add a comma in the Comment column in csv!

## Missing list items
* The list for 2018 shows three titles less than the BGG list. Why?
** "Alubari" and the "Azul expansion" are twice on the BGG list, so it's correct to not show them twice.
** The title "A game, wherein you blether..." is not found because the title stands on it's own in the html file. I think it's too long even for BGG. Sorry for that one missing.
