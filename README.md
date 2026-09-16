# Livres de Belk Siri — ressources publiques

Ce dépôt réunit les ressources gratuites des livres de Belk Siri : données,
notebooks, énoncés d'exercices, guides d'installation et visuels de
couverture. Chaque livre occupe son propre dossier.

| Livre | Version | Page du livre |
|---|---|---|
| *Data science avec Python, pas à pas* | v1.0.1 | [https://belksiri.github.io/books/data-science-python-pas-a-pas/](https://belksiri.github.io/books/data-science-python-pas-a-pas/) |

## Organisation

```text
books/
├── README.md                 ce fichier
├── index.html                page d'accueil de la collection (GitHub Pages)
├── .github/ISSUE_TEMPLATE/   formulaire pour signaler un problème
└── data-science-python-pas-a-pas/
    ├── index.html            page stable du livre (cible du QR code)
    ├── couverture/           couverture, QR code, logo
    ├── livre/                informations sur le livre
    ├── ressources/           archive lecteur et son empreinte
    ├── checksums/            empreintes SHA-256
    ├── documentation/        guides et FAQ
    └── releases/             notes de chaque version
```

Pour ajouter un livre, crée un dossier `nom-du-livre/` avec la même
organisation, ajoute une ligne au tableau ci-dessus et une carte dans
`index.html`. Les archives sont aussi publiées dans les *Releases* sous
une étiquette propre à chaque livre (`nom-du-livre-vX.Y.Z`), pour que
deux livres puissent avoir chacun leur version 1.0.0.

## Ce que ce dépôt ne contient pas

Les corrigés, les fichiers de vérité des données et le livre lui-même ne
sont pas publiés ici. Les corrigés sont distribués séparément.

## Signaler un problème

Ouvre une *issue* : [https://github.com/belksiri/books/issues/new?template=probleme_ressources.md](https://github.com/belksiri/books/issues/new?template=probleme_ressources.md). Indique le livre, la
version des ressources, ton système (macOS, Windows, Linux), ta version de
Python, la commande lancée et le message d'erreur complet.
