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

Ak sa nedarí, nainštaluj [odtiaľto](https://git-scm.com/download/).

---

### GIT NASTAVENIA

Otestuj, či ho máš nainštalovaný.

```
git --version
```

Nastav **meno** a **heslo** (ak používaš Github, _použi github údaje_).

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

0pakuj naveky;)

---

### KÚSOK GITU NAVYŠE

Označ všetky **.png** súbory z adresá **images**.

```
git add images/*.png
```

Označ všetky z tohoto adresára.

```
git add .
```

Ak chceš zrušiť označenie súborov.

```
git restore --staged .
```

Commitni všetky **zmenené** (nie nové) súbory.
Hneď pridaj komentár.

```
git commit -a
git commit -am "upravil som kód, a teraz je dobrý"
```

Vypimpuj log.
Daj ho na jeden riadok.

```
git log --graph --decorate --abbrev-commit --all
git log --graph --decorate --abbrev-commit --all --pretty=oneline
```

Ak uložíš **index.html**, ale pokašľal si to. A chceš sa vrátiť na verziu z gitu.

```
git checkout -- index.html
```

Cez _git log_ nájdeš hash commitu. Skopči prvých pár znakov (napr. **c10e47f**) a takto môžeš skočiť na staršiu verziu projektu.

```
git checkout c10e47f
```

Vráť sa naspať na aktuálnu verziu.

```
git checkout master
```

---
