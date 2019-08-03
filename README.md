# bgg_preview_converter
TCL Converter from the BoardGameGeek condensed preview list to CSV

## Prerequisites
1. Install Tcl: https://www.tcl.tk/software/tcltk/
2. Use Firefox (see "Known Issues" below)
3. Download the BGG Preview Converter and unzip it to some folder

## Initial Usage
1. Go to a BoardGameGeek preview list, e.g. https://boardgamegeek.com/geekpreview/13/gen-con-2019-preview
2. Switch to "Condensed View", e.g. https://boardgamegeek.com/geekpreview/13/gen-con-2019-preview?viewstyle=condensed
3. Optional: Filter your selection, e.g. Must Have, Interested and Undecided
4. Scroll down and click "Show all"
5. Save the page as full html, e.g. as "gencon2019.html", in the folder of the unzipped BGG Preview Converter
6. Open a terminal and navigate to the folder where you stored the the html and the converter
7. Call "update_bgg_preview gencon2019.html > mylist.csv" (on Windows) or "./update_bgg_preview gencon2019.html > mylist.csv" (on Linux)
8. Import mylist.csv in LibreOffice, OpenOffice, Excel etc., edit and save it if you like

## Next Usage
1. As steps 1 to 6 as before
2. Call "update_bgg_preview gencon2019.html mylist.csv > mylist.csv" (on Windows) or "./update_bgg_preview gencon2019.html mylist.csv > mylist.csv" (on Linux)
3. Import mylist.csv in LibreOffice, OpenOffice, Excel etc., edit and save it if you like

## Know Issues
* Works only with Firefox because other browsers save a different kind of html.
* Do not add or remove new columns in the csv! Do not add a comma in the Comment column in csv!
