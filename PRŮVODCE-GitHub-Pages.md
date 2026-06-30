# Průvodce: Jak spustit web Hra-D na GitHub Pages zdarma

Tento průvodce tě provede krok za krokem od nuly až po živý web s vlastní doménou.
Celý postup zabere asi **30–45 minut**.

---

## Co budeš potřebovat

- Počítač s internetem
- E-mailová adresa
- Vlastní doména (tu už máš ✓)

---

## KROK 1 — Vytvoř si GitHub účet

1. Jdi na **https://github.com**
2. Klikni na **Sign up** (vpravo nahoře)
3. Zadej e-mail, heslo a zvol si uživatelské jméno (např. `hra-d` nebo `aneta-balikova`)
4. Potvrď e-mail

> GitHub je zdarma a budeš ho používat jako "úložiště" pro soubory webu.

---

## KROK 2 — Vytvoř nový repozitář (složku na webu)

1. Po přihlášení klikni na zelené tlačítko **New** (nebo + → New repository)
2. Vyplň:
   - **Repository name:** `hra-d` (nebo libovolný název bez mezer)
   - Vyber **Public** (veřejné — nutné pro GitHub Pages zdarma)
   - Zaškrtni **Add a README file**
3. Klikni na **Create repository**

---

## KROK 3 — Nahraj soubory webu

1. V repozitáři klikni na **Add file → Upload files**
2. Přetáhni nebo vyber **všechny soubory** z této složky:
   - `index.html`
   - `pravidla.html`
   - `mista.html`
   - `organizatori.html`
   - `videa.html`
   - `fotogalerie.html`
   - `informace.html`
   - `kontakt.html`
   - `style.css`
3. Dolů napiš popis, např. „Nahrání webu" a klikni na **Commit changes**

> Až budeš mít fotky, stejným způsobem nahraj složku `foto/` s obrázky.

---

## KROK 4 — Zapni GitHub Pages

1. V repozitáři klikni na **Settings** (nahoře)
2. V levém menu najdi sekci **Pages**
3. Pod **Branch** zvol **main** a složku **/ (root)**
4. Klikni **Save**

Za chvíli (1–2 minuty) bude web dostupný na adrese:
`https://TVOJE-UZIVATELSKE-JMENO.github.io/hra-d/`

---

## KROK 5 — Připoj vlastní doménu

### Na GitHub Pages (strana GitHub)

1. Stále v **Settings → Pages**
2. Do pole **Custom domain** zadej svou doménu, např. `www.hra-d.cz`
3. Klikni **Save**
4. GitHub vytvoří soubor `CNAME` v repozitáři automaticky

### U svého registrátora domény (strana DNS)

Přihlás se ke správci domény (kde jsi doménu koupila — např. Wedos, Forpsi, Active24...) a přidej tyto záznamy:

**Pokud chceš `www.hra-d.cz`:**
- Typ: `CNAME`
- Název: `www`
- Hodnota: `TVOJE-UZIVATELSKE-JMENO.github.io`

**Pokud chceš i samotné `hra-d.cz` (bez www), přidej 4 záznamy typu A:**
- Typ: `A`, Název: `@`, Hodnota: `185.199.108.153`
- Typ: `A`, Název: `@`, Hodnota: `185.199.109.153`
- Typ: `A`, Název: `@`, Hodnota: `185.199.110.153`
- Typ: `A`, Název: `@`, Hodnota: `185.199.111.153`

> DNS změny se mohou projevit za 1–24 hodin. Buď trpělivá!

---

## KROK 6 — Zapni HTTPS (bezpečné připojení)

1. Zpět v **Settings → Pages**
2. Zaškrtni **Enforce HTTPS**

Web bude přístupný přes zabezpečené `https://` — to je důležité pro důvěryhodnost.

---

## Jak aktualizovat web v budoucnu?

Kdykoli chceš upravit obsah:
1. Uprav soubor (např. `informace.html`) v textovém editoru (Poznámkový blok, nebo lépe Notepad++)
2. Jdi na GitHub → repozitář → **Add file → Upload files**
3. Nahraj upravený soubor
4. Potvrď změny — web se aktualizuje během minut

---

## Struktura souborů

```
hra-d/
├── index.html          ← Úvodní stránka
├── pravidla.html       ← Pravidla hry
├── mista.html          ← Zapojená místa (100 míst)
├── organizatori.html   ← Organizátoři (doplň sám)
├── videa.html          ← Videa (vložit YouTube iframe)
├── fotogalerie.html    ← Fotky (přidat složku foto/)
├── informace.html      ← Důležité informace
├── kontakt.html        ← Kontaktní stránka
├── style.css           ← Vzhled celého webu
└── foto/               ← Sem patří fotografie (složku vytvoř)
    ├── foto1.jpg
    └── foto2.jpg
```

---

## Jak upravit text na webu?

Každý `.html` soubor otevři v **Poznámkovém bloku** (nebo Notepad++).
Text na stránce je mezi HTML značkami, například:

```html
<p>Toto je odstavec textu, který vidíš na webu.</p>
<h2>Toto je nadpis</h2>
```

Uprav jen text mezi `>` a `<` — nezasahuj do samotných HTML tagů.

---

## Potřebuješ pomoc?

Kdykoli se zasekneš, obrať se na mě (Claude) — napiš mi co přesně vidíš na obrazovce a pomůžu ti.
