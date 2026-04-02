# Cod reducere eMAG — fetch automat de pe shopilo.ro

Modul Python pentru fetch automat de **coduri de reducere eMAG** de pe [shopilo.ro](https://shopilo.ro/magazin/emag.ro). Returneaza **cupoane eMAG** active in format JSON, gata de integrat intr-un bot Telegram, extensie de browser sau orice alt tool.

**Pagina live:** [shopilo-ro.github.io/cod-reducere-emag](https://shopilo-ro.github.io/cod-reducere-emag/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Instalare

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-ro/cod-reducere-emag
cd cod-reducere-emag
python fetch.py
```

## Output exemplu

```json
[
  {
    "store": "eMAG",
    "code": "SHOPILO30",
    "discount": "30%",
    "description": "30% extra reducere cu Genius Deals",
    "expires": "2026-10-02",
    "source": "https://shopilo.ro/magazin/emag.ro"
  }
]
```

## Cupoane eMAG disponibile

| Reducere | Descriere | Sursa |
|----------|-----------|-------|
| 30% | 30% extra reducere cu Genius Deals | [shopilo.ro](https://shopilo.ro/magazin/emag.ro) |

Codurile active: **[shopilo.ro/magazin/emag.ro](https://shopilo.ro/magazin/emag.ro)**

## Intrebari frecvente

### Cum folosesc un cod de reducere eMAG?
Copiaza codul din tabelul de mai sus sau de pe [shopilo.ro](https://shopilo.ro/magazin/emag.ro), adauga produsele in cos pe eMAG, si introdu codul la checkout in campul dedicat.

### Cat timp sunt valabile cupoanele eMAG?
Fiecare cupon are data de expirare afisata in coloana "Expira". Scriptul fetch.py returneaza doar cupoanele active la momentul rularii.

### Unde gasesc cele mai noi voucher-uri eMAG?
Pagina [shopilo.ro/magazin/emag.ro](https://shopilo.ro/magazin/emag.ro) este actualizata zilnic cu cele mai noi cod reducere eMAG, voucher eMAG si cupon promotional eMAG.

### Codul nu functioneaza. Ce fac?
Verifica data de expirare si conditiile (valoare minima cos, produse eligibile). Unele coduri sunt valabile doar in aplicatia mobila sau pentru prima comanda.

## Despre eMAG

eMAG este unul dintre magazinele online populare. Gasesti pe [shopilo.ro](https://shopilo.ro/magazin/emag.ro) cele mai bune cod reducere eMAG, cupoane eMAG verificate si voucher eMAG active, actualizate zilnic.

## Instalare npm

```bash
npm install cod-reducere-emag
```

```javascript
const { fetchCoupons } = require('cod-reducere-emag');
fetchCoupons().then(data => console.log(data));
```

## Licenta

MIT — date sursa de pe [shopilo.ro](https://shopilo.ro)
