## Jaký je smysl tohodle title packu?
Kdykoli chcete přepočítat stíny map ze starých verzí ManiaPlanet, nebo převést Stadium tratě ze starších Trackmania verzí, tento title pack to dokáže vyřešit jednoduše a hromadně.

## Proč MapType?
Tato vlastnost byla přidána hlavně z důvodu převodu Platform, Stunt a Puzzle map z TM1 do ManiaPlanet, ale lze ji použít i v mnoha dalších případech. Například zhratelnit mapy které ztratily svůj MapType atd.

## Jak použít tento nástroj?
Prvně je potřeba specifikovat složku, kde jsou tvé mapy, relativně k složce Maps/. Můžeš toto políčko také nechat prázdné pokud chceš vypočítat stíny pro všechny mapy. Dále můžeš dodatečně specifikovat MapType, který se použije pro všechny vypočítané mapy, nebo naopak vypnout tuto vlastnost malou fajfkou v horním rohu. Teď už jsi připraven začít kliknutím na Vypočítat to všechno.
K přerušení nástroje, v menu klikni na tlačítko Přerušit. Máš 2 sekundy na kliknutí než začně další výpočet. Pokud jsi uprostřed výpočtu, můžeš jednoduše kliknout na tlačítko Zpět (nic se tím nerozbije) a budeš přesunut zpět do menu k tlačítku Přerušit. **Poznámka: Stíny nebudou vypočítány, ale MapType se přesto změní.**

## Jak je to lepší než /calculateallshadows?
Máš pravdu, /calcualteallshadows něco umí, ale nemáš žádnou kontrolu nebo ponětí, co se právě vypočítává. Dříve jsi funkci tohodle nástroje mohl replikovat tímto způsobem s pár dalšími příkazy, ale od MP4.1, většinu těchto příkazů přestalo fungovat.

## Všiml jsem si, že stíny mapy nejsou vypočítaný na Vysoké, ale Základní. Proč tomu tak je?
Tohle se provedlo z technických důvodů.
Pokud vypočítáš stíny na vyšší než Základní, lightmapy nejsou uloženy do souboru mapy, ale jen do tvé mezipaměti, což znamená, že ostatní lidé neuvidí vypočítané stíny.
Pokud chceš vypočítat stíny na nejvyšší, doporučuju to udělat odděleně jen pro mapy, kde to opravdu potřebuješ.

## Moje mapy používají jiný MapType než Race. Co mám udělat, aby zůstal na všech mapách stejnej MapType?
V nástroji v kroku MapType klikni na malou fajfku v horním rohu. Tímhle se vypne tato vlastnost.

## I converted a Stadium map from TM1, but several blocks suddently dissapeared. Why?
I'm not exactly sure either, but I consider this as a ManiaPlanet bug, happening especially with sculptures. Same thing would happen if you convert the maps manually.
Currently, I'm trying to find a solution for this. For now, you have no other option than to place them manually.

## I minimized the game, but moved nowhere in the calculation when I checked. Why it just stopped?
When you click on the minimize button at the top, all of the scripts that do the calculation freeze. You have to Alt+Tab or switch from the game without actual minimalization.

## After calculation, the map sizes are very small, nice! It that alright though?
No, it actually is not. The shadows weren't saved to the map file. This usually happens when the maps were already calculated in the past. Check your cache in ProgramData/ManiaPlanet/Cache and remove the lightmap files. They should be one of the newest. If you're not sure, you can clear the whole cache in ManiaPlanet settings, which will do just fine.