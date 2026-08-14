# 🎙️ PodMonétise — Kit Monétisation directe pour podcasteurs

Site de vente du kit pour podcasteurs indépendants (100-10 000 écoutes/épisode) qui perdent leur revenu pub in-app depuis que Spotify rend les pubs sautables (2026). Angle : la vente directe (sponsors, offres privées, abonnements, newsletter).

## 📁 Contenu du livrable

| Fichier | Rôle |
|---|---|
| `index.html` | Page d'accueil immersive 3D (WebGL + parallaxe) : hero, 6 modules, 3 offres (49/79/149 €), formulaire de commande EmailJS, garantie, footer |
| `kit-monetisation-podcast.md` | Le contenu complet niveau expert : 6 modules (leçon + exemple réel + exercice), checklist finale, grille tarifs — promesse : « premier sponsor signé en 30 jours » |
| `calculateur.html` | Calculateur interactif de tarifs sponsor (JS pur) : écoutes × CPM (2-4 € selon niche) × bonus engagement (+0/+15/+30 %) → prix unitaire + grille complète (spot, intégration, série, trimestre) |
| `chatbot.js` + `chatbot-config.js` | Widget chatbot « PodMonétise » : FAQs préprogrammées + capture de leads avec envoi EmailJS |
| `templates/` | 20 templates .md prêts à remplir : pitchs, relances, offre privée, contrat, média-kit, grille tarifs, questionnaire, scripts d'appel et d'antenne, emails abonnement/newsletter, rapport de campagne, renouvellement |

## ⚙️ Configuration EmailJS (déjà branchée)

- Service : `service_cy1ytdb`
- Template : `template_xpo58cv` (champs : `site`, `name`, `email`, `question`)
- Clé publique : `8Pui4ZEqxW2jRVF7h`

Le formulaire de commande envoie `{site: "PodMonétise — Kit Monétisation directe", name, email, question: "COMMANDE : <offre>"}`. Le chatbot envoie le même format pour les leads.

## 🚀 Mise en ligne

Site 100 % statique : déposez le dossier sur n'importe quel hébergement (Netlify, Vercel, GitHub Pages) ou exposez-le via un tunnel cloudflared. Aucun backend requis.

## 💰 Offres

- **Kit Essentiel — 49 €** : les 6 modules + checklist
- **Kit Pro — 79 €** : kit + calculateur interactif + 20 templates (le plus choisi)
- **Kit Premium — 149 €** : kit Pro + audit manuel personnalisé (réponse sous 48 h via EmailJS)

Garantie 14 jours satisfait ou remboursé.
