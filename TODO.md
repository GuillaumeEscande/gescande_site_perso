# TODO — Refonte site perso escande.ovh

## 🔴 Critique (bloquants ou incohérences visibles)

- [ ] **Incohérence certification AWS** : la section Compétences dit "AWS Architect Associate" mais les certifications affichent le badge Professional. Décider laquelle est la bonne et aligner les deux endroits dans `index.html`.
- [ ] **TOGAF** : Mettre à jour le statut (obtenu ou toujours en cours ?). Si obtenu, ajouter le lien vers le PDF et retirer le badge "En cours".
- [ ] **Favicon** : Aucun favicon sur le site actuellement. Créer un fichier `favicon.ico` (ou `favicon.svg`) avec le monogramme "G.E" stylisé et l'ajouter dans `<head>`.

---

## 🟠 Contenu à compléter ou clarifier

### Section "À Propos"
- [ ] Confirmer / affiner le texte : tu es "chez Obeo" ET disponible en freelance en parallèle, ou tu es en transition ? Adapter la formulation.
- [ ] Ajouter 1-2 phrases sur ce qui te différencie en tant que consultant (ton "why").
- [ ] Compléter les **statistiques** en haut de la section About :
  - "10+ ans d'expérience" → vérifier l'exact (depuis 2013 = ~13 ans)
  - "6+ projets majeurs" → mettre le nombre réel

### Section "Services Freelance"
- [ ] Préciser ta **disponibilité réelle** : immédiate, à partir de quelle date, jours/semaine.
- [ ] Ajouter (optionnel mais recommandé) : **TJM ou fourchette de prix**, ou au moins "Devis sur demande".
- [ ] Préciser les **modes d'intervention** : full remote, présentiel Toulouse, déplacements France entière ?
- [ ] Durée minimale de mission : mission one-shot ou engagement minimum (ex. 5 jours) ?
- [ ] Statut juridique freelance : micro-entrepreneur, SASU, portage salarial ? À mentionner si pertinent.

### Section "Expérience"
- [ ] **Obeo (poste actuel)** : les détails sont très courts (CDK, Ansible, Proxmox, GitOps, Cloudwatch). Compléter avec 4-5 technos/sujets supplémentaires pour mieux refléter l'activité réelle.
- [ ] Ajouter éventuellement un lien vers les **talks ou articles publiés** sur chaque expérience.

### Section "Compétences"
- [ ] Revoir le niveau "Expert" sur Système si tu te considères plutôt "Maître/Senior" pour rester cohérent.
- [ ] Ajouter **K8S / Kubernetes** dans la section Cloud ou Système (tu l'as dans l'expérience GS2.0 mais pas dans les compétences).

---

## 🟡 Visuels à fournir ou améliorer

- [ ] **Photo de profil professionnelle** (`images/profil.jpg`) : la photo actuelle est utilisée, mais pour un site vitrine freelance une photo professionnelle récente (fond neutre, bonne lumière) est fortement recommandée.
- [ ] **OG Image** : créer une image 1200×630px pour les partages sur réseaux sociaux (aperçu LinkedIn, etc.) — peut être un bandeau "Guillaume Escande — Architecte Cloud & DevOps" sur fond sombre avec les couleurs du site.
- [ ] **Favicon** : voir section Critique ci-dessus.
- [ ] Les GIFs d'illustration (`diy.gif`, `sport.gif`, `familly.gif`) : ils fonctionnent mais sont petits (64px) dans la nouvelle mise en page. Envisager des illustrations SVG ou des photos plus modernes si disponibles.
- [ ] **Images AWS** : vérifier que `aws-certified-solutions-architect-professional.png` correspond bien à la certification détenue (et non associate).

---

## 🟢 Améliorations optionnelles (nice to have)

### SEO & Méta
- [ ] Mettre à jour le `<meta name="description">` avec une formulation orientée freelance.
- [ ] Ajouter `<meta name="theme-color" content="#070b14">` pour le navigateur mobile.
- [ ] Ajouter un `sitemap.xml` si référencement important.

### Contenu additionnel
- [ ] **Section "Projets"** (optionnel) : une galerie de 3-4 projets DIY ou open source avec lien GitHub. Donne de la crédibilité technique.
- [ ] **Témoignages clients** (optionnel) : si tu as des références de missions passées, 2-3 témoignages courts seraient très efficaces pour la partie freelance.
- [ ] **Blog / Articles** : si tu écris sur Medium ou ailleurs, ajouter un lien dans la nav et une section dédiée.
- [ ] **Section "Liens utiles"** : vérifier que tous les liens sont encore actifs et pertinents en 2025.

### Social / Contact
- [ ] **LinkedIn** : vérifier que le lien `https://www.linkedin.com/in/guillaume-escande-architect/` est toujours valide.
- [ ] **Téléphone** : le numéro `06 86 06 56 16` a été retiré du site dans cette refonte (pour limiter le spam). Tu peux le remettre dans la section contact si tu souhaites.
- [ ] **Facebook** : le lien Facebook a été retiré. Si tu veux le remettre, ajouter dans la section social du footer.

### Technique
- [ ] Remplacer `https://cdn.tailwindcss.com` (CDN dev) par une version buildée pour la production (pas critique mais meilleures performances).
- [ ] Supprimer l'import jQuery de `scripts/scroll-active.js` (plus utilisé dans la nouvelle version).
- [ ] Ajouter un `robots.txt` si pas encore présent sur le serveur.

---

## ✅ Déjà fait dans cette refonte

- [x] Refonte visuelle complète (dark theme, gradient cyan/violet)
- [x] Navbar fixe avec effet scroll et menu mobile
- [x] Section Hero full-screen avec orbes animés et typewriter
- [x] Nouvelle section "Services Freelance" avec 4 offres détaillées
- [x] Timeline expérience repensée (alternée desktop / mobile friendly)
- [x] Skills en pill tags (suppression des étoiles et GIFs)
- [x] Certifications en cartes
- [x] Section Intérêts, Liens, Médias convertis en Tailwind (anciens CSS cassés réparés)
- [x] Section Contact dédiée avec CTA
- [x] Footer
- [x] Scroll reveal animations (IntersectionObserver)
- [x] Active nav link highlighting
- [x] Suppression de la dépendance jQuery
- [x] Compatibilité desktop & mobile
