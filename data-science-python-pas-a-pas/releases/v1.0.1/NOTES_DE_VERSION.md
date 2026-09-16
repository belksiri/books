# Data science avec Python, pas à pas — ressources du lecteur v1.0.1

Première version publique des ressources du livre de **Belk Siri**.

## Téléchargement

| Fichier | Taille | SHA-256 |
|---|---:|---|
| `Ressources_Lecteur_v1.0.1.zip` | 541 Ko | `f63cdf2b4cb0306e46371ec24c01ce584013ca088e6b2ea5f70c5596fec6eb0e` |
| `Ressources_Lecteur_v1.0.1.zip.sha256` | — | empreinte au format `shasum` |

## Contenu

- Données du projet fictif SmartMarket : export brut (6 120 lignes),
  fichier propre (6 000 clients), 800 clients à scorer sans cibles,
  dictionnaires et manifeste des empreintes.
- 26 notebooks de cours, 5 notebooks d'annexes et 34 notebooks d'énoncés
  d'exercices et de défis, sans sorties.
- Code du projet (`src/smartmarket/`), tests, script de vérification pour
  Windows, `requirements.txt` et `pyproject.toml`.

Les corrigés et les fichiers de vérité des données ne sont pas inclus :
ils sont distribués séparément.

## Installation

Python **3.12, 3.13 ou 3.14**.

```bash
python3 -m venv .venv
source .venv/bin/activate          # Windows : .venv\Scripts\Activate.ps1
python -m pip install -r requirements.txt
python -m pip install -e .
python -m smartmarket.verifier_environnement
```

Guide complet : [GUIDE_INSTALLATION.md](https://github.com/belksiri/books/blob/main/data-science-python-pas-a-pas/documentation/GUIDE_INSTALLATION.md).

## Vérifications effectuées

Sur une extraction neuve de cette archive, sous macOS avec Python 3.14.6 :
installation des versions figées, diagnostic, 14 tests réussis et
exécution sans erreur des 65 notebooks. Compatibilité Windows préparée et
revue statiquement, mais non validée sur une machine Windows.

## Signaler un problème

[Ouvrir une issue](https://github.com/belksiri/books/issues/new?template=probleme_ressources.md).
