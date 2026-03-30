# 🍽️ Restoran Jezero — Grupni projekt

**Grupa A · 4 učenika · Bootstrap završni projekt**

---

## 📋 O projektu

Izrađujete web stranicu za fiktivni restoran Jezero.
Stranica mora biti potpuno responzivna, vizualno konzistentna i deployable na GitHub Pages.

---



Ovaj projekt je **samo Bootstrap** — HTML, CSS i Bootstrap komponente.
 Sve interaktivne komponente
(modal, hamburger meni, tabovi, accordion) rade isključivo kroz
Bootstrap `data-bs-*` atribute i Bootstrap JS koji je već linkан u `index.html`.



---

## 👥 Podjela uloga i zadataka

| Uloga | Učenik | Branch | Zadatak |
|-------|--------|--------|---------|
| **Lead Developer** | *Luka Pasalic* | `feature/navigacija` + `feature/footer` | Navbar, "O nama", Footer, koordinacija tima |
| **UI Developer** | *Karlo Buljan* | `feature/hero` | Hero sekcija, vizualni identitet |
| **Content Developer** | *Viktor Cacija* | `feature/meni` | Meni sekcija s tabovima/accordionom i karticama |
| **Form Developer** | *Luka Dalic* | `feature/rezervacija` | Forma za rezervaciju, modal, validacija |

> **Napomena:** Lead Developer mergea PR-ove i rješava konflikte. Svaki član je reviewer za PR kolege do njega.

---

## 🚀 Kako početi — Git workflow

### Korak 1 — Kloniraj repo

```bash
git clone https://github.com/bozoperic/restoran-jezero.git
cd restoran-jezero
```

### Korak 2 — Napravi svoj branch

```bash
# Primjer za UI Developera:
git checkout -b feature/hero

# Provjeri jesi li na pravom branchu:
git branch
```

### Korak 3 — Radi i commita redovito

```bash
# Nakon svake logičke cjeline — commit!
git add .
git commit -m "Dodan hero naslov i dva gumba"

# Push na GitHub:
git push -u origin feature/hero
```

### Korak 4 — Otvori Pull Request

1. Idi na GitHub repo
2. Klikni **Compare & pull request**
3. Naslov PR-a: što si napravio (npr. "Dodana hero sekcija")
4. U opisu napiši što si implementirao
5. Assignee: ti, Reviewer: Lead Developer

### Korak 5 — Code review

- Lead Developer pregledava svaki PR
- Ostavlja komentare na **Files changed** tbu
- Odobrava ili traži izmjene

### Korak 6 — Sync s mainom

Redovito povlači promjene kolega u svoj branch:

```bash
git checkout main
git pull
git checkout feature/tvoj-branch
git merge main
```

---

## ⚠️ Pravila rada

1. **Nikad direktno na main** — sve kroz brancheve i PR-ove
2. **Commit poruke moraju biti opisne** — `"promjene"` nije prihvatljivo
3. **Minimalno jedan commit po radnom satu** — ne gomilaj sve na kraj
4. **Svaki PR mora imati review** — Lead Developer odobrava prije mergea
5. **Konflikti** — rješavaju se zajedno, Lead Developer koordinira

---

## 📁 Struktura projekta

```
restoran-stara-carsija/
├── index.html          ← glavna stranica
├── css/
│   └── style.css       ← custom stilovi (ne dirај bootstrap!)
├── img/                ← slike (koristite picsum.photos ako nemate vlastite)
└── README.md
```

---

## ✅ Zahtjevi projekta — što mora biti implementirano

### Obavezno (za prolaz):
- [ ] Responzivni navbar s hamburger menijem
- [ ] Hero sekcija (min-height 90vh)
- [ ] Meni s min. 9 stavki u karticama (3 kategorije × 3)
- [ ] Forma za rezervaciju s min. 5 polja
- [ ] Modal (otvara se s najmanje 2 mjesta na stranici)
- [ ] Footer s adresom i radnim vremenom
- [ ] Custom CSS (promijenjena boja i font)
- [ ] Responzivno na 375px (testirano u DevToolsu)
- [ ] Minimalno 8 commitova po osobi
- [ ] Svi PR-ovi kroz review

### Bonus (samo Bootstrap, bez JS):
- [ ] Bootstrap nav-tabs za kategorije menija
- [ ] Validacijske klase na formi (`is-valid` / `is-invalid`)
- [ ] Accordion za FAQ (pitanja o rezervaciji, alergeni...)
- [ ] Google Maps embed u footeru (`<iframe>`)
- [ ] Hover efekt na karticama menija (CSS `transition` u `style.css`)

---

## 🗓️ Vremenski okvir

| Faza | Što | Rok |
|------|-----|-----|
| Setup | Clone, branch, prvi commit | Sat 1, prvih 15 min |
| Razvoj | Svaki na svom dijelu | Sat 1 + Sat 2 |
| Integracija | PR-ovi, review, merge | Zadnjih 30 min |
| Prezentacija | Demo pred razredom | Kraj sata |

---

## 🎨 Smjernice dizajna

- **Paleta:** tople, zemljane boje (bordo, zlatna, krem, tamno smeđa)
- **Fontovi:** Playfair Display (naslovi) + Lato (tijelo) — već učitani u CSS-u
- **Stil:** elegantan, topao, tradicionalan bosanski ugođaj
- **Slike:** `https://picsum.photos/seed/[naziv]/400/300` za placeholder

---

*Projekt se predaje kao GitHub repo link. README mora biti popunjen imenima.*
