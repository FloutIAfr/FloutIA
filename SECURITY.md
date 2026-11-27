# Politique de sécurité

## Signaler une vulnérabilité

Si vous découvrez une faille de sécurité, **ne l'ouvrez pas en issue publique**.

Écrivez à **contact@floutia.fr** avec :

- une description de la vulnérabilité ;
- les étapes pour la reproduire, avec des données fictives ;
- l'impact potentiel.

Nous accusons réception sous 48 h et publions un correctif dans les meilleurs délais (objectif : 7 jours pour les failles critiques).

## Audit de sécurité

FloutIA a été conçu avec les principes suivants :

- zéro requête réseau depuis l'outil (CSP stricte `connect-src 'none'`) ;
- aucune dépendance externe ni CDN ;
- validation des entrées et limites contre le gel de la page ;
- 33 tests unitaires intégrés, exécutables dans le navigateur.

Le code s'exécute intégralement côté client et peut être inspecté directement depuis votre navigateur.
