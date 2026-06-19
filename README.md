# Valuneto — investor preview

Gated klikací demo Valuneto. Statická stránka, jeden soubor (`index.html`), bez build kroku.

## Nasazení (Vercel přes GitHub)
1. Zkopíruj `index.html` do rootu repa, který je napojený na Vercel
   (přepíše stávající `index.html` / rozbitý stub).
2. Commit + push → Vercel nasadí automaticky.
3. Hotovo — žádný build, žádné dependencies.

## Přístupový kód
Default: **VALUNETO26** (nezáleží na velikosti písmen).
Změníš ho v `index.html` na řádku:

```js
var ACCESS_CODE = "VALUNETO26"; // <-- zmen pristupovy kod zde
```

## Pozor — úroveň ochrany
Tohle je **client-side gate** = vizuální zámek. Stačí na to, aby náhodný
návštěvník neviděl demo, ale kdokoliv technický si otevře view-source a kód
i obsah přečte. Pokud potřebuješ reálnou ochranu, zapni navíc
**Vercel Deployment Protection** (Project → Settings → Deployment Protection,
password, server-side) a gate nech jen jako vizuální vrstvu.

Demo běží na simulovaných datech — žádné reálné účty ani platby.
