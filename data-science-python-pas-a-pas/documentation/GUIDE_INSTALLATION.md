# Guide d'installation des ressources

*Data science avec Python, pas à pas* — ressources du lecteur v1.0.1.

## 1. Télécharger et vérifier l'archive

Télécharge [`Ressources_Lecteur_v1.0.1.zip`](https://github.com/belksiri/books/releases/download/data-science-python-pas-a-pas-v1.0.1/Ressources_Lecteur_v1.0.1.zip) (541 Ko).

Son empreinte SHA-256 doit être exactement :

```text
f63cdf2b4cb0306e46371ec24c01ce584013ca088e6b2ea5f70c5596fec6eb0e
```

**macOS** (Terminal, dans le dossier du téléchargement) :

```bash
shasum -a 256 Ressources_Lecteur_v1.0.1.zip
```

**Windows** (PowerShell, dans le dossier du téléchargement) :

```powershell
Get-FileHash Ressources_Lecteur_v1.0.1.zip -Algorithm SHA256
```

Windows affiche l'empreinte en majuscules : c'est la même valeur.
Si elle diffère, supprime le fichier et télécharge-le de nouveau.

## 2. Décompresser

Décompresse l'archive dans ton dossier **Documents**. Tu obtiens le
dossier `data_science_python_pas_a_pas`. N'ouvre pas les fichiers CSV avec
Excel pour les réenregistrer : le diagnostic vérifie leurs empreintes.

## 3. Premier résultat sans rien installer

Ouvre `notebooks/00_demarrage_express.ipynb` dans VS Code **ou** dans
Google Colab (Fichier › Importer le notebook), puis exécute les cellules
une par une. L'extrait de données est inclus dans le notebook.

## 4. Installer le projet complet

Il faut **Python 3.12, 3.13 ou 3.14**. Le chapitre 2 du livre explique
l'installation de Python et de VS Code ; le chapitre 4, l'environnement
virtuel.

Ouvre un terminal **dans le dossier `data_science_python_pas_a_pas`**.

**macOS**

```bash
python3 -m venv .venv
source .venv/bin/activate
python -m pip install --upgrade pip
python -m pip install -r requirements.txt
python -m pip install -e .
python -m smartmarket.verifier_environnement
```

**Windows (PowerShell)**

```powershell
py -m venv .venv
.venv\Scripts\Activate.ps1
python -m pip install --upgrade pip
python -m pip install -r requirements.txt
python -m pip install -e .
python -m smartmarket.verifier_environnement
```

Si PowerShell refuse l'activation :
`Set-ExecutionPolicy -Scope CurrentUser RemoteSigned`, puis recommence.

Le diagnostic doit se terminer par :

```text
Environnement SmartMarket prêt.
```

## 5. Vérifier que tout fonctionne

Environnement activé, depuis le dossier du projet :

```bash
python -m pytest                    # tests
python -m smartmarket.pipeline      # projet de bout en bout
python -m smartmarket.presentation  # six diapositives
```

Sous Windows, un script enchaîne l'installation et toutes les
vérifications :

```powershell
powershell -ExecutionPolicy Bypass -File scripts\verifier_windows.ps1
```

## Systèmes vérifiés

| Système | Statut |
|---|---|
| macOS, Python 3.12.4 | notebooks, projet et tests exécutés |
| macOS, Python 3.13.15 | installation, diagnostic, projet, tests, 26 notebooks de cours |
| macOS, Python 3.14.6 | installation depuis l'archive, diagnostic, tests, 65 notebooks |
| Windows 10/11 | Compatibilité Windows préparée et revue statiquement, mais non validée sur une machine Windows. |

## En cas de problème

1. Relis le message d'erreur jusqu'à la dernière ligne (chapitre 6).
2. Consulte l'annexe E du livre (dépannage) et la [FAQ](FAQ.md).
3. [Signale le problème](https://github.com/belksiri/books/issues/new?template=probleme_ressources.md) en joignant la sortie du
   diagnostic.
