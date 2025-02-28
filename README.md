# 🚀 flvm - Flutter Local (Light) Version Manager
**Gérez facilement plusieurs versions de Flutter localement**

---

## 📌 Description
`flvm` (**Flutter Local (Light) Version Manager**) est un outil CLI permettant de :
✔ **Installer plusieurs versions de Flutter**  
✔ **Basculer rapidement entre différentes versions**  
✔ **Utiliser un dépôt interne de Flutter** (`FLUTTER_STORAGE_BASE_URL`)  
✔ **Nettoyer les versions inutilisées**  
✔ **Lister les versions installées**  
✔ **Mettre à jour Flutter vers la dernière version stable**  

🔥 **Idéal pour les développeurs Flutter travaillant sur plusieurs projets !**  

---

## 📌 Installation

### 1️⃣ Activer le package globalement
```bash
dart pub global activate flvm
```

### 2️⃣ Ajouter `~/.pub-cache/bin` au PATH (si ce n'est pas déjà fait)
Ajoute cette ligne à ton `~/.bashrc`, `~/.zshrc` ou `~/.profile` :
```bash
export PATH="$PATH":"$HOME/.pub-cache/bin"
```
Puis exécute :
```bash
source ~/.bashrc   # ou source ~/.zshrc
```

---

## 📌 Utilisation

### 📥 1. Installer une version spécifique
```bash
flvm install 3.13.9
```

### 🔄 2. Changer de version
```bash
flvm use 3.13.9
```

### 📜 3. Lister les versions installées
```bash
flvm list
```

### 🔍 4. Voir la version actuelle
```bash
flvm current
```

### 🗑️ 5. Supprimer une version installée
```bash
flvm remove 3.10.8
```

### 🧹 6. Nettoyer les versions inutilisées
```bash
flvm clean
```

### 🔄 7. Mettre à jour vers la dernière version stable
```bash
flvm update
```

---

## 📌 Utilisation d’un dépôt interne (URL personnalisée)

Si ton entreprise héberge ses propres versions de Flutter, définis **une variable d’environnement** :
```bash
export FLUTTER_STORAGE_BASE_URL="https://intranet.mycompany.com/flutter"
```
Puis exécute :
```bash
flvm install 3.13.9
```

---

## 📌 Comparaison avec `fvm` (Flutter Local (Light) Version Manager)

| Fonctionnalité  | flvm | fvm |
|----------------|------|------|
| 📥 Installer une version Flutter | ✅ Oui | ✅ Oui |
| 🔄 Changer de version | ✅ Oui | ✅ Oui |
| 🏢 Support des dépôts internes | ✅ Oui | ❌ Non |
| 🧹 Nettoyage automatique des versions inutilisées | ✅ Oui | ❌ Non |
| 📜 Lister les versions installées | ✅ Oui | ✅ Oui |
| ⚡ Simplicité d'utilisation | ✅ Très simple | ❌ Plus complexe |

🔹 **`flvm` est conçu pour être plus léger et rapide que `fvm`, avec une meilleure prise en charge des entreprises.**  

---

## 📌 Désinstallation

Si tu veux supprimer `flvm` :
```bash
dart pub global deactivate flvm
```

Supprime également le cache local :
```bash
rm -rf ~/flvm_versions
```

---

## 📌 Licence

**MIT License** - Utilisation libre et open source 🚀  

---

## 📌 Contribuer

Si tu veux contribuer :
1. **Fork le projet** sur [GitHub](https://github.com/mohachouch/flvm)
2. Clone le repo :
   ```bash
   git clone https://github.com/mohachouch/flvm.git
   cd flvm
   ```
3. Fais tes modifications et propose une **pull request** ✅

---

🚀 **Merci d'utiliser `flvm` - Gère tes versions Flutter en toute simplicité !** 🎯
