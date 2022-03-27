# Git!

https://education.github.com/git-cheat-sheet-education.pdf

## PULL

Come si clona
Git Graph
A cosa serve il pull
Extra: README.md file

esperimento:

- nuovo progetto
- clono nuovo progetto in locale
- commit su github (spiego modifica readme)
- faccio vedere su Git Graph che non ci sono modifiche
- pull sulla repo locale
- faccio vedere su Git Graph

[Markdown](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)

Quando pullare? Prima di iniziare a lavorare.

Ma anche prima di pushare!
ogni commit deve compilare (non si pushano commit con errori)

pull = fetch + merge !

## MERGE

ALTRO: come aggiungono collaboratori

esperimento:

- aggiungo nuovo utente (o altro studente)
- faccio fare una modifica al readme da github con altro utente
- modifico dal mio pc senza pullare la stessa linea
- faccio un commit
- push -> errore!!!
- merge
- modifico cancellando roba in più
- commit, push
- faccio vedere su Git Graph

ALTRO: come si identificano i commit (id e HEAD)

## BRANCH

Come fare se devo fare tante e modifiche, tipo una nuova feature del programma??
Oppure qualcosa di invasivo che fino a quando non è finito non serve agli altri?

esperimento:

- creo branch
- faccio due commit
- checkout main
- faccio commit su main
- checkout feature, checkout main
- mergio branch su main con git graph

```
git checkout master
git merge new-branch
```

Non si testa in produzione!
`dev o develop`

come mergiare una branch, meglio farlo solo sul main/develop.

```
git checkout main
git merge my-feature-branch
```

pagina 8, 17 slides!

ALTRO:
Stampa branch corrente:  
`git branch`
Crea branch:  
`git branch develop`

Crea una branch e fa checkout in quella:  
`git checkout -b my-feature-branch`

## GITHUB

Altro: contribution file

## Issue

Discussione, assegnazione, tags esempi vari

https://goodfirstissue.dev/
https://hacktoberfest.digitalocean.com/
https://www.freecodecamp.org/news/a-simple-git-guide-and-cheat-sheet-for-open-source-contributors/

## Merge request / Pull request

Come chiedere che il proprio branch venga mergiato sul progetto al mantainer

https://docs.gitlab.com/ee/user/project/merge_requests/creating_merge_requests.html

https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/incorporating-changes-from-a-pull-request/merging-a-pull-request

## Sviluppo architettura

develop branch con feature branches
su main: releases e branch di hotfix

#### Altro che potrebbe servire:

Per settare il remote branch di default: `git push -u origin main`

[Comandi di vi](https://www.redhat.com/sysadmin/introduction-vi-editor)
