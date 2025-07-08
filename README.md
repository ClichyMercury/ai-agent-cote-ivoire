# 🤖 Agent IA - Démarches Administratives Côte d'Ivoire

Un agent conversationnel intelligent pour accompagner les citoyens ivoiriens dans leurs démarches administratives.

## ✨ Fonctionnalités

- 🎭 **Conversation intelligente** avec mémoire contextuelle
- 🧠 **Recherche sémantique** avancée avec OpenAI
- 📋 **4 procédures** : CNI, Passeport, Acte de naissance, Mariage
- 🏢 **Centres administratifs** à Abidjan et Bouaké
- 💰 **Estimations** de coûts et délais
- 🎯 **Analyse d'intention** automatique
- 💡 **Suggestions proactives** personnalisées

## 🚀 Technologies

- **Backend**: NestJS + TypeScript
- **IA**: OpenAI GPT-4o-mini
- **Validation**: class-validator
- **API**: REST avec DTOs complets

## 📦 Installation

```bash
# Cloner le repo
git clone https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git
cd YOUR_REPO_NAME

# Installer les dépendances
npm install

# Configurer les variables d'environnement
cp .env.example .env
# Ajouter votre OPENAI_API_KEY dans .env

# Démarrer en développement
npm run start:dev
```

## 🔧 Configuration

Créez un fichier `.env` :
```env
OPENAI_API_KEY=sk-votre-clé-openai-ici
NODE_ENV=development
PORT=3000
```

## 📡 API Endpoints

### Conversation IA
- `POST /agent/conversation` - Chat avec mémoire
- `GET /agent/conversation/:userId/history` - Historique
- `GET /agent/conversation/:userId/suggestions` - Suggestions

### Recherche Intelligente
- `POST /agent/intelligent-search` - Recherche sémantique
- `POST /agent/analyze-intent` - Analyse d'intention
- `GET /agent/smart-suggestions` - Suggestions contextuelles

### Données
- `GET /agent/procedures` - Toutes les procédures
- `GET /agent/centers/:city` - Centres par ville
- `GET /agent/estimations` - Estimations coûts/délais

## 🧪 Tests avec Postman

Importez la collection Postman fournie dans `/docs/postman-collection.json`

## 🌍 Déploiement

Le projet est prêt pour le déploiement sur :
- Railway (recommandé)
- Vercel
- Docker + Cloud providers

## 📊 Données Supportées

- **4 Procédures** : CNI, Passeport, Acte naissance, Mariage
- **4 Centres** : Abidjan (3), Bouaké (1)
- **Estimations complètes** avec coûts en FCFA et délais

## 🤝 Contribution

Les contributions sont bienvenues ! Ouvrez une issue ou une PR.

## 📄 Licence

MIT License - Voir le fichier LICENSE

---

# .env.example
# Configuration pour l'agent IA
OPENAI_API_KEY=sk-your-openai-api-key-here
NODE_ENV=development
PORT=3000

# Optionnel pour des fonctionnalités avancées
REDIS_URL=redis://localhost:6379

---

# .gitignore
# Dependencies
node_modules/
npm-debug.log*
yarn-debug.log*
yarn-error.log*

# Runtime data
pids
*.pid
*.seed
*.pid.lock

# Coverage directory used by tools like istanbul
coverage/
*.lcov

# nyc test coverage
.nyc_output

# Compiled output
/dist
/tmp
/out-tsc

# Environment variables
.env
.env.local
.env.development.local
.env.test.local
.env.production.local

# IDEs and editors
/.idea
.project
.classpath
.c9/
*.launch
.settings/
*.sublime-workspace
.vscode/

# OS
.DS_Store
.DS_Store?
._*
.Spotlight-V100
.Trashes
ehthumbs.db
Thumbs.db

# Logs
logs
*.log

# Build
build/
dist/

---

# LICENSE
MIT License

Copyright (c) 2025 Danaya

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
