[README-LIDL.md](https://github.com/user-attachments/files/33959486/README-LIDL.md)
# Veckokassen – Lidl-erbjudanden

## Viktigt
Den här versionen kan visa verifierade erbjudanden från `offers.json`, men den hämtar **inte** automatiskt priser från Lidl. Jag har inte lagt in påhittade priser eller byggt en scraper mot en källa vars villkor inte är bekräftade.

## Lägg in kontrollerade erbjudanden
1. Öppna Lidls officiella erbjudandesida: https://www.lidl.se/c/erbjudanden/s10017738
2. Kontrollera produkt, pris, enhet och datum för din butik/region.
3. Redigera `offers.json` i GitHub och lägg till produkter i `offers`.
4. Spara ändringen. GitHub Pages publicerar filen tillsammans med appen.

Exempel på format (ersätt med ett faktiskt kontrollerat erbjudande):

```json
{
  "store": "Lidl",
  "updatedAt": "2026-10-26",
  "source": "Lidls officiella erbjudandesida",
  "offers": [
    {
      "name": "Produktnamn",
      "price": 19.9,
      "unit": "st",
      "validFrom": "2026-10-26",
      "validTo": "2026-11-01",
      "sourceUrl": "https://www.lidl.se/c/erbjudanden/s10017738"
    }
  ]
}
```

Datum anges som `ÅÅÅÅ-MM-DD`. Appen visar bara erbjudanden som har Lidl som butik, pris, giltighetsdatum som omfattar dagens datum och en HTTPS-källänk. Erbjudandena visas som information; de ändrar inte automatiskt totalsumman i inköpslistan. Ange pris i inköpslistan för att påverka din budget.

## Varför ingen automatisk GitHub Actions-hämtning?
En schemalagd körning kan inte skapa korrekta priser utan en stabil, tillåten och verifierbar datakälla. Att skrapa butikssidor kan vara opålitligt och kan strida mot villkor. Därför är detta en ärlig grund som inte låtsas ha livepriser. Om en officiell öppen datakälla/API blir tillgänglig kan en automatiserad uppdatering kopplas in senare.
