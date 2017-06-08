# Alapfogalmak

## Kommit:
Elemi egység, a fájlokról elmentett pillanatkép.
Minél gyakrabban és minél kisebb logikailag összetartozó egységet kommitoljunk
A kommitokank van gyereke és szülője.
HEAD: utolsó kommit

## Branch
Kommitok egymásutáni sorozata
(kommit pötty, branch vonal)
master: automatikusan létrejön

## Workspace
Fejlesztésben használt fájlok, ezeken dolgozunk

## Repository
Metadatok tárolása (kommitok, branchek, címkék)

# Installálás

```
apt-get install git-core git-doc git-gui gitk
```

# Help

```
git help
```

```
git help <parancs> # pl git help commit
```

# Beállítások

```
git config --global user.name "Simon Balázs"
git config --global user.email "balazs.simon@intren.hu"

git config --global color.ui auto

git config -l # lista
```

## Alias
```
  git config --global alias.co "checkout"
  git config --global alias.st "status"
```

# Init
Új git repository létrehozása
```
  git init
```

# Status
Változások listázása
```
  git status
```

# Add, mv, rm
File hozzáadása, áthelyezése, törlése
```
  git add <filename>
  git mv <oldfilename> <newfilename>
  git rm <filename>
```

# Commit  
Változások mentése
```
  git commit
  git commit -m 'commit message'
  git commit -a
```

# Log
Commitok listázása
```
  git log
```

# Diff
Változások megtekintése
```
  git diff
  git diff -w # whitespace karakterek figyelmen kívül hagyása
  git diff <oldhash>..<newhash>
  git diff <oldtag>..<newtag> # tag is használható
```

# Blame
File változások listázása
```
  git blame <filename>
```

# Tag
Címkézés (pl programverzió), kommit azonosítására (checkout, diff)
```
  git tag <cimke> # címke létrehozása
  git tag # használt címkék listázása
  git tag -d <cimke> # címke törlése
```

# Reset
Nem kommitolt módosítás eldobása
```
  git reset --hard
```
Kommit törlése
```
  git reset --hard <hash>
```
