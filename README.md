# 🪙 Cryptax

Calculateur d'impôt crypto pour les déclarations **Canada / Québec** — conçu pour les exports CSV de **NDAX**.

## Fonctionnalités

- **Import CSV** — Glissez-déposez vos fichiers NDAX (trades + staking)
- **Prix de base rajusté (PBR/ACB)** — Calcul automatique par la méthode du coût moyen pondéré (exigée par l'ARC)
- **Revenu de staking** — Évalué à la juste valeur marchande via l'API CoinGecko
- **Résumé fiscal** — Montants à déclarer et lignes de formulaire (T1 / TP-1)

## Utilisation

1. Ouvrez `index.html` dans votre navigateur
2. Importez vos fichiers CSV NDAX (trades et staking)
3. Cliquez **Calculer**
4. Consultez les 3 onglets : Trades & ACB, Staking, Résumé fiscal

> Aucune installation requise — tout est dans un seul fichier HTML.

## Calculs fiscaux

### ACB (Prix de base rajusté)
- Méthode du coût moyen pondéré pour chaque actif
- Inclut les achats **et** les récompenses de staking comme acquisitions
- Les frais de transaction sont automatiquement pris en compte

### Revenu de staking
- Les récompenses sont évaluées en CAD au prix du jour (via CoinGecko)
- À déclarer comme **autres revenus** :
  - Fédéral (T1) : Ligne 13000
  - Québec (TP-1) : Ligne 154

## Technologies

- HTML / CSS / JavaScript (aucun framework)
- [Papa Parse](https://www.papaparse.com/) pour le parsing CSV
- [CoinGecko API](https://www.coingecko.com/) pour les prix historiques
- [Inter](https://fonts.google.com/specimen/Inter) (Google Fonts)

## Avertissement

Cet outil est fourni à titre informatif seulement. Ce n'est pas un avis fiscal professionnel. Consultez un comptable ou un fiscaliste pour votre situation particulière.
