# Git / GitHub od základov

Môj kurz **Git / GitHub od základov 🇸🇰** nájdeš [celý zdarma na youtube](http://robweb.sk).  
Ak ma chceš podporiť (a taktiež mocne potešiť) môžeš [cez patreon](https://www.patreon.com/yablko).  
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

Označ všetky z tohoto adresára (okrem vymazaných súborov).

```
git add .
```

Označ všetky z tohoto adresára (vrátane vymazaných súborov).  
  
```
git add -A
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

### AKO VYPNÚŤ VIM;)

```
- stlač "i"
- napíš text
- esc
- :wq
- enter
- ;)
```

A šípky **hore/dole** a **q**, ak git log je pridhlý.

---

### REMOTE SERVER (GitHub v mojom prípade) GIT PUSH/PULL

Naklonuj projekt do adresára **hemingway**.

```
git clone https://github.com/yablko/hemingwayovatoro-rotator.git hemingway
```

Vytvor odkaz na externý server (resp. konkrétny repozitár).

```
git remote add origin https://github.com/ty/odkaz-na-tvoj-projekt.git
```

Natlač zmeny z tvojho počítača na server. (Zadaj github meno/heslo.)

```
git push origin master
```

Naťahaj zmeny zo servera do tvojho počítača.

```
git pull origin master
```

Čekni, či na serveri nenastali zmeny.

```
git remote update
git status
```

Plus mínus aké zmeny to boli?

```
git whatchanged origin/master -n 1
```

---

### GIT KONFLIKT !!!

Pozri si kurz;)

---

### GIT VO VISUAL STUDIO CODE

Pozri si kurz;)

---

### GIT BRANCH/MERGE (rozvetvi sa)

Ak robíš **bugfix**, sprav si **bugfix vetvu**. Ak robíš novú **login** fičúru, sprav si **login vetvu**.

```
git branch login
```

Prepni sa do novej login vetvy. Commity o logine rob do nej.

```
git checkout login
```

Vytvor a _okamžite sa prepni_ do novej bugfix vetvy. Commity o bugixerob rob do nej.

```
git checkout -b bugfix
```

Keď máš login fičúru hotovú, prepni sa do hlavnej vetvy.

```
git checkout master
```

A zlúč zmeny z loginu do nej.

```
git merge login
```

Ak chceš nevedieť, kde ti hlava stojí, prečítaj si o [merge vs rebase](https://www.atlassian.com/git/tutorials/merging-vs-rebasing).

---

### CHEAT SHEETS

- https://github.github.com/training-kit/downloads/github-git-cheat-sheet.pdf  
- https://www.atlassian.com/git/tutorials/atlassian-git-cheatsheet  
- https://www.git-tower.com/blog/git-cheat-sheet/  
- https://devhints.io/git-tricks  

---

### ODKAZY Z KURZU, BIBLIOGRAFIA

GIT  
:: https://git-scm.com/  

GIT OFICIÁLNY ONLINE BOOK  
:: https://git-scm.com/book/en/v2  

GIT OFICIÁLNE VIDEÁ  
:: https://git-scm.com/videos  

OFICIÁLNY CHEAT SHEET (pdf)  
:: https://github.github.com/training-kit/downloads/github-git-cheat-sheet.pdf  

CAMBRIDGE Lecture 6: Version Control (git) (2020)  
:: https://www.youtube.com/watch?v=2sjqTHE0zok  

---

GIT KRAKEN  
:: https://www.gitkraken.com  

SUBLIME MERGE  
:: https://www.sublimemerge.com   
   
GITLAB    
:: https://about.gitlab.com  

BITBUCKET  
:: https://bitbucket.org/product  

---

GITHUB TRENDING  
:: https://github.com/trending  

HEMINGWAYOVÁTORO-ROTÁTOR™  
:: https://github.com/yablko/hemingwayovatoro-rotator  
  
---
    
HYPER (Mac terminal)  
:: https://hyper.is/  

CMDER (pre Win)  
:: https://cmder.net/  

GIT INŠTALÁTOR  
:: https://git-scm.com/book/en/v2/Getting-Started-Installing-Git  

---

Using Version Control in VS Code  
:: https://code.visualstudio.com/Docs/editor/versioncontrol  

Git version control in VS Code (VIDEO)   
:: https://code.visualstudio.com/docs/introvideos/versioncontrol  

How to use Git Integration in Visual Studio Code  
:: https://www.digitalocean.com/community/tutorials/how-to-use-git-integration-in-visual-studio-code  

---

MERGE vs REBASE  
:: https://www.atlassian.com/git/tutorials/merging-vs-rebasing  
:: https://derekgourlay.com/blog/git-when-to-merge-vs-when-to-rebase/  
:: https://www.reddit.com/r/git/comments/56ie0x/git_fastforward_merge_vs_git_rebase_same_thing/  

---

.gitignore  
:: https://git-scm.com/docs/gitignore  
:: https://www.atlassian.com/git/tutorials/saving-changes/gitignore  
:: https://docs.github.com/en/github/using-git/ignoring-files  

.gitignore GENERÁTOR  
:: https://www.toptal.com/developers/gitignore  

---

MARKDOWN SYNTAX  
:: https://www.markdownguide.org/basic-syntax  
:: https://daringfireball.net/projects/markdown/syntax   
