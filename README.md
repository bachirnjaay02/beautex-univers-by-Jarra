# BEAUTEX UNIVERS — Boutique simple (Front-end)

Résumé
- Petite vitrine de tissus avec ajout au panier, gestion des quantités, persistance locale, et envoi d'un récapitulatif via WhatsApp.

Fonctionnalités principales ✅
- Ajouter un produit au panier (badge du panier et total mis à jour).
- Contrôles de quantité (+ / −) et suppression d'articles.
- Bouton **Vider le panier** avec confirmation.
- Modal de confirmation avec champs **Nom**, **Téléphone**, **Adresse** et option "Mémoriser mes coordonnées" (stocké dans localStorage).
- Envoi de la commande via WhatsApp Web/App avec message pré‑rempli (nom, téléphone, adresse, liste des articles, total).
- Animation visuelle lors de l'ajout et styles responsives.

Fichiers clés
- `index.html` : structure HTML, composants produit, offcanvas panier, modal de checkout, et toute la logique JavaScript.
- `styles.css` : styles globaux et l'animation "pulse".
- `img/` : images des produits.

Installation / Aperçu local
1. Ouvrir simplement `index.html` dans votre navigateur (double‑clic) pour un usage local.
2. Pour servir via un petit serveur (recommandé si vous utilisez des modules ou voulez éviter restrictions de CORS) :
   - Python 3 : `python -m http.server 8000` puis ouvrir `http://localhost:8000`.

Configuration
- Numéro WhatsApp destinataire : dans `index.html` cherchez la variable `const phone = '221777120901';` et remplacez par le numéro souhaité (format international, sans espaces ni +)

Tests rapides
1. Ouvrir la page et cliquer sur **Ajouter** sur un ou plusieurs produits.
2. Ouvrir le panier (il s'ouvre automatiquement après ajout) et modifier les quantités, tester **Suppr** et **Vider le panier**.
3. Cliquer **Commander** → la modal s'ouvre ; remplir (optionnel) Nom/Téléphone/Adresse. Cliquer **Envoyer via WhatsApp**.
4. WhatsApp Web / App doit s'ouvrir avec le message prêt à l'envoi. Le panier est vidé après l'envoi.

Bonnes pratiques et améliorations possibles
- Ajouter des toasts (au lieu d'alerte navigateur) pour messages d'information.
- Validation plus stricte des numéros.
- Intégration côté serveur pour stocker les commandes et envoi de notifications.

Licence
- Projet d'exemple — libre à l'utilisation et modification pour vos besoins.

Contact
- Pour des améliorations ou questions, éditez directement les fichiers dans ce dépôt ou demandez des ajouts spécifiques.