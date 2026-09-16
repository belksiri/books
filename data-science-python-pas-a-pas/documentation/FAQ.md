# Questions fréquentes

*Data science avec Python, pas à pas* — ressources du lecteur v1.0.1.

## Faut-il le livre pour utiliser les ressources ?

Oui. Les notebooks suivent les chapitres et les énoncés renvoient au
texte du livre. Les ressources seules ne remplacent pas les explications.

## Où sont les corrigés ?

Les corrigés rédigés des exercices sont dans l'annexe G du livre. Les
notebooks corrigés exécutés et les fichiers de vérité des données forment
une archive séparée, qui n'est pas publiée dans ce dépôt.

## Le livre cite `corriges/…` après les exercices, mais ce dossier n'existe pas

C'est normal : le dossier `notebooks/corriges/` appartient à l'archive des
corrigés, distribuée séparément. Les énoncés de l'archive du lecteur
fonctionnent sans lui.

## Puis-je faire le défi de la partie VI ?

Ce défi compare les segments trouvés aux profils utilisés pour générer les
données. Ces fichiers de vérité ne sont que dans l'archive des corrigés : le
défi VI se fait avec elle.

## Quelle version de Python choisir ?

Python 3.12, 3.13 ou 3.14. Les résultats imprimés dans le livre ont été
obtenus avec Python 3.12.4 et les versions de bibliothèques de
`requirements.txt`.

## Mes chiffres diffèrent légèrement de ceux du livre

Vérifie d'abord que l'environnement virtuel est activé et que
`python -m smartmarket.verifier_environnement` se termine par
« Environnement SmartMarket prêt. ». Le diagnostic contrôle les versions
et les empreintes des données.

## Le diagnostic signale une empreinte de données différente

Un fichier de `data/` a été modifié, souvent en l'ouvrant puis en
l'enregistrant avec Excel. Décompresse de nouveau l'archive.

## Les cellules de `06_erreurs_volontaires` échouent

C'est voulu : ces cellules sont marquées `raises-exception` et montrent
comment lire une erreur.

## Les ressources fonctionnent-elles sous Windows ?

Compatibilité Windows préparée et revue statiquement, mais non validée
sur une machine Windows. Le script `scripts\verifier_windows.ps1` enchaîne
toutes les vérifications ; si l'une échoue, [signale-le](https://github.com/belksiri/books/issues/new?template=probleme_ressources.md).

## Comment savoir si une nouvelle version existe ?

La [page du livre](https://belksiri.github.io/books/data-science-python-pas-a-pas/) indique toujours la version en cours, et
chaque version est décrite dans les
[releases](https://github.com/belksiri/books/releases).

## Les données décrivent-elles de vrais clients ?

Non. SmartMarket est une entreprise fictive et les 6 000 clients ont été
générés par un programme à partir d'une graine fixe (20241231).
