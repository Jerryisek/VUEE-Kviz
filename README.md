# Energetika — přehled ke zkoušce

Interaktivní kartičky a kvíz ke zkoušce z elektroenergetiky (FEI VŠB-TUO).
Jeden samostatný soubor (`index.html`), žádný server, žádné závislosti —
funguje i offline po stažení.

- **138 otázek** z 8 kapitol (obecně, tepelné elektrárny, jaderné, vodní,
  OZE, elektrická část elektráren, elektrotepelná technika, světelná
  technika), sloučeno a zbaveno duplicit ze dvou zdrojových materiálů.
- **25 vložených diagramů/schémat** přímo v kartičkách.
- **Kartičky** — otočení karty, filtr podle kapitoly, označení
  umím / ještě ne.
- **Kvíz** — pokrývá všech 138 otázek. Tam, kde má otázka jednoznačnou
  faktickou odpověď, je to výběr ze 4 možností. Tam, kde je odpověď
  popisná / výčtová / vzorcová, je to samo-test (zobrazíš odpověď a sám/sama
  vyhodnotíš, jestli jsi to věděl/a) — místo vymýšlení nespolehlivých
  falešných možností ke složitým technickým odpovědím.
- **Postup se ukládá v prohlížeči** (localStorage) — po zavření nebo
  refreshi zůstane zachovaný.

## Jak si to spustit

**Nejjednodušší:** stáhni `index.html` a otevři ho dvojklikem v prohlížeči.
Nic dalšího není potřeba.

**Jako web (GitHub Pages)**, aby na to šel poslat odkaz:

1. Na GitHubu vytvoř nový repozitář (např. `energetika-kviz`).
2. Nahraj do něj tento `index.html` (přes "Add file → Upload files" ve
   webovém rozhraní, nebo přes git — viz níže).
3. V repozitáři jdi do **Settings → Pages**, jako zdroj vyber větev
   `main` a složku `/ (root)`, ulož.
4. Za chvíli se appka objeví na
   `https://<tvoje-uzivatelske-jmeno>.github.io/<nazev-repa>/`.

### Přes git (příkazová řádka)

```bash
git init
git add index.html README.md
git commit -m "Energetika – kartičky a kvíz"
git branch -M main
git remote add origin https://github.com/<tvoje-uzivatelske-jmeno>/energetika-kviz.git
git push -u origin main
```

Pak stejně jako výše zapni GitHub Pages v nastavení repozitáře.

## Důležité o ukládání postupu

Uložený postup ("umím / neumím") je **lokální v prohlížeči každého
člověka zvlášť** — není to sdílená databáze. Když appku pošleš nebo
nasdílíš spolužákům, každý bude mít svůj vlastní nezávislý postup
uložený jen u sebe v prohlížeči; nikdo nevidí postup nikoho jiného.
Pokud appku otevřeš v jiném prohlížeči nebo v anonymním okně, postup
se nepřenese — zůstává vázaný na konkrétní prohlížeč/zařízení.

## Obsah

Zdrojový materiál byl sloučen ze dvou dokumentů; při vzájemném rozporu
byla u dvou otázek použita fyzikálně správná verze (typ turbíny pro
velké spády — Peltonova; spektrum nízkotlaké vs. vysokotlaké sodíkové
výbojky).
