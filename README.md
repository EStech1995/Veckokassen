[README.md](https://github.com/user-attachments/files/33960637/README.md)
# Veckokassen – Primat/Lidl-integration

## Aktivera
1. Besök https://primat.nu/data och skapa en API-nyckel. Använd en **publishable** nyckel (`primat_pk_…`), aldrig en hemlig `primat_live_…`-nyckel i webbläsaren.
2. Begränsa nyckeln till origin `https://estech1995.github.io`.
3. I GitHub-repot `estech1995/Veckokassen`, ersätt `index.html` och `service-worker.js` med dessa filer. Behåll befintligt manifest och ikoner om de redan fungerar.
4. Commit/pusha och vänta tills GitHub Pages publicerat.
5. Öppna https://estech1995.github.io/Veckokassen/ → Inställningar → klistra in nyckeln och ort/postnummer → Spara API-inställningar.
6. Gå till Inköpslista & priser → Hämta Lidl-priser.

## Vad det gör / begränsningar
Söker produktpris för varje ingrediens via Primat och visar produktnamn, pris per förpackning, eventuell förpackningsstorlek, senast bekräftat datum och källänk. Det lägger inte automatiskt ihop dessa förpackningspriser till veckans kostnad eftersom en säker beräkning måste matcha receptens gram/ml/st med produktens storlek. Befintliga kostnadsuppskattningar är fortfarande uppskattningar.

Primats aktuella villkor och priser finns på https://primat.nu/data och https://primat.nu/villkor. Gratisnivån kräver synlig attribution till primat.nu; app-planen anges till 249 kr/månad exklusive moms efter en 30-dagars provperiod. Kontrollera villkoren innan du startar en eventuell provperiod.
