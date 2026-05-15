# Guide de déploiement du site — Margaux Bezard, Psychologue

> Ce guide t'accompagne **pas à pas** pour mettre ton site en ligne.
> Compte environ **1h30 à 2h** la première fois. Aucune compétence technique requise.
>
> Tu auras besoin de :
> - Une adresse email
> - Une carte bancaire (uniquement pour le nom de domaine, ~10€/an)
> - Le dossier `margaux-site` que Matthieu t'a transféré

---

## 🗺️ Vue d'ensemble — ce qu'on va faire

1. **GitHub** (gratuit) → stocker les fichiers du site
2. **Netlify** (gratuit) → publier le site sur internet
3. **OVH** (~10€/an) → acheter ton nom de domaine (`margaux-bezard-psychologue.fr` par exemple)
4. **Brancher** OVH sur Netlify → ton site sera accessible avec ton vrai nom de domaine
5. **Google Search Console** → dire à Google d'indexer ton site

À la fin, quand quelqu'un tapera "psychologue Bayonne" ou "psy TCC Pays Basque" sur Google, ton site apparaîtra (après quelques semaines d'indexation).

---

## ÉTAPE 1 — Créer un compte GitHub (10 min)

GitHub, c'est l'endroit où on stocke les fichiers de ton site. C'est gratuit.

1. Va sur **https://github.com**
2. Clique sur **"Sign up"** (en haut à droite)
3. Entre ton email professionnel (ex : margaux.bezard@gmail.com)
4. Choisis un mot de passe solide (note-le quelque part en sécurité)
5. Choisis un nom d'utilisateur (ex : `margauxbezard`)
6. Tu vas recevoir un email avec un code → entre-le pour valider
7. Sur les questions de personnalisation : choisis **Free plan**, ignore le reste

✅ Tu as maintenant un compte GitHub.

---

## ÉTAPE 2 — Créer ton repository (l'endroit où vont vivre les fichiers) (5 min)

1. Une fois connectée sur GitHub, clique sur le **"+"** en haut à droite → **"New repository"**
2. Remplis :
   - **Repository name** : `margaux-site`
   - **Description** : `Site web psychologue TCC Pays Basque`
   - Coche **"Public"** (gratuit, c'est ce qu'on veut)
   - Coche **"Add a README file"**
3. Clique sur **"Create repository"** (bouton vert en bas)

✅ Tu as un dossier (repository) prêt à recevoir les fichiers.

---

## ÉTAPE 3 — Uploader les fichiers du site (10 min)

Tu vas glisser-déposer les fichiers dans ton repository.

1. Sur la page de ton repository, clique sur **"Add file"** (bouton blanc à droite, au-dessus de la liste des fichiers) → **"Upload files"**
2. Ouvre le dossier `margaux-site` que Matthieu t'a transféré sur ton ordinateur
3. **Sélectionne TOUS les fichiers** (Ctrl+A sur Windows, Cmd+A sur Mac) :
   - `index.html`
   - `styles.css`
   - `mentions-legales.html`
   - `robots.txt`
   - `sitemap.xml`
   - `_redirects`
   - `_headers`
   - `.gitignore`
4. **Glisse-les** dans la zone "Drag files here..." du navigateur
5. Attends que tous les fichiers soient uploadés (barre de progression verte)
6. En bas de page :
   - Dans le champ "Commit changes", écris : `Mise en ligne initiale`
   - Laisse "Commit directly to the main branch" coché
7. Clique sur **"Commit changes"** (bouton vert)

✅ Tes fichiers sont sur GitHub. Tu peux les voir listés sur la page du repository.

> ⚠️ Tu ne vois pas `.gitignore` ou `_redirects` après l'upload ? C'est normal, les fichiers qui commencent par un point ou underscore sont parfois cachés. Vérifie qu'ils sont bien là en cliquant sur la liste des fichiers.

---

## ÉTAPE 4 — Créer un compte Netlify (5 min)

Netlify va prendre tes fichiers GitHub et les transformer en site internet accessible à tout le monde.

1. Va sur **https://www.netlify.com**
2. Clique sur **"Sign up"** (en haut à droite)
3. Choisis **"Sign up with GitHub"** → ça connecte directement ton compte
4. Autorise Netlify à accéder à GitHub (clique sur "Authorize Netlify")
5. Sur l'écran d'accueil Netlify, on te demande quelques infos (rôle, équipe...) → tu peux tout sauter ou répondre rapidement

✅ Tu as un compte Netlify connecté à ton GitHub.

---

## ÉTAPE 5 — Publier ton site avec Netlify (10 min)

1. Sur le tableau de bord Netlify, clique sur **"Add new site"** → **"Import an existing project"**
2. Choisis **"Deploy with GitHub"**
3. Une fenêtre s'ouvre → autorise Netlify à accéder à tes repositories
   - Choisis **"Only select repositories"**
   - Sélectionne `margaux-site` dans la liste
   - Clique sur **"Install"**
4. De retour sur Netlify, clique sur ton repository `margaux-site`
5. Sur la page de configuration :
   - **Branch to deploy** : `main` (laissé par défaut)
   - **Build command** : laisse vide
   - **Publish directory** : laisse vide ou mets `/`
