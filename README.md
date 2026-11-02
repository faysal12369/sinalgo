# SinalGo — Encaissement des coursiers

Application Android utilisée par les coursiers pour encaisser les règlements des clients à la livraison : scan du bon de livraison sur terminal Honeywell, saisie du paiement, signature du client et position GPS.

> Projet réalisé par **Fayçal Gheroufella** chez SINAL (distribution optique, Algérie). Le code source appartient à l'entreprise et reste privé ; démonstration possible en entretien.

## Fonctionnalités

- Scan du bon de livraison avec le lecteur intégré des terminaux **Honeywell** (SDK Data Collection / AIDC via `honeywell_scanner`), avec repli sur la caméra du téléphone (`mobile_scanner`)
- Vérification du bon côté serveur : s'il est déjà payé, alerte ; sinon ouverture de l'écran de règlement
- Saisie du règlement, **signature du client** à l'écran et **géolocalisation** de l'encaissement
- Tableau de bord coursier, tableau de bord administrateur et historique
- Deux rôles : administrateur et coursier
- API PHP / MySQL protégée par un en-tête d'autorisation

## Technologies

Flutter · Dart · provider · http · signature · geolocator · honeywell_scanner · mobile_scanner · PHP 8 · MySQL (PDO) · WinDev Mobile (v1)

## En chiffres

16 fichiers Dart (~5 400 lignes) · API PHP d'environ 830 lignes  
Version 1 en WinDev Mobile (oct. 2025 – janv. 2026), réécrite en Flutter (févr. – mars 2026).

## Organisation du projet

- `app/` — application Flutter (Android)
- `backend/` — API PHP (login, clients, vérification BL, règlements, tableaux de bord, historique)

## Contact

gheroufellafaycal@gmail.com · [LinkedIn](https://linkedin.com/in/faysal-gheroufella-4a7969355)
