[README-GRATIS-LIDL-PRISER.md](https://github.com/user-attachments/files/33960181/README-GRATIS-LIDL-PRISER.md)
# Veckokassen – kostnadsfri Lidl-budget

Den här versionen kräver ingen API-nyckel och inget abonnemang. Den använder en inbyggd prislista med uppskattade Lidl-normalpriser och vanliga förpackningsstorlekar för ingredienserna i appens recept.

## Vad den gör
- Förifyller pris per förpackning och förpackningsstorlek.
- Beräknar antal hela förpackningar för inköpslistans sammanlagda mängder.
- Räknar inköpskostnad när måttenheter kan konverteras säkert.
- Låter dig ändra priser och förpackningsstorlekar när du ser riktiga priser i din butik.
- Märker normalpriserna som uppskattningar, inte liveverifierade priser.

## Installera
1. Packa upp ZIP-filen.
2. Öppna https://github.com/estech1995/Veckokassen
3. Ersätt `index.html` och `service-worker.js`. Behåll manifest och ikoner om dina nuvarande redan fungerar.
4. Commit/pusha och vänta på GitHub Pages.
5. Öppna https://estech1995.github.io/Veckokassen/

## Begränsning
Lidl publicerar offentliga reklamblad och produktkategorier, men inte ett stabilt komplett flöde med alla ordinarie priser som vi säkert kan läsa automatiskt utan API. Den inbyggda prislistan är därför en praktisk startuppskattning. Den ska kalibreras mot din lokala butik. Veckans erbjudanden kan skilja sig från normalpriserna.

Några exempel på offentliga Lidl-källor:
- https://www.lidl.se/c/reklamblad/s10018018
- https://www.lidl.se/c/lidl-plus-erbjudanden/a10105849
