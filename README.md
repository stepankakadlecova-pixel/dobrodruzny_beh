# Dobrodružný běh

Mobilní webová hra Pro malé dobrodruhy. Hlavní hra je v `index.html`; grafika a zvuk jsou v kořenovém adresáři.

## Spuštění
Otevřete přes statický webový server (např. `python3 -m http.server 8000`) a navštivte `http://localhost:8000`. Otestujte na telefonu i počítači.

## Úpravy
V `index.html` je objekt `SETTINGS` s délkou hry, rychlostí, gravitací a intervaly vytváření předmětů. Seznam `collectImages` určuje sbírané předměty a body; `obstacleImages` překážky a penalizace. Obrázky musí mít odpovídající názvy souborů.

## Ovládání
Dotyk/kliknutí do herní plochy nebo mezerník vyvolá skok. Při skrytí stránky se hra pozastaví a po návratu pokračuje. Rekord se ukládá lokálně v prohlížeči.

## Důležité před publikací
Tato verze je webová hra, **nikoli** hotová aplikace v App Store/Google Play. Výsledky uložené v prohlížeči nejsou bezpečným podkladem pro vydávání skutečných slev, bodů ani poukazů. K tomu je nutný server s ověřováním a ochranou proti podvodům. Před vydáním ověřte všechny obrázky, mobilní ovládání, přístupnost a licence použitých souborů.

## Vývojový postup
Změny připravujte v samostatných větvích a kontrolujte přes pull request. Zachovejte funkční `main`. Doporučené další kroky: oddělit CSS/JS, přidat automatické testy, PWA podporu a až potom mobilní balíčky.