6. Clique sur **"Deploy margaux-site"** (bouton bleu en bas)

⏳ Attends 1 à 2 minutes. Netlify construit ton site.

7. Quand c'est prêt, tu vois une URL bizarre du genre `https://gentle-cloud-12345.netlify.app`
8. **Clique dessus** → ton site est en ligne ! 🎉

> 💡 **Renommer l'URL Netlify** : dans Netlify → "Site configuration" → "Change site name" → mets `margaux-bezard-psychologue`. L'URL devient `https://margaux-bezard-psychologue.netlify.app`. C'est temporaire, on va brancher ton vrai nom de domaine ensuite.

---

## ÉTAPE 6 — Acheter ton nom de domaine sur OVH (15 min)

Le nom de domaine, c'est ton adresse propre (ex : `margaux-bezard-psychologue.fr`). Ça coûte environ **8 à 12€ par an**.

### Idées de noms de domaine
- `margaux-bezard-psychologue.fr` ← recommandé (clair, complet, bon pour le SEO)
- `margauxbezard.fr`
- `psychologue-bezard.fr`
- `psy-pays-basque.fr` ← très bon pour le SEO mais générique
- `bezard-psychologue.fr`

> 🎯 **Conseil SEO** : un nom contenant "psychologue" ou ta localisation aide légèrement le référencement. Mais le plus important reste la lisibilité.

### Procédure d'achat

