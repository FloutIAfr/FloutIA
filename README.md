<div align="center">

# FloutIA

**Profitez de ChatGPT, Claude ou Gemini sans jamais leur confier vos données sensibles.**

*100 % local • Zéro serveur • Zéro inscription • Fonctionne hors-ligne*

[Accéder à l'outil en ligne](https://floutia.fr) · [Signaler un bug](mailto:contact@floutia.fr) · [Politique de sécurité](SECURITY.md)

![Aperçu de FloutIA](preview.png)

</div>

---

## Pourquoi FloutIA ?

Chaque jour, des millions de messages professionnels, contrats, tableaux Excel ou logs d'erreurs sont collés dans des IA avec des noms de clients, des RIB, des numéros de Sécurité sociale ou des clés API.

**FloutIA agit comme un sas de protection 100 % local dans votre navigateur :**
1. **Collez ou importez** votre texte, votre fichier Excel (`.xlsx` / `.csv`) ou vos logs.
2. **FloutIA remplace automatiquement** les données sensibles par des étiquettes (`[PERSONNE_1]`, `[IBAN_1]`) ou des noms fictifs.
3. **Envoyez** la version protégée à votre IA (ou téléchargez le `.xlsx` protégé).
4. **Collez la réponse de l'IA** : FloutIA remet vos vraies données exactement à leur place.

---

## Ce que FloutIA protège automatiquement

| Catégorie | Exemples détectés | Remarques |
| :--- | :--- | :--- |
| **Identité & Contact** | Emails, téléphones FR, civilités (`M.`, `Mme`…), adresses postales | Sélection manuelle en 1 clic pour les noms isolés |
| **Banque & Administratif** | IBAN (tous pays), BIC (en contexte), NIR (clé 97), SIREN/SIRET (Luhn), montants | Zéro faux positif sur les numéros aléatoires |
| **Excel & Tableaux** | Fichiers `.xlsx` (multi-feuilles), `.csv`, `.tsv`, copier-coller Excel | Export direct en `.xlsx` protégé |
| **Code, Logs & Configs** | Clés API (`sk-...`, `ghp_...`, `AKIA...`), JWT, Bearer/Basic, `.env`, IPv4/IPv6, chemins | Préserve les noms de variables et la structure du code |

---

## Comment vérifier la sécurité vous-même ?

FloutIA n'utilise **aucun serveur de traitement**, **aucun cookie** et **aucune dépendance CDN externe**. La page embarque une politique de sécurité stricte (`connect-src 'none'`).

1. Ouvrez `https://floutia.fr` et appuyez sur `F12` (onglet **Réseau**).
2. Collez un texte ou importez un fichier `.xlsx`, puis masquez et restaurez : **0 requête sortante** n'apparaît.
3. Coupez votre Wi-Fi : l'outil continue de fonctionner normalement.

---

## Utilisation 100 % locale (sur votre ordinateur)

Pour les environnements les plus sensibles, vous pouvez télécharger `index.html` et l'ouvrir directement en local (`file://`) sans connexion Internet.

---

## Limites à connaître

- **Pseudonymisation, pas anonymisation RGPD :** le remplacement est réversible pendant la session (stocké uniquement en mémoire vive, détruit à la fermeture de l'onglet).
- **Détection heuristique :** relisez toujours le texte protégé avant de l'envoyer à une IA.
- **Noms fictifs :** si l'IA abrège un nom (*« Camille »* au lieu de *« Camille Laurent »*), préférez le mode **Étiquettes** (activé par défaut).

---

## Licence & Contact

© 2026 FloutIA — Tous droits réservés.  
Conçu en France • Contact : **contact@floutia.fr**
