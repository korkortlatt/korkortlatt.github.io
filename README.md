# KörkortLätt – publika sidor

Statiska sidor för App Store: integritetspolicy och support.
Inga byggsteg, inga beroenden. Filerna är fristående HTML.

## Publicera med GitHub Pages

Innehållet i den här mappen ska ligga i **roten** på ett publikt repo.

1. Skapa ett publikt repo på appens GitHub-konto.
2. Kopiera in allt i den här mappen (inklusive `.nojekyll`).
3. Settings → Pages → Source: `Deploy from a branch`, branch `main`, mapp `/ (root)`.

`.nojekyll` finns för att GitHub annars kör filerna genom Jekyll, som ignorerar
filer och mappar som börjar med understreck.

## Om sidorna ändras

Källtexterna ligger i `docs/*.md` i appens repo. HTML:en genererades från dem.
Ändrar du en policy, ändra markdown-filen först så att de inte glider isär.

## Egen domän senare

Lägg en fil `CNAME` i roten med domännamnet och peka DNS mot GitHub Pages.
URL:erna i appen finns i `KorkortLatt/ReleaseConfiguration.swift` och måste
uppdateras samtidigt.
