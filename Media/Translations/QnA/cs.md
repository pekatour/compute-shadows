## Jaký je smysl tohodle title packu?
Kdykoli chcete přepočítat stíny map ze starých verzí ManiaPlanet, nebo převést Stadium tratě ze starších Trackmania verzí, tento title pack to dokáže vyřešit jednoduše a hromadně.

## Co je to MapType?
Je to speciální skript, který ti říká, jestli je mapa správně postavená. Mapy, které nesplňují požadavky, jsou zakázány hrou k použití v singleplayeru nebo multiplayeru.

## Proč vůbec MapType?
Tato vlastnost byla přidána hlavně z důvodu převodu Platform, Stunt a Puzzle map z TM1 do ManiaPlanet, ale lze ji použít i v mnoha dalších případech. Například zhratelnit mapy které ztratily svůj MapType atd.

## Jak použít tento nástroj?
Prvně je potřeba specifikovat složku, kde jsou tvé mapy, relativně k složce Maps/. Můžeš toto políčko také nechat prázdné pokud chceš vypočítat stíny pro všechny mapy. Dále můžeš dodatečně specifikovat MapType, který se použije pro všechny vypočítané mapy, nebo naopak vypnout tuto vlastnost malou fajfkou v horním rohu. Teď už jsi připraven začít kliknutím na Vypočítat to všechno.
K přerušení nástroje, v menu klikni na tlačítko Přerušit. Máš 2 sekundy na kliknutí než začně další výpočet. Pokud jsi uprostřed výpočtu, můžeš jednoduše kliknout na tlačítko Zpět (nic se tím nerozbije) a budeš přesunut zpět do menu k tlačítku Přerušit. **Poznámka: Stíny nebudou vypočítány, ale MapType se přesto změní.**

## Jaké jsou přesné problémy vypnutí ukládání již vypočítaných map?
Předchozí soubor mapy obsahující vypočítané stíny může občas být nahrazen souborem bez uložených stínů, což může věci naopak pro uživatele prodloužit v porovnání s manuální prácí. Nicméně vypnutí této možnosti udělá nástroj použitelný pro masivní změny MapTypů a podobné věcí. Každopádně pro bezpečnost nech zapnuto, zálohování map doporučuji.

## Jak je to lepší než /calculateallshadows?
Máš pravdu, /calcualteallshadows něco umí, ale nemáš žádnou kontrolu nebo ponětí, co se právě vypočítává. Dříve jsi funkci tohodle title packu mohl replikovat tímto způsobem s pár dalšími příkazy, ale od MP4.1, většinu těchto příkazů přestalo fungovat.

## Všiml jsem si, že stíny mapy nejsou vypočítaný na Vysoké, ale Základní. Proč tomu tak je?
Tohle se provedlo z technických důvodů.
Pokud vypočítáš stíny na vyšší než Základní, lightmapy nejsou uloženy do souboru mapy, ale jen do tvé mezipaměti, což znamená, že ostatní lidé neuvidí vypočítané stíny.
Pokud chceš vypočítat stíny na nejvyšší, doporučuju to udělat odděleně jen pro mapy, kde to opravdu potřebuješ.

## Moje mapy používají jiný MapType než Race. Co mám udělat, aby zůstal na všech mapách stejnej MapType?
V nástroji v kroku MapType klikni na malou fajfku v horním rohu. Tímhle se vypne tato vlastnost. Lze ji znovu zapnout dalším klikem.

## Převedl jsem Stadium mapu z TM1, ale několik bloků z ničeho nic zmizelo. Proč?
Taky si nejsem úplně jistý, ale považuji to za bug ManiaPlanet enginu, stávající se hlavně se skulptury. Stejná věc by se stala pokud by jsi převedl tu mapu manuálně.
Aktuálně se pro to snažím najít řešení. Zatím nemáš jinou možnost než zmizlý bloky položit manuálně.

## Minimalizoval jsem hru, ale výpočet se nikam neposunul když jsem se podíval. Proč se to prostě zastavilo?
Když klikneš nahoře na tlačítko minimalizace, všechny skripty, které řeší výpočty, se zmrazí. Musíš zmáčknout Alt+Tab nebo přejít ze hry bez skutečné minimalizace.

## Po výpočtech jsou velikosti map hodně malé, pěkně! Je to ale v pohodě?
Ne, to skutečně není. Stíny nebyly uloženy do souboru mapy. Tohle se často stává když mapy byly už v minulosti vypočítány. Podívej se do mezipaměti hry v ProgramData/ManiaPlanet/Cache a odstraň lightmap soubory (.Bump.LightMap.zip). Měly by být označeny jako novější. Pokud si nejsi jist, můžeš vyčistit celou mezipamět v nastavení ManiaPlanet, což bude fungovat stoprocentně.