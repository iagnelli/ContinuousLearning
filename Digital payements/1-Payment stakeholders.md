Certo. Pensa a una transazione carta/contactless su una VLT.

## I tre ruoli

### 1. Merchant

È **chi vende/incassa**.

Nel tuo caso potrebbe essere, a seconda del modello:

```markdown
Merchant = concessionario / operatore / POS / retailer / soggetto che incassa il pagamento
```

Esempio semplice:

> Se il player paga 20€ per caricare credito, il merchant è il soggetto a cui quei 20€ devono arrivare.

---

### 2. Acquirer

- è il soggetto autorizzato che consente al merchant di accettare pagamenti con carta/contactless e ricevere i fondi, secondo le regole dei circuiti di pagamento;

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

Un esempio pratico di **acquirer** in Italia è **Nexi**.

Nel suo sito, Nexi parla esplicitamente di **acquiring services** e di soluzioni per l’accettazione di pagamenti digitali, fisici e online da parte dei merchant. ([Nexi][1])

### Esempio VLT

```markdown
Player paga 20€ con carta/contactless sulla VLT
→ il merchant è il concessionario/operatore che incassa
→ l’acquirer, ad esempio Nexi, abilita quel merchant ad accettare pagamenti carta
→ il PSP/gateway gestisce tecnicamente il flusso della transazione
→ l’issuer, cioè la banca del player, autorizza o rifiuta il pagamento
→ se autorizzato, il credito viene caricato sulla VLT
```

Altri esempi di acquirer/payment provider da mappare sono **Worldline**, che ha una pagina italiana dedicata all’**Acquiring**, e **Adyen**, che opera come piattaforma pagamenti e acquiring in diversi mercati. ([Worldline][2])

La distinzione pratica è:

```markdown
Nexi / Worldline / Adyen = possono svolgere ruolo di acquirer o payment provider, a seconda del contratto e del modello.
Stripe / gateway / PSP = spesso percepiti come layer tecnico, ma alcuni possono offrire anche acquiring.
Banca del player = issuer.
Concessionario/operatore = merchant.
```

[1]: https://www.nexigroup.com/en/business/banks-and-financial-institutions/merchant-solutions-and-acquiring/?utm_source=chatgpt.com "Merchants and acquiring solutions"
[2]: https://worldline.com/it-it/home/main-navigation/solutions/merchants/acquiring?utm_source=chatgpt.com "Acquiring | Worldline Italia"



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

### Nota – Merchant, PSP, acquirer e issuer nel contesto VLT

Nel caso di pagamento digitale su VLT, i ruoli possono essere letti così:

- il **merchant** è il soggetto che incassa il pagamento del player, ad esempio il concessionario, l’operatore o il soggetto contrattualmente responsabile dell’incasso;

- il **PSP** è il provider che abilita tecnicamente il pagamento digitale sulla VLT o sull’ecosistema collegato, tramite terminale, gateway, API, QR code, wallet o integrazione con la piattaforma;

- l’**acquirer** è il soggetto che consente al merchant di accettare pagamenti con carta/contactless e di ricevere i fondi sul proprio conto, secondo le regole dei circuiti di pagamento;

- l’**issuer** è la banca o istituto del player, cioè il soggetto che autorizza o rifiuta la transazione quando il player usa carta, wallet o altro strumento collegato al proprio conto.


Esempio pratico VLT:
1. Il player vuole caricare 20€ di credito sulla VLT.
2. Usa carta/contactless, wallet o app.
3. Il PSP gestisce tecnicamente la richiesta di pagamento.
4. L’acquirer abilita l’accettazione della carta lato merchant.
5. L’issuer del player autorizza o rifiuta il pagamento.
6. Se il pagamento è autorizzato, il credito viene caricato sulla VLT.
7. La piattaforma registra credito, giocata, contatori, accounting e flussi verso ADM/Sogei.

Il punto critico è che il pagamento autorizzato non basta: nel gaming regolato deve essere riconciliato con il credito effettivamente caricato, la giocata, i contatori e il reporting ADM.
