# Moje trke

Lični trkački kalendar za Srbiju i region. Prati šta te zanima, na šta si prijavljen i šta si istrčao — bez naloga, bez servera, bez praćenja korisnika.

Aplikacija je jedna React komponenta koja radi kao web stranica, PWA i Android aplikacija.

---

## Šta radi

**Kalendar trka**
Trke iz regiona, od septembra 2026 grupisane po mesecima. Svaka trka ima datum, mesto, podlogu i deonice sa dužinom i usponom.

| Zemlja | 
|---|---|
| Srbija | 
| Bosna i Hercegovina | 
| Severna Makedonija | 
| Crna Gora | 
| Slovenija | 

**Praćenje sezone**
Svakoj trci daješ jedan od tri statusa: `zanima me`, `prijavljen`, `istrčano`. Za istrčane upisuješ vreme i biraš koju si deonicu trčao — aplikacija računa tempo po kilometru.

**Statistika**
Broj istrčanih trka, broj prijava, ukupni kilometri i ukupan uspon. Zbiru doprinose samo trke sa upisanim vremenom.

**Filteri**
Pretraga po nazivu i mestu, podloga, zemlja, mesec, `Moja sezona` (sve označeno), `Zanima me` (samo taj status) i `Prošle trke`. Svi se kombinuju, a dugme `Poništi filtere` se pojavljuje čim je bar jedan aktivan.

**Podsetnici**
Zvonce prikazuje trke u narednih 7 dana kojima si dao status `zanima me` ili `prijavljen`. Uz dozvolu pregledača šalje i sistemsko obaveštenje, jednom po trci.

**Tvoje izmene**
Možeš dodati svoju trku sa proizvoljnim brojem deonica, i ispraviti datum, mesto ili deonice bilo koje postojeće trke. Ispravke se čuvaju odvojeno od originala, pa se dugmetom `Vrati original` poništavaju.

**Vizuelni detalj**
Svaka kartica ima generisan SVG greben čija strmina odgovara najtežoj deonici te trke. Oblik je determinističan — izvlači se iz hasha ID-ja, pa je ista trka uvek isti greben.
---
