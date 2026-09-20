# Publier le dépôt sur GitHub

## 1. Créer le dépôt

Sur GitHub, crée un dépôt public nommé `openbms-designer`. Laisse les options
README, `.gitignore` et licence décochées : elles sont déjà incluses.

## 2. Personnaliser le lien

Dans `index.html`, remplace `YOUR-USERNAME` par ton identifiant GitHub.

## 3. Créer le premier commit

Depuis le dossier du projet :

```bash
git init -b main
git add .
git commit -m "feat: bootstrap OpenBMS Designer MVP"
git remote add origin https://github.com/YOUR-USERNAME/openbms-designer.git
git push -u origin main
```

Utilise l'identité Git configurée sur ton ordinateur afin que le commit soit
correctement associé à ton compte GitHub.

## 4. Configurer le dépôt

- Description : `Vendor-neutral open-source tool for sizing BMS controllers, I/O modules and communication networks from a point list.`
- Topics : `bms`, `building-automation`, `hvac`, `bacnet`, `modbus`, `energy-management`, `open-source`
- Active les Issues.
- Active Private vulnerability reporting dans **Settings → Security**.

## 5. Publier la démonstration

Dans **Settings → Pages**, choisis **Deploy from a branch**, puis la branche
`main` et le dossier `/ (root)`. L'application ne nécessite aucune compilation.

L'URL sera généralement :

`https://YOUR-USERNAME.github.io/openbms-designer/`

## 6. Avant la candidature

- Vérifie que le dépôt est public.
- Ouvre la démonstration et teste le bouton **Load example**.
- Remplace tous les `YOUR-USERNAME` restants.
- Ajoute l'URL du dépôt dans le formulaire Anthropic.
- Présente honnêtement le projet comme `early-stage`.
