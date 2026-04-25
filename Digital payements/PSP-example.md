Sì, quello che hai sentito probabilmente è **Aircash**.

È un esempio concreto da mappare, ma attenzione: da quello che emerge pubblicamente è più forte sul mondo **wallet / cash-to-wallet / gaming online / rete retail**, non necessariamente come soluzione diretta “pagamento contactless embedded sulla VLT”.

### Esempio pratico: Aircash

[Aircash](https://aircash.eu/it/) si presenta come una super-app/wallet per pagamenti, trasferimento denaro e servizi digitali. Ha anche una sezione specifica **Gaming** sul proprio sito. ([Aircash wallet][1])

Nel mercato gaming italiano, fonti di settore riportano casi di partnership Aircash per ricariche e prelievi legati al conto gioco, con logiche **cash-to-wallet** e utilizzo presso punti vendita/retail abilitati. ([JAMMA][2])

Quindi, per il tuo caso VLT/AWP, Aircash potrebbe essere interessante da contattare per capire se copre uno di questi modelli:

```markdown
- wallet digitale collegato al conto gioco;
- ricarica/prelievo presso rete retail;
- cash-to-wallet;
- wallet-to-gaming-account;
- eventuale pagamento tramite QR/app;
- riconciliazione tra transazione, wallet, conto gioco e operatore.
```

### Però non lo classificherei subito come “PSP per VLT embedded”

Per una VLT fisica, il caso più delicato è diverso:

```markdown
player → terminale/contactless/QR → PSP/acquirer → piattaforma VLT → credito di gioco → ADM/reporting
```

Qui devi verificare se Aircash può coprire:

* pagamento direttamente sulla macchina;
* integrazione con terminale fisico/unattended;
* flussi autorizzativi in real time;
* refund/reversal/timeout;
* riconciliazione con credito macchina;
* compatibilità con requisiti ADM;
* modello contrattuale con concessionario/retailer.

### Altri nomi da tenere in radar

Per confronto, nel mondo italiano/retail gaming emergono anche soluzioni come **ADMIRAL Pay / APay / Novomatic**, perché Novomatic comunica soluzioni di pagamento digitale e cashless collegate al proprio ecosistema VLT, inclusi riferimenti a e-wallet e pagamenti elettronici. ([Enada][3])

### Frase corretta per il README

```markdown
Esempi di provider/soluzioni da mappare nel mercato gaming retail:
- Aircash, per wallet, cash-to-wallet, gaming account e rete retail;
- soluzioni proprietarie di operatori/vendor gaming, come APay / ADMIRAL Pay / Novomatic, per modelli cashless più vicini all’ecosistema VLT;
- PSP/acquirer tradizionali, da valutare se il modello prevede carta/contactless direttamente su terminale o macchina.
```

La domanda giusta da fare ad Aircash non è “siete un PSP per VLT?”, ma:

> Quali modelli supportate per il gaming retail fisico: wallet, cash-to-wallet, QR/app payment, ricarica conto gioco, integrazione con terminale unattended o credito macchina?

[1]: https://aircash.eu/gaming/?utm_source=chatgpt.com "Gaming - Aircash wallet"
[2]: https://www.jamma.it/mercato/aircash-e-betpassion-nasce-la-partnership-per-i-pagamenti-cash-to-wallet-nel-gaming-online-italiano-348243?utm_source=chatgpt.com "Aircash e Betpassion: nasce la partnership per i pagamenti ..."
[3]: https://www.enada.it/it/dettaglio-profilo/NOVOMATIC%20ITALIA%20SPA?digitalProfileId=6896350&utm_source=chatgpt.com "NOVOMATIC ITALIA SPA"
