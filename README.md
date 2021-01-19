# Git på göteborgska

## Introduktion

Gren från https://github.com/ErikGartner/git-pa-skanska

Det dagliga språket för de olika kommandona i `git` (eller `gött`) är
på skånska ett enda stort skångelskakalas. Jag finner mig själv ofta
sägandes _"Kan du pusha branchen?"_ eller _"Jag pullar!"_.

Detta dokument ämnar etablera en rent ~~skånsk~~ göteborgsk jargong som kan användas
på arbetsplatsen för att med fördel undvika pressade situationer.

## Förslag

Nedan följer tabeller över verb och substantiv relaterade till git,
deras nuvarande bruk samt förslag på hur vi tillsammans kan bättra
oss.

| Verb        | Nuvarande bruk | Förslag       |
|-------------|----------------|---------------|
| init        | inita          | *jubba*       |
| clone       | klona          | möla [i sig]  |
| pull        | pulla          | dra           |
| push        | pusha          | knö           |
| fetch       | fetcha         | *pela*        |
| branch      | brancha        | *spåga*       |
| add         | adda           | *åsso*        |
| commit      | commita        | *hutta*       |
| rebase      | rebasa         | feppla        |
| merge       | merga          | mosa          |
| stash       | stasha         | svale         |
| cherry-pick | cherry-picka   | *pela päror*  |
| blame       | blamea         | bonka         |
| checkout    | checka ut      | käcka [sig]   |
| log	      | logga          | *härförleden* |
| force       | forca          | döna          |

| Substantiv   | Nuvarande bruk | Förslag      |
|--------------|----------------|--------------|
| git          | git            | gött/go      |
| repository   | repo           | tappen       |
| branch       | branch         | grenuttag    |
| merge        | merge          | mos          |
| commit       | commit         | abrovinsch   |
| push         | push           | tryck        |
| pull request | pull request   | halledönare  |
| stash        | stash          | svalen       |
| head         | headen         | hövvet       |
| remote       | remoten        | kicket       |
| origin       | origin         | bamba        |
| master       | mastern        | frölundaborg |
| dev          | deven          | fabriken     |


## Exempel

    - Kan du asa spågan jag just nimmade och prega den till github?

    - Jag spågade alldeles nyss och hutta ändringarna från min tocka där.

    - Skicka en jidder när du är färdig med klyddandet!

    - Låt oss pela päror från kagehus-spågan.

    - Hoppsan, jag råkade visst fedeprega mot kagehuset. D:

    - Jag har en drös på glytt, kan jag klydda in det i kagehuset och sedan prega himm det?

    - Nils! Du kan inte hutta och prega innan du har asat himm från kagehuset! Nu har pågarna fått en rälig klyddkonflikt!

    - Det för mycket klydd härförleden Edvard, du vet att man bara ska nimma där himma ditt ålahue!

## Exempel kommandon

```bash
# git init
fubbick jubba

# git add test.py
fubbick åsso test.py

# git commit -m "Add new features"
fubbick hutta -m "Mög"

# git remote add origin
fubbick ude åsso himma

# git push origin master
fubbick prega himma kagehus

# git pull origin
fubbick asa himma

# git merge origin/dev
fubbick klydda himma/glytt
```

## Dagligt bruk

Nedan följer en rad kommandoradskommandon för att sätta upp en skånsk
gitmiljö. Avsaknaden av skånska tecken i täcknamnen beror på en brist i git
(överväg att förbättra mjukvaran och skicka en jidder!). Följande
kommandon ändrar din `~/.gitconfig` och kommer att verka globalt.

```bash
git config --global alias.jubba init
git config --global alias.abekatta clone
git config --global alias.asa pull
git config --global alias.prega push
git config --global alias.fedeprega "push --force"
git config --global alias.pela fetch
git config --global alias.spaga branch
git config --global alias.asso add
git config --global alias.hutta commit
git config --global alias.nimma rebase
git config --global alias.klydda merge
git config --global alias.tocka stash
git config --global alias.pelaparor cherry-pick
git config --global alias.gaffla blame
git config --global alias.henka checkout
git config --global alias.härförleden log

alias fubbick=git
```