1. Va sur **https://www.ovh.com/fr/domaines/**
2. Tape le nom de domaine que tu veux dans la barre de recherche → "Rechercher"
3. Si le domaine est disponible (coche verte), clique sur **"Commander"**
4. Sur la page de configuration :
   - Choisis l'offre **"Domaine seul"** (la moins chère)
   - Décoche tous les services supplémentaires (DNS Anycast, certificat SSL — Netlify s'en charge gratuitement)
   - Choisis **1 an** (~10€)
5. Crée un compte OVH si tu n'en as pas (email + mot de passe)
6. Remplis tes informations (adresse personnelle ou professionnelle)
7. Paye avec ta carte bancaire

✅ Tu as ton nom de domaine. Tu reçois un email de confirmation.

⏳ **Attends 1 à 2 heures** que le domaine soit activé avant l'étape suivante.

---

## ÉTAPE 7 — Connecter ton domaine OVH à Netlify (20 min)

C'est l'étape la plus technique mais on va y aller doucement.

### 7A — Ajouter ton domaine dans Netlify

1. Sur Netlify, va sur ton site → **"Domain management"** (dans le menu de gauche)
2. Clique sur **"Add a domain"** → tape `margaux-bezard-psychologue.fr` (ton vrai domaine sans le `www.`)
3. Netlify te dit : "Verify domain" → confirme que c'est bien à toi
4. Netlify affiche maintenant deux options :
   - Option **"Set up Netlify DNS"** ← **on va prendre celle-ci**, c'est la plus simple
   - Option "External DNS"

5. Clique sur **"Set up Netlify DNS"** → Netlify te donne **4 adresses** appelées "name servers" qui ressemblent à :
   ```
   dns1.p01.nsone.net
   dns2.p01.nsone.net
   dns3.p01.nsone.net
   dns4.p01.nsone.net
   ```
   ⚠️ **Note bien ces 4 adresses** (copie-les dans un texte) — tu vas les coller dans OVH.

### 7B — Configurer OVH pour pointer vers Netlify

1. Va sur **https://www.ovh.com/manager/** et connecte-toi
2. Clique sur **"Web Cloud"** dans le menu de gauche
3. Clique sur **"Noms de domaine"** → ton domaine `margaux-bezard-psychologue.fr`
4. Cherche l'onglet **"Serveurs DNS"** (ou "DNS servers")
5. Clique sur **"Modifier les serveurs DNS"**
6. **Supprime** les serveurs DNS OVH actuels (`dns.ovh.net`, etc.)
7. **Colle les 4 serveurs DNS de Netlify** un par un :
   ```
   dns1.p01.nsone.net
   dns2.p01.nsone.net
   dns3.p01.nsone.net
   dns4.p01.nsone.net
   ```
8. Clique sur **"Appliquer la configuration"** ou "Valider"

⏳ **Attends entre 1h et 24h** que le changement se propage sur internet. C'est normal, c'est la "propagation DNS".

### 7C — Vérifier que ça marche

1. De temps en temps, tape ton domaine dans le navigateur : `https://margaux-bezard-psychologue.fr`
2. Quand tu vois TON site (et pas une page d'erreur OVH), c'est bon ! ✅
3. Sur Netlify, retourne dans **"Domain management"** → tu dois voir des coches vertes à côté de ton domaine
4. **Active HTTPS** : Netlify le fait automatiquement gratuitement (Let's Encrypt). Si tu vois "Verify DNS configuration" → clique dessus pour activer le certificat SSL.

✅ Ton site est officiellement en ligne avec ton vrai nom de domaine et en HTTPS sécurisé !

---

## ÉTAPE 8 — Soumettre ton site à Google (15 min)

C'est ce qui va faire apparaître ton site dans les résultats de recherche Google. **Étape critique pour le SEO.**

1. Va sur **https://search.google.com/search-console**
2. Connecte-toi avec ton compte Google (Gmail)
3. Clique sur **"Ajouter une propriété"** → choisis **"Préfixe de l'URL"**
4. Entre l'URL complète : `https://margaux-bezard-psychologue.fr/` (avec le `https://` et le `/` final)
5. Google demande de vérifier que c'est ton site. Méthode la plus simple : **"Balise HTML"**
   - Google te donne un code du genre `<meta name="google-site-verification" content="ABC123XYZ..." />`
   - Tu dois l'ajouter dans le `<head>` de ton fichier `index.html`
   - Pour ça : retourne sur GitHub → ton repo → clique sur `index.html` → clique sur le crayon ✏️ pour éditer → ajoute la balise juste après `<meta name="viewport" ...>` → "Commit changes"
   - Attends 2 minutes que Netlify republie le site
   - Retourne sur Search Console → clique sur **"Valider"**
6. Une fois validé, dans Search Console :
   - Va dans **"Sitemaps"** (menu de gauche)
   - Entre `sitemap.xml` dans la barre
   - Clique sur **"Envoyer"**

✅ Google sait maintenant que ton site existe. Il faut compter **2 à 6 semaines** pour qu'il commence à apparaître dans les résultats de recherche.

---

## ÉTAPE 9 — Compléter Google My Business (15 min) — TRÈS IMPORTANT pour le SEO local

Pour apparaître quand quelqu'un cherche "psychologue Bayonne" ou "psychologue Anglet", **Google My Business est le levier n°1**.

1. Va sur **https://business.google.com**
2. Crée une fiche avec :
   - **Nom** : Margaux Bezard — Psychologue
   - **Catégorie** : Psychologue
   - **Adresse** : adresse du cabinet à Anglet
   - **Zone desservie** : Anglet, Bayonne, Biarritz, Pays Basque
   - **Téléphone** : ton numéro pro
   - **Site web** : `https://margaux-bezard-psychologue.fr`
   - **Horaires** : tes vrais horaires
3. Google envoie un courrier postal avec un code de vérification (compter 1 à 2 semaines)
4. Une fois vérifiée, **demande à tes premiers clients de te laisser un avis Google** → c'est ce qui te fera vraiment décoller dans les résultats locaux.

---

## 📋 Ce qu'il reste à faire AVANT de communiquer le site

Avant de partager ton site, complète/modifie ces points avec Matthieu :

- [ ] **Mentions légales** (`mentions-legales.html`) : compléter l'adresse du cabinet, l'email, le n° ADELI et le SIRET
- [ ] **Schema.org** (dans `index.html`, balise `<script type="application/ld+json">`) : ajouter le numéro de téléphone
- [ ] **Balise canonical** dans `index.html` : remplacer `https://www.margaux-bezard-psychologue.fr/` par ton vrai domaine
- [ ] **Sitemap.xml** : remplacer le domaine pareil
- [ ] **Robots.txt** : remplacer le domaine pareil

> Matthieu peut éditer ces fichiers directement sur GitHub (clic sur le fichier → crayon → modifier → commit). Netlify republie automatiquement à chaque modification.

---

## 🔄 Pour modifier le site à l'avenir

À chaque fois que tu veux changer quelque chose (texte, tarif, ajouter une spécialité...) :

1. Va sur GitHub → ton repository
2. Clique sur le fichier à modifier (`index.html` pour le texte, `styles.css` pour le design)
3. Clique sur le crayon ✏️
4. Modifie
5. En bas, "Commit changes" avec un petit message du genre "Mise à jour tarif"
6. ✨ Netlify republie automatiquement en 1-2 minutes

---

## 💰 Coûts récurrents

| Service | Coût | Fréquence |
|---------|------|-----------|
| GitHub | 0€ | — |
| Netlify | 0€ | — |
| OVH (nom de domaine) | ~10€ | par an |
| **Total annuel** | **~10€** | |

---

## 🆘 En cas de problème

- **Mon site ne s'affiche pas avec mon nom de domaine** → c'est probablement la propagation DNS. Attends 24h max.
- **Netlify dit "Site not deployed"** → vérifie que tu as bien fait "Commit changes" sur GitHub.
- **HTTPS ne fonctionne pas** → dans Netlify, "Domain management" → "HTTPS" → "Verify DNS configuration" → "Provision certificate".
- **Tu as cassé quelque chose** → GitHub garde tout l'historique. Tu peux toujours revenir à la version précédente (onglet "History" du fichier).

---

## ✨ Récapitulatif des URL importantes

| Service | URL | À quoi ça sert |
|---------|-----|----------------|
| GitHub | https://github.com | Stocker les fichiers |
| Netlify | https://app.netlify.com | Publier le site |
| OVH | https://www.ovh.com/manager | Gérer le nom de domaine |
| Search Console | https://search.google.com/search-console | SEO Google |
| My Business | https://business.google.com | SEO local |

Bon courage Margaux ! Si tu bloques sur une étape, fais signe à Matthieu — il connaît le process. 💚
