# Codice sconto Photosi, recupero automatico da shopilo.it

Modulo Python per il recupero automatico di **codici sconto Photosi** da [shopilo.it](https://shopilo.it/negozi/photosi.com). Restituisce **coupon Photosi** attivi in formato JSON, pronto per l'integrazione in un bot Telegram, estensione del browser o qualsiasi altro strumento.

**Pagina live:** [shopilo-it.github.io/codice-sconto-photosi](https://shopilo-it.github.io/codice-sconto-photosi/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Installazione

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-it/codice-sconto-photosi
cd codice-sconto-photosi
python fetch.py
```

## Output di esempio

```json
[
  {
    "store": "Photosi",
    "code": "SHOPILO20",
    "discount": "20%",
    "description": "20% di sconto su fotolibri e stampe",
    "expires": "2026-10-10",
    "source": "https://shopilo.it/negozi/photosi.com"
  }
]
```

## Coupon Photosi disponibili

| Sconto | Descrizione | Fonte |
|----------|-----------|-------|
| 20% | 20% di sconto su fotolibri e stampe | [shopilo.it](https://shopilo.it/negozi/photosi.com) |

Codici attivi: **[shopilo.it/negozi/photosi.com](https://shopilo.it/negozi/photosi.com)**

## Domande frequenti

### Come utilizzo un codice sconto Photosi?
Copia il codice dalla tabella qui sopra o da [shopilo.it](https://shopilo.it/negozi/photosi.com), aggiungi i prodotti al carrello su Photosi e inserisci il codice al checkout nel campo dedicato.

### Quanto durano i coupon Photosi?
Ogni coupon ha una data di scadenza indicata nella colonna "Scadenza". Lo script fetch.py restituisce solo i coupon attivi al momento dell'esecuzione.

### Dove trovo i voucher Photosi piu recenti?
La pagina [shopilo.it/negozi/photosi.com](https://shopilo.it/negozi/photosi.com) viene aggiornata quotidianamente con i codici sconto Photosi, voucher Photosi e coupon promozionali Photosi piu recenti.

### Il codice non funziona. Cosa faccio?
Verifica la data di scadenza e le condizioni (importo minimo del carrello, prodotti idonei). Alcuni codici sono validi solo nell'app mobile o per il primo ordine.

## Informazioni su Photosi

Photosi e uno dei negozi online piu popolari. Su [shopilo.it](https://shopilo.it/negozi/photosi.com) trovi i migliori codici sconto Photosi, coupon Photosi verificati e voucher Photosi attivi, aggiornati ogni giorno.

## Installazione npm

```bash
npm install codice-sconto-photosi
```

```javascript
const { fetchCoupons } = require('codice-sconto-photosi');
fetchCoupons().then(data => console.log(data));
```

## Licenza

MIT, dati prelevati da [shopilo.it](https://shopilo.it)
