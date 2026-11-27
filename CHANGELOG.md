# Changelog

Toutes les modifications notables de FloutIA sont listées ici.
Le format suit [Keep a Changelog](https://keepachangelog.com/fr/1.1.0/) et le versionnage suit [SemVer](https://semver.org/lang/fr/).

## [Non publié]

### Ajouté
- Pages de contenu : `anonymiser-excel-chatgpt`, `masquer-cles-api-logs`, `pseudonymiser-donnees-rgpd`.
- Favicons (`favicon.svg`, `favicon.png`, `favicon.ico`).

### Modifié
- Mention RGPD des pages de contenu : le site ne transmet ni ne stocke les documents ; le formulaire de retour (Tally) est décrit dans les mentions légales.

## [1.1.0] - 2026-11-27

### Ajouté
- Démo « avant / après » dans le héros, avec animation de floutage (désactivée si le mouvement réduit est demandé) et bouton « Essayer cet exemple ».
- Liens profonds `#excel` et `#code` : ouvrent directement l'onglet correspondant.
- Infobulle au survol d'un jeton protégé, qui affiche la donnée d'origine (`data-orig`).

### Modifié
- Nouvelle charte : palette navy, titres en serif, jetons masqués en caviardage navy (inversé en mode sombre), restauration en vert.
- Badge d'en-tête : « 100 % local, rien n'est envoyé ».
- Textes d'aide raccourcis. La limite de 500 000 caractères reste appliquée, avec un message d'erreur.
- Accord des pluriels dans les compteurs (caractère / caractères, mot / mots).

### Corrigé
- Marge du héros : la règle `.container` annulait l'espacement du `<main>` (0 px au lieu de 34 px).
- Pied de panneau gauche (compteur et bouton « Masquer mes données ») aligné en bas du panneau.

## [1.0.0] - 2026-11-27

### Ajouté
- Pseudonymisation réversible locale de texte, d'emails, d'IBAN, de NIR, de coordonnées, de logs et de secrets `.env`.
- Traitement de fichiers `.xlsx` multi-feuilles et `.csv`, avec export natif, lecture par `DecompressionStream`.
- Validateurs Luhn (SIREN/SIRET) et clé 97 (NIR).
- Restauration automatique des données dans la réponse de l'IA.
- Liste de mots personnalisée, mémorisée uniquement si l'utilisateur le demande.
- Politique de sécurité stricte : `connect-src 'none'`, `form-action 'none'`, `referrer no-referrer`.
- Mentions légales et page « Confidentialité & limites ».
- Tests intégrés exécutables depuis la page.
