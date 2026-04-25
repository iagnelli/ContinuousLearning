Certo. Pensa a una transazione carta/contactless su una VLT.

## I tre ruoli

### 1. Merchant

È **chi vende/incassa**.

Nel tuo caso potrebbe essere, a seconda del modello:

```markdown
Merchant = concessionario / operatore / soggetto che incassa il pagamento
```

Esempio semplice:

> Se il player paga 20€ per caricare credito, il merchant è il soggetto a cui quei 20€ devono arrivare.

---

### 2. Acquirer

È **la banca o istituto che abilita il merchant ad accettare pagamenti con carta**.

L’acquirer:

* apre il rapporto contrattuale con il merchant;
* permette di accettare carte Visa/Mastercard ecc.;
* riceve l’esito dai circuiti;
* accredita i fondi al merchant, secondo le regole contrattuali;
* gestisce parte del rischio lato merchant.

In parole semplici:

```markdown
Acquirer = la “banca lato esercente” che consente al merchant di incassare pagamenti carta.
```

---

### 3. PSP

È **il provider tecnologico/operativo che fa funzionare il pagamento**.

Il PSP:

* fornisce gateway/API;
* collega macchina, app, terminale o piattaforma al sistema di pagamento;
* instrada la transazione;
* restituisce esito autorizzato/negato;
* gestisce timeout, errori, refund, reportistica tecnica;
* può anche offrire servizi di riconciliazione.

In parole semplici:

```markdown
PSP = il soggetto tecnico che integra e orchestra il pagamento.
```

---

## Esempio pratico VLT

Scenario: il player appoggia la carta/contactless per caricare 20€.

```markdown
Player
→ paga 20€ con carta/contactless
→ terminale/device sulla VLT
→ PSP gestisce tecnicamente la transazione
→ acquirer abilita l’accettazione carta lato merchant
→ issuer autorizza il pagamento
→ merchant riceve i fondi
→ piattaforma VLT carica 20€ di credito
→ sistema registra credito/giocata/contatori/flussi ADM
```

---

## Differenza secca

```markdown
Merchant = chi incassa.
Acquirer = chi permette al merchant di accettare carte e ricevere i fondi.
PSP = chi fornisce la tecnologia/processo per far passare il pagamento.
Issuer = banca del cliente/player che autorizza o rifiuta il pagamento.
```

## Mini esempio non gaming

Quando paghi su un e-commerce:

```markdown
Cliente = tu
Merchant = negozio online
PSP = Stripe / Nexi / Adyen / PayPal gateway
Acquirer = soggetto che consente al negozio di accettare carte
Issuer = la tua banca
Circuito = Visa / Mastercard
```

## Nel README puoi inserirlo così

```markdown
### Nota – Merchant, PSP e acquirer

Nel modello di pagamento digitale:

- il **merchant** è il soggetto che incassa il pagamento;
- il **PSP** abilita tecnicamente il pagamento tramite gateway, API, terminale o integrazione;
- l’**acquirer** consente al merchant di accettare pagamenti carta e ricevere i fondi;
- l’**issuer** è la banca o istituto del cliente/player che autorizza o rifiuta la transazione.

Nel contesto VLT/AWP, questi ruoli devono essere chiariti fin dall’inizio perché impattano responsabilità, compliance, flussi contabili, riconciliazione e controllo ADM.
```
