# Code promo Conforama, recuperation automatique depuis shopilo.fr

Module Python pour la recuperation automatique de **codes promo Conforama** depuis [shopilo.fr](https://shopilo.fr/reductions/conforama.fr). Renvoie les **coupons Conforama** actifs au format JSON, pret a etre integre dans un bot Telegram, une extension de navigateur ou tout autre outil.

**Page live :** [shopilo-fr.github.io/code-promo-conforama](https://shopilo-fr.github.io/code-promo-conforama/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Installation

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-fr/code-promo-conforama
cd code-promo-conforama
python fetch.py
```

## Exemple de sortie

```json
[
  {
    "store": "Conforama",
    "code": "SHOPILO10",
    "discount": "10%",
    "description": "10% de reduction sur les meubles et la decoration",
    "expires": "2026-10-13",
    "source": "https://shopilo.fr/reductions/conforama.fr"
  }
]
```

## Coupons Conforama disponibles

| Reduction | Description | Source |
|----------|-----------|-------|
| 10% | 10% de reduction sur les meubles et la decoration | [shopilo.fr](https://shopilo.fr/reductions/conforama.fr) |

Codes actifs : **[shopilo.fr/reductions/conforama.fr](https://shopilo.fr/reductions/conforama.fr)**

## Questions frequentes

### Comment utiliser un code promo Conforama ?
Copiez le code depuis le tableau ci-dessus ou depuis [shopilo.fr](https://shopilo.fr/reductions/conforama.fr), ajoutez les produits a votre panier sur Conforama et saisissez le code au moment du paiement dans le champ prevu.

### Combien de temps durent les coupons Conforama ?
Chaque coupon a une date d'expiration indiquee dans la colonne "Expiration". Le script fetch.py renvoie uniquement les coupons actifs au moment de l'execution.

### Ou trouver les bons de reduction Conforama les plus recents ?
La page [shopilo.fr/reductions/conforama.fr](https://shopilo.fr/reductions/conforama.fr) est mise a jour quotidiennement avec les codes promo Conforama, bons de reduction Conforama et coupons promotionnels Conforama les plus recents.

### Le code ne fonctionne pas. Que faire ?
Verifiez la date d'expiration et les conditions (montant minimum de commande, produits eligibles). Certains codes sont valables uniquement sur l'application mobile ou pour la premiere commande.

## A propos de Conforama

Conforama est l'une des boutiques en ligne les plus populaires. Sur [shopilo.fr](https://shopilo.fr/reductions/conforama.fr), retrouvez les meilleurs codes promo Conforama, coupons Conforama verifies et bons de reduction Conforama actifs, mis a jour chaque jour.

## Installation npm

```bash
npm install code-promo-conforama
```

```javascript
const { fetchCoupons } = require('code-promo-conforama');
fetchCoupons().then(data => console.log(data));
```

## Licence

MIT, donnees extraites de [shopilo.fr](https://shopilo.fr)
