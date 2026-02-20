# 🕰️ TimeTravel Agency — Webapp Interactive

**Webapp moderne et immersive pour une agence fictive de voyage temporel premium.**  
Projet pédagogique réalisé avec Next.js, TypeScript, Tailwind CSS et IA conversationnelle.

---

## 🚀 Démo en ligne

👉 https://euro-site-france--eenzocl.replit.app

---

# 🌌 Concept du projet

TimeTravel Agency est une plateforme web interactive permettant de :

- Découvrir des destinations temporelles immersives  
- Interagir avec un agent conversationnel intelligent  
- Recevoir des recommandations personnalisées  
- Réserver et planifier un voyage temporel  

L’expérience est pensée premium, immersive et mobile-first, avec un design sombre élégant et des animations subtiles.

---

# 🛠️ Stack technique

## Frontend
- Next.js (App Router)
- TypeScript
- Tailwind CSS
- Framer Motion (animations)

## Backend
- API Route `/api/chat`
- Mode IA compatible :
  - Mistral
  - OpenRouter
  - Groq
- Mode démo intégré (fonctionne sans clé API)

---

# ✨ Fonctionnalités du site

## 🏠 Landing Page immersive

- Hero avec animation / vidéo de fond (fallback gradient animé)
- Thème sombre premium + accents dorés `#d4af37`
- Présentation de l’agence :
  - Luxe
  - Sécurité temporelle
  - Accompagnement
  - Temporal Protocol™
- CTA vers :
  - Destinations
  - Réservation
  - Chatbot

---

## 🌍 Destinations temporelles

### 🇫🇷 Paris 1889
- Belle Époque  
- Exposition Universelle  
- Tour Eiffel  
- Voyage culturel raffiné  

### 🦖 Crétacé (-65M)
- Dinosaures  
- Jungle préhistorique  
- Expédition guidée  
- Aventure immersive  

### 🎨 Florence 1504
- Renaissance  
- Michel-Ange  
- Art & architecture  
- Voyage élégant  

---

## 🧩 Cards interactives

- Hover : glow + zoom image  
- Reveal informations  
- Navigation vers pages détails  

---

## 📄 Pages détails destinations

Chaque page contient :

- Hero immersif
- Résumé narratif
- “À ne pas manquer”
- Conseils de l’agent
- Règles de sécurité temporelle
- CTA “Planifier ce voyage”

Les données sont centralisées dans :

`src/data/destinations.ts`

---

## 🤖 Chatbot IA

Widget flottant en bas à droite.

Fonctionnalités :

- Historique de conversation
- Conseils sur destinations
- Réponses FAQ agence
- Suggestions personnalisées
- Aide à la réservation

### Personnalité

Assistant professionnel, chaleureux, passionné d’histoire et expert crédible en voyage temporel de luxe.

---

## 🧠 Backend IA

Route :

`POST /api/chat`

### Mode Démo
- Réponses générées via règles + FAQ

### Mode IA réel
Si clé fournie :

- Mistral
- OpenRouter
- Groq

Les clés sont stockées côté serveur uniquement.

---

## 🧪 Quiz de recommandation

4 questions interactives :

- Type d’expérience
- Période préférée
- Ambiance
- Activité idéale

Résultat :

- Destination recommandée
- Explication personnalisée
- CTA vers réservation

---

## 📝 Formulaire de réservation

Page `/book` :

- Destination
- Dates
- Groupe (1–6)
- Préférences
- Niveau de confort

Validation :

- Champs requis
- Dates cohérentes
- Message de confirmation stylé

Option :

- Itinéraire généré automatiquement (IA ou template)

---

# 🎨 Design & UX

- Dark mode premium
- Accents dorés `#d4af37`
- Animations Framer Motion :
  - Fade-in scroll
  - Hover interactions
- Mobile-first
- Accessibilité :
  - Navigation clavier
  - aria-label
- Lazy loading images
- Lighthouse friendly

---

# 📂 Structure du projet

app/  
 page.tsx  
 destinations/  
 book/  
 about/  
 api/chat/  

src/  
 components/  
 data/  
 styles/  

public/  
 images/  

---
