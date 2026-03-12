# Technical Documentation Portal

Bienvenue dans la documentation technique de **ventoy-toolkit**. Ce projet rationalise le déploiement multi-OS via une clé USB Ventoy personnalisée.

---

## Structure de `docs/`

```text
docs/
├── README.md           # Ce portail
├── cloc-report.md      # Statistiques du code (Généré par cloc)
├── specification.txt   # Dictionnaire technique dense
└── diagrams/           # Sources et exports visuels
    └── png/            # Exports images (.png)
```

---

## 1. Dictionnaire Technique

[**specification.txt**](./specification.txt) — Une vue condensée de la structure des dossiers ISO, des fichiers de persistance et du système de thème.

---

## 2. Statistiques du Code (CLOC)

> [!TIP]
> Pour régénérer ce rapport :
> ```bash
> nix shell nixpkgs#cloc -c cloc . --exclude-dir=.git,node_modules,result,.direnv --md --out=docs/cloc-report.md
> ```

Rapport complet : [**cloc-report.md**](./cloc-report.md).

---

## 3. Architecture du Projet

```text
/
├── assets/                 # Repository visual assets and logos
├── iso/                    # ISO storage (rescue, tools, os)
└── ventoy/                 # Ventoy core configuration (json, theme)
```
