# SENTINEL v6

**Application de diagnostic système multi-plateforme**  
*protect · clean · control*

> © 2025 SHAMS&DEAN — Tous droits réservés.  
> Reproduction, redistribution ou usage commercial sans autorisation écrite strictement interdits.

---

## Présentation

SENTINEL analyse votre ordinateur et génère un rapport HTML complet, 100% local.  
Aucune donnée n'est envoyée à un serveur externe.

Deux modes d'affichage :

- **Mode Simple** — Vue débutant : cartes compactes, verdicts colorés, langage clair.
- **Mode Expert** — Vue technique : 240+ métriques, tableaux détaillés, commandes Terminal.

---

## Fonctionnalités

| Module | Données collectées |
|---|---|
| Sécurité | Gatekeeper, SIP, FileVault, pare-feu, Secure Boot, permissions apps |
| Performance | CPU, GPU, RAM, températures, consommation, processus actifs |
| Batterie | Cycles, capacité, tension, autonomie estimée |
| Stockage | Disques SMART, volumes, fichiers en double, top fichiers lourds |
| Réseau | WiFi, IP, DNS, VPN, appareils connectés, connexions actives |
| Périphériques | USB, Thunderbolt, Bluetooth, caméras, audio |
| Applications | Liste installée, versions, droits d'accès caméra/micro |
| Diagnostic | Scores 0–100, radar d'alertes, estimation de valeur de revente |

---

## Versions disponibles

### macOS Intel (x86_64)
- Mac Intel — 2017 à 2020
- Launcher bash + application .app
- Python 3.9+ requis
- Guide d'installation illustré inclus

### macOS Apple Silicon (arm64)
- M1, M2, M3, M4 — 2020 et après
- Launcher zsh + PATH Homebrew ARM
- Capteurs thermiques Apple Silicon
- Python 3.9+ requis

### Windows 10 / 11
- Launcher SENTINEL.bat (double-clic)
- PowerShell, WMI, Registre Windows
- BitLocker, Defender, TPM, UAC, Secure Boot UEFI
- Python 3.9+ requis — [python.org](https://www.python.org/downloads/)

### Linux — Ubuntu / Debian / Fedora
- Script `sentinel.sh` + fichier `.desktop`
- `/proc/`, `lsblk`, `nmcli`, `ss`, `df`, `sensors`
- LUKS, AppArmor / SELinux, ClamAV
- Snap, Flatpak, dpkg, rpm supportés

---

## Installation

### macOS
```bash
# 1. Extraire le ZIP sur votre Bureau
# 2. Ouvrir le guide d'installation (install_guide.html)
# 3. Suivre les étapes pour contourner Gatekeeper
# 4. Double-cliquer sur Sentinel.app
```

### Windows
```
1. Installer Python 3.9+ depuis python.org (cocher "Add to PATH")
2. Extraire le ZIP
3. Double-cliquer sur SENTINEL.bat
```

### Linux
```bash
# Extraire le ZIP
chmod +x sentinel.sh
./sentinel.sh

# Dépendances optionnelles (Ubuntu/Debian)
sudo apt install lsblk util-linux smartmontools lm-sensors
```

---

## GitHub Pages

Pour déployer la vitrine sur GitHub Pages :

```bash
# 1. Forker ou cloner ce dépôt
git clone https://github.com/shamsetdean/sentinel.git
cd sentinel

# 2. Activer GitHub Pages
# Settings > Pages > Source: Deploy from branch > main / root

# 3. La page sera disponible à :
# https://shamsetdean.github.io/sentinel/
```

Structure du dépôt :

```
sentinel/
├── index.html          ← Vitrine GitHub Pages
├── README.md           ← Ce fichier
├── LICENSE             ← Licence propriétaire
├── LEGAL.md            ← Mentions légales
├── PRIVACY.md          ← Politique de confidentialité
└── assets/
    ├── screenshot_simple.svg
    └── screenshot_expert.svg
```

---

## Confidentialité

SENTINEL ne contacte **aucun serveur externe** pendant l'analyse.

- Aucune donnée personnelle transmise
- Rapport HTML généré et stocké localement (Bureau)
- Mot de passe admin utilisé uniquement en mémoire vive, jamais stocké
- Aucun telemetry, aucun tracking, aucune analytics

---

## Licence et protections

Ce projet est protégé par le droit d'auteur.

- Code source : licence propriétaire SHAMS&DEAN
- Icônes SVG : Lucide Icons (ISC License) — libres pour usage commercial
- Polices : DM Sans, DM Mono (Google Fonts, SIL OFL 1.1) — libres pour usage commercial
- Rapport HTML généré : propriété de l'utilisateur final

**Toute reproduction, modification ou redistribution du code source sans autorisation écrite est interdite.**

Voir [LICENSE](LICENSE) et [LEGAL.md](LEGAL.md) pour les détails.

---

## Contact

SHAMS&DEAN  
Pour toute demande de licence commerciale ou partnership, contactez-nous via GitHub.

---

*SENTINEL v6.0 — © 2025 SHAMS&DEAN*
