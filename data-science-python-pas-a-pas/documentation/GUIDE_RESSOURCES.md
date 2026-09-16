# Guide des ressources

Ressources du livre « Data science avec Python, pas à pas », de Belk
Siri, version **v1.0.1** (septembre 2026). Toutes les
données SmartMarket sont **fictives** : aucune ligne ne décrit une
personne ou une entreprise réelle.

Les ressources sont livrées en deux archives :

| Archive | Pour qui | Contenu |
|---|---|---|
| `Ressources_Lecteur_v1.0.1.zip` | lecteur | données, notebooks de cours, énoncés, code, tests, scripts |
| `Ressources_Corriges_v1.0.1.zip` | correction, formation | tout le contenu lecteur, plus corrigés, fichiers de vérité, génération et validation des données, résultats attendus |

Ce guide décrit l'archive du lecteur ; l'archive des corrigés ajoute
`GUIDE_CORRIGES.md`.

## 1. Par où commencer

| Situation | Action |
|---|---|
| Tu veux un premier résultat sans rien installer | ouvre `notebooks/00_demarrage_express.ipynb` (VS Code ou Google Colab) |
| Tu installes le projet | suis le chapitre 4, puis lance `python -m smartmarket.verifier_environnement` |
| Quelque chose ne fonctionne pas | annexe E du livre, puis la section 6 ci-dessous |

## 2. Contenu

| Emplacement | Contenu |
|---|---|
| `data/raw/` | export brut imparfait (chapitres 7 à 10) ; ne jamais le modifier |
| `data/processed/` | fichier propre de 6 000 clients, point de reprise dès le chapitre 11 |
| `data/scoring/` | 800 clients observés au 31/12/2025, sans cibles (chapitre 22) |
| `data/reference/` | dictionnaires des données, manifeste des empreintes |
| `notebooks/` | un notebook par chapitre (`NN_nom.ipynb`), à exécuter dans l'ordre |
| `notebooks/exercices/` | énoncés des exercices et des défis de partie, sans solutions |
| `notebooks/annexes/` | vérifications des annexes A, C, D, E et F |
| `src/smartmarket/` | code réutilisable : chemins, nettoyage, diagnostic, modèles, projet complet |
| `tests/` | tests automatiques (`python -m pytest`) |
| `scripts/verifier_windows.ps1` | vérification complète sous Windows |
| `outputs/` | vide au départ : tes figures, modèles, métriques et rapports |

## 3. Notebooks et chapitres

| Chapitres | Notebooks |
|---|---|
| 1 | `00_demarrage_express` |
| 2 à 4 | aucun : Terminal et installation |
| 5 et 6 | `05_bases_python`, `06_premier_dataframe`, `06_erreurs_volontaires` |
| 7 à 11 | `07_decouvrir_les_donnees` … `11_explorer_les_relations` |
| 12 à 15 | `12_preparer_prediction` … `15_analyser_erreurs` |
| 16 à 19 | `16_clients_jumeaux_knn` … `19_choix_modele` |
| 20 à 22 | `20_regression_logistique` … `22_seuil_priorites` |
| 23 et 24 | `23_kmeans`, `24_choisir_k` |
| 25 et 26 | `25_projet_reproductible`, `26_presenter` |
| 27 et 28 | `27_sous_le_capot`, `28_et_maintenant` |

`06_erreurs_volontaires` et `annexe_e_depannage` contiennent des cellules
qui **échouent exprès** (marquées `raises-exception`) : c'est normal.

Chaque notebook se vérifie avec **Redémarrer**, puis **Exécuter tout**.
Les notebooks des chapitres 25 et 26 écrivent dans `outputs/` : exécute
le 25 avant le 26.

## 4. Exercices et corrigés

À partir du chapitre 3, chaque chapitre propose trois exercices, et
chaque partie se termine par un défi. Les énoncés sont dans le livre et
dans `notebooks/exercices/`. Les corrigés sont dans l'annexe G du livre
et, avec leur code complet exécuté, dans `notebooks/corriges/` de
l'archive des corrigés.

Le défi de la partie VI et le corrigé du défi de la partie V ouvrent les
fichiers de vérité de la génération (`data/reference/*_verite.csv`) : un
vrai projet n'en dispose pas. Ces fichiers ne sont que dans l'archive des
corrigés ; le défi VI se fait avec elle.

## 5. Commandes utiles

```bash
python -m smartmarket.verifier_environnement   # diagnostic
python -m smartmarket.pipeline                 # projet de bout en bout
python -m smartmarket.presentation             # six diapositives
python -m pytest                               # tests
```

Dans l'archive des corrigés seulement :

```bash
python -m smartmarket.generer_donnees          # régénérer les données
python -m smartmarket.controles_donnees        # contrôles statistiques
python -m pytest tests_corriges                # tests des corrigés
```

## 6. Systèmes testés

| Système | Statut |
|---|---|
| macOS (Apple Silicon), Python 3.12.4 | tout exécuté : notebooks, corrigés, projet, tests, régénération des données à l'identique |
| macOS, Python 3.13.15 | installation des versions figées dans un dossier neuf, diagnostic, projet (mêmes résultats), tests, et exécution des 26 notebooks de cours |
| macOS, Python 3.14.6 | installation des versions figées, diagnostic, projet et tests exécutés (sorties du Terminal du livre) |
| Windows 10/11 | **Compatibilité Windows préparée et revue statiquement, mais non validée sur une machine Windows.** Relecture statique du code (chemins `pathlib`, encodage UTF-8 explicite, fins de ligne des données fixées par `.gitattributes` et par l'écriture des fichiers) ; script `scripts/verifier_windows.ps1` fourni |

Sous Windows, lance depuis le dossier du projet :

```powershell
powershell -ExecutionPolicy Bypass -File scripts\verifier_windows.ps1
```

Le script installe l'environnement, puis enchaîne diagnostic,
empreintes des données, exécution d'un notebook, projet complet et
tests ; dans l'archive des corrigés, il ajoute les contrôles statistiques
et les tests des corrigés. Son rapport est écrit dans
`outputs\reports\verification_windows.txt`.

**Point d'attention Windows.** Si tu récupères le projet avec Git, garde
le fichier `.gitattributes` : il empêche Git de convertir les fins de
ligne des CSV, ce qui changerait leurs empreintes. N'ouvre pas les CSV
avec Excel pour les réenregistrer.

## 7. Licences

Code : MIT. Données fictives : CC BY 4.0.
