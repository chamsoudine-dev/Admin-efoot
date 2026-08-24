# ⚙️ EFootLigue — Panneau d'Administration

Projet autonome pour la gestion des tournois, compétitions et tirages au sort de la plateforme **EFootLigue**.

Ce dépôt est strictement réservé aux organisateurs et administrateurs. Il est déployé de manière indépendante sur Vercel afin que les joueurs/utilisateurs n'aient aucun accès à l'administration depuis le site public.

---

## 🚀 Déploiement sur Vercel

1. Rendez-vous sur votre tableau de bord [Vercel](https://vercel.com).
2. Cliquez sur **Add New... > Project**.
3. Importez le dépôt GitHub : `chamsoudine-dev/Admin-efoot`.
4. Laissez les paramètres par défaut (Framework Preset : **Other** / Static).
5. Cliquez sur **Deploy**.
6. Vous obtenez votre URL d'administration privée (ex: `https://admin-efoot.vercel.app`).

---

## 🔐 Accès Administrateur

- **Mot de passe initial par défaut :** `cham123@`
- Vous pouvez créer votre propre compte organisateur ou changer le mot de passe depuis l'onglet **Paramètres** de l'administration.
- Une protection anti brute-force (verrouillage temporaire après 5 tentatives infructueuses) est intégrée.

---

## 🛠 Fonctionnalités

- **Gestion des compétitions :** Création, modification des règles, frais d'inscription, cagnottes et dates de tirage.
- **Gestion des inscriptions :** Liste des participants, validation des paiements Mobile Money en un clic, suppression / désinscription.
- **Tirage au sort automatique :** Génération des tableaux (1/8e, 1/4, 1/2, Finale) avec gestion des BYE automatique.
- **Saisie des scores en direct :** Saisie des scores par match et qualification instantanée du vainqueur.
- **Annonces en temps réel :** Diffusion d'alertes instantanées aux visiteurs du site joueur via Firebase Realtime Database.
- **Sauvegarde & Restauration :** Exportation et importation des données complètes au format JSON.

---

## 📡 Synchronisation Firebase

Les données sont synchronisées en direct avec Firebase Realtime Database :
- Base : `https://efoot-ba3de-default-rtdb.firebaseio.com`
