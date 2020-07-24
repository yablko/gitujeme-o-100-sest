# Git / GitHub od základov

Môj kurz **Git / GitHub od základov 🇸🇰** nájdeš [celý zdarma na youtube](http://robweb.sk).
Toto sú príkazy, ktoré ukazujem a podrobne vysvetľujem v kurze.

---

### INŠTALÁCIA

Pre Windows odporúčam [cmder](https://cmder.net/).

Na Macu spusti prvý príkaz cez Terminál a mal by sa nainštalovať Git.
Ak nie, spusti druhý príkaz.

```
git --version
xcode-select --install
```

Ak sa nedarí (alebo máš Linux), nainštaluj [odtiaľto](https://git-scm.com/download/).

---

### GIT NASTAVENIA

Otestuj, či ho máš nainštalovaný.

```
git --version
```

Nastav meno a heslo (ak používaš Github, _použi github údaje_).

```
git config --global user.name "tvojemeno"
git config --global user.email "tvoj@email.hu"
```

---

### GIT ZÁKLADY

Aktivuj git pre projekt.

```
git init
```

Over stav / pozri, čo sa zmenilo.

```
git status
```

Ak spravíš zmenu v súbore, **a chceš ho v novej verzii projektu**, označ ho.

```
git add index.html
```

Vytesaj zmenu do kameňa. **Vždy pridaj stručný popis zmeny.**

```
git commit -m "pridal som index.html"
```

Pozri si vývoj projektu.

```
git log
```
