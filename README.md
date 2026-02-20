🕰️ TimeTravel Agency – Webapp Interactive

Webapp moderne et immersive pour une agence fictive de voyage temporel premium.

Projet pédagogique réalisé avec Next.js (App Router) + TypeScript + Tailwind CSS, intégrant :

🌌 Landing immersive

🌍 3 destinations temporelles interactives

🤖 Chatbot IA (mode démo ou API réelle)

🧠 Quiz de recommandation personnalisé

📝 Formulaire de réservation intelligent

✨ Animations subtiles & UX premium

🚀 Démo en ligne

👉 https://euro-site-france--eenzocl.replit.app

🛠️ Stack Technique

Next.js (App Router)

TypeScript

Tailwind CSS

Framer Motion (animations)

API Route interne /api/chat

Mode IA compatible :

Mistral

OpenRouter

Groq

Aucune dépendance lourde ou exotique.

✨ Fonctionnalités principales
🏠 Landing Page immersive (/)

Hero section avec faux background vidéo (fallback gradient animé)

Thème sombre premium + accents dorés #d4af37

Présentation agence :

Luxe

Sécurité temporelle

Accompagnement personnalisé

Temporal Protocol™

CTA vers :

Destinations

Réservation

Chatbot

🌍 Galerie des destinations (/destinations)

3 destinations interactives :

🇫🇷 Paris 1889

Belle Époque

Exposition Universelle

Tour Eiffel

Risque faible

Séjour culturel raffiné

🦖 Crétacé (-65M)

Dinosaures

Jungle préhistorique

Expédition guidée

Risque élevé

Aventure immersive

🎨 Florence 1504

Renaissance italienne

Michel-Ange

Art & architecture

Risque modéré

Élégance artistique

🎯 Cards interactives

Hover : glow doré + zoom image

Reveal “En savoir plus”

Navigation vers page détail

📄 Pages Détails Destinations (/destinations/[slug])

Chaque destination contient :

Hero immersif

Résumé narratif premium

“À ne pas manquer”

Bloc dynamique “Conseils de l’agent”

Règles de sécurité temporelle (checklist)

CTA “Planifier ce voyage”

Les données sont centralisées dans :

src/data/destinations.ts

Toutes les pages lisent depuis cette source unique.

🤖 Chatbot IA (Widget flottant)

Bulle flottante bas-droite

Historique messages

Placeholder :

"Posez-moi vos questions sur les voyages temporels…"

Personnalité

Assistant virtuel professionnel, chaleureux, passionné d’histoire, expert crédible en voyage temporel de luxe.

Il peut répondre à :

Questions sur les destinations

Prix

Conseils personnalisés

FAQ agence

Aide à la réservation

🧠 Backend IA

Route API :

POST /api/chat

Reçoit :

{
  "messages": [{ "role": "user", "content": "..." }]
}
Deux modes :
🔹 Mode Démo (sans clé API)

Réponses générées par règles + FAQ interne

Recommandations basées sur mots-clés

🔹 Mode IA réel (si clé fournie)

Supporte :

Mistral

OpenRouter

Groq

⚠️ Les clés sont uniquement côté serveur (jamais exposées client).

🧩 Quiz de recommandation

4 questions :

Type d’expérience

Période préférée

Ambiance

Activité idéale

Résultat :

Scoring automatique

Destination recommandée

Explication personnalisée

Si IA active → reformulation enrichie

Bouton vers /book avec destination pré-sélectionnée

📝 Formulaire de réservation (/book)

Champs :

Destination

Dates départ / retour

Taille du groupe (1–6)

Préférences

Niveau de confort (Standard / Premium / Ultra)

Validation :

Dates cohérentes

Champs requis

Message de confirmation stylé

Option :

Récapitulatif généré (template ou IA)

🎨 Design & UX

Thème sombre premium

Accents dorés #d4af37

Animations Framer Motion :

Fade-in au scroll

Hover subtil

Mobile-first

Accessibilité :

aria-label

navigation clavier

Lazy loading images

Lighthouse friendly

📂 Structure du projet
app/
  page.tsx
  destinations/
  book/
  about/
  api/chat/

src/
  data/destinations.ts
  components/
  styles/

Assets placeholders prévus pour être remplacés facilement par les visuels du projet précédent.

⚙️ Installation locale
npm install
npm run dev

Build :

npm run build
npm start
🔐 Configuration IA (optionnel)

Créer un fichier :

.env.local

Exemple :

MISTRAL_API_KEY=
OPENROUTER_API_KEY=
GROQ_API_KEY=

Ou utiliser .env.example fourni.

📸 Remplacement des images

Les images actuelles sont des placeholders.

Pour les remplacer :

Ajouter vos visuels dans public/images/

Modifier src/data/destinations.ts

Mettre à jour les chemins

📖 Transparence IA

Code assisté par IA générative

Chatbot : modèle léger (si clé API fournie)

Mode démo intégré pour usage pédagogique

🎓 Contexte pédagogique

Projet réalisé dans le cadre d’un module M1/M2 Digital & IA.

Objectifs :

Architecture moderne Next.js

Intégration IA responsable

UX premium

Déploiement fonctionnel

Documentation open source claire

📜 Licence

Projet pédagogique — usage académique.
