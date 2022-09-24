# eestec.etf.rs
## Uvod
GH repo za sajt LK Beograda.
## Setup
Opredelili smo se da radimo front-end u Vue.js-u, i back-end u Laravelu, ali za početak ćemo se samo baviti front delom dok se sve potrebne stranice ne postave.

Kada sredite sve da bi pokrenuli Vue.js, potrebno je da skinete repozitorijum kloniranjem git-a sa:

```sh
git clone https://github.com/EESTEC-LC-Belgrade/eestec.etf.rs
``` 

Kad se zavrsi clone, predjete u direktorijum projekta sa:

```sh
cd eestec.etf.rs
```

Buildujete i pokrenete projekat sa ulaskom u front-end sa:

```sh
cd front-end
npm run serve
```

Ukoliko se pojavi greska Error: Cannot find module '@vue/cli-plugin-babel' potrebno je da se iskuca:

```sh
npm install @babel/core @babel/preset-env
```

Prilikom push-ovanja potrebno je da se napravi novi branch i da se nakon toga ta grana push-uje sa sledećim komandama:

```sh
git checkout -b imeGrane
git add .
git status
git commit -m "tekst poruke"
git push --set-upstream origin imeGrane
```

I to je manje vise to. Happy coding :)
