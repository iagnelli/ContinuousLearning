# Digital Payments for VLT/AWP – Learning Path

## Obiettivo

Costruire una competenza credibile su **pagamenti digitali applicati a macchine retail regolamentate**, con focus su VLT/AWP.

Il posizionamento da sviluppare è:

> Program / Platform Manager con expertise in digital payments for regulated retail gaming.

Nel contesto VLT/AWP, il pagamento digitale introduce una **doppia catena di controllo**:

- la catena **bancaria/payments**, presidiata da Banca d’Italia, autorità europee, PSP/acquirer e standard di sicurezza come PCI;
- la catena **gaming regolata**, presidiata da ADM/Sogei e dai laboratori di certificazione.

La differenza chiave è questa:
> Nel banking viene controllato il pagamento come operazione finanziaria; nel gaming viene controllato il credito di gioco e la sua corretta tracciabilità nel sistema regolato ADM.

<details>

**In ambito bancario / pagamenti**
Il controllo è principalmente in capo a:
Banca d’Italia, per vigilanza su banche, istituti di pagamento, istituti di moneta elettronica e sistema dei pagamenti.
EBA / BCE / autorità europee, per framework europeo, PSD2/PSD3/PSR, SCA, instant payments, open banking.
UIF, per la parte antiriciclaggio e segnalazioni di operazioni sospette. La UIF è collocata presso Banca d’Italia ma opera in autonomia e indipendenza.
Quindi, se parliamo di pagamento come servizio finanziario, la logica è:
Banca d’Italia / autorità europee / UIF.

**Nel gioco pubblico regolato**
Il controllo è principalmente in capo a:
ADM – Agenzia delle Dogane e dei Monopoli, che presidia il settore dei giochi pubblici, tutela gli interessi erariali e governa la legalità del gioco.
Sogei / sistema di controllo, per la parte tecnica di raccolta, trasmissione e controllo dei dati di gioco.
Laboratori di certificazione, come GLI, per verifiche tecniche/certificative prima dell’autorizzazione.
Quindi, se parliamo di giocata, credito sulla macchina, contatori, flussi ADM, VLT/AWP e rendicontazione di gioco, la logica è:
ADM / Sogei / laboratorio di certificazione.

</details>

Per questo non serve diventare “esperta bancaria pura”.  
Serve saper governare l’intersezione tra:

- pagamento autorizzato
- credito caricato sulla macchina
- giocata
- vincita / payout
- contatori
- accounting
- riconciliazione
- reporting verso ADM
- sicurezza e responsabilità operative

Il valore del ruolo è quindi guidare un programma che combina:

- pagamenti digitali
- hardware / terminali / acceptance
- compliance e controlli ADM/regolatori
- sicurezza
- accounting, riconciliazione e reporting verso autorità
- operations su rete retail
- impatti regolatori nel gaming

### Postilla – Come avviene il controllo

Nel mondo **bancario/payments**, il controllo riguarda la correttezza e sicurezza dell’operazione di pagamento:

- autorizzazione del pagamento;
- autenticazione del pagatore;
- gestione del rischio frode;
- ruolo di issuer, acquirer, PSP e circuiti;
- protezione dei dati di pagamento;
- settlement e riconciliazione finanziaria.

Nel mondo **gaming regolato**, il controllo riguarda invece la coerenza tra pagamento, credito di gioco e dati regolatori:

- credito effettivamente caricato sulla macchina;
- giocata effettuata;
- vincita o payout;
- contatori di macchina e di sistema;
- flussi verso ADM/Sogei;
- tracciabilità, auditabilità e riconciliazione contabile.

Il punto critico del progetto VLT/AWP è quindi la **riconciliazione tra pagamento autorizzato, credito caricato, dati di gioco, contatori e reporting ADM**.
---

## Perché è rilevante per il contesto VLT/AWP

Oggi le macchine usano prevalentemente accettatori di banconote.  
L’introduzione dei pagamenti digitali cambia il perimetro del progetto: non è solo hardware, ma un’iniziativa **platform + compliance + security + operations**.

Le domande chiave da governare saranno:

- Il pagamento sarà sulla singola macchina, su device esterno o tramite wallet/club card?
- Sarà carta/contactless, mobile wallet, A2A/instant payment o mix?
- Chi certifica device, firmware, host, integrazione e flussi contabili?
- Come cambiano accounting, riconciliazione ADM, DWH e reporting?
- Come si gestiscono chargeback, refund, reversal, timeout e scenari offline?
- Come si dividono le responsabilità tra platform owner, PSP, acquirer, hardware vendor, operations e retailer?

---

## Learning Path consigliato

### 1. Base digital payments

**Risorse principali**

- [CFTE – Payments Online Masterclass](https://courses.cfte.education/payments-online-masterclass-free-digital-payments-course/)
- [Coursera – The Future of Payment Technologies](https://www.coursera.org/learn/paytech)
- [Coursera – FinTech: Foundations, Payments, and Regulations](https://www.coursera.org/learn/wharton-fintech-overview-payments-regulations)

**Perché serve**

Costruisce il linguaggio base su:

- payment ecosystem
- issuer, acquirer, PSP, gateway, processor, merchant
- card payments
- wallet
- account-to-account
- open banking
- payment processing
- regolamentazione dei pagamenti

---

### 2. Acceptance, contactless e terminali fisici

**Risorse principali**

- [EMVCo – Educational Videos](https://www.emvco.com/knowledge-hub-category/educational-videos/)
- [EMVCo – Knowledge Hub](https://www.emvco.com/knowledge-hub/)
- [EMVCo – EMV Contactless Chip](https://www.emvco.com/emv-technologies/emv-contactless-chip/)
- [EMVCo – Technical Resources](https://www.emvco.com/resources/)
- [EMVCo – Contactless Product Approval Process](https://www.emvco.com/processes/contactless-product-approval-process/)

**Perché serve**

È il blocco più vicino al contesto VLT/AWP, perché riguarda pagamenti su dispositivi fisici e potenzialmente unattended.

Da capire bene:

- EMV
- contactless
- NFC wallet
- terminali embedded/unattended
- differenza tra POS tradizionale e device integrato
- dipendenze hardware / firmware / host / acquirer
- test e approval dei terminali

---

### 3. Sicurezza pagamenti

**Risorsa principale**

- [PCI SSC – PCI Awareness Training](https://www.pcisecuritystandards.org/program_training_and_qualification/requirements_awareness/)
- [PCI SSC – PCI Professional Qualification](https://www.pcisecuritystandards.org/program_training_and_qualification/pci_professional_qualification/)
- [PCI SSC – Internal Security Assessor Qualification](https://www.pcisecuritystandards.org/program_training_and_qualification/internal_security_assessor_certification/)

**Perché serve**

Se entrano carte/contactless/NFC, entrano anche temi PCI.

Da approfondire:

- PCI DSS
- protezione dati carta
- segmentazione rete
- hardening device
- audit trail
- incident management
- responsabilità tra operatore, acquirer, terminal vendor e integratore

---

### 4. Regolamentazione pagamenti

**Fonti principali**

- [Banca d’Italia – Verso la revisione della PSD2](https://www.bancaditalia.it/compiti/sispaga-mercati/comitato-pagamenti-italia/CPI-Tavolo-Revisione-PSD2.pdf)
- [EBA – Educational Seminars](https://www.abe-eba.eu/training-education/eba-summer-winter-schools-and-other-educational-seminars/)
- [EBA – Strong Customer Authentication and secure communication](https://www.eba.europa.eu/legacy/regulation-and-policy/regulatory-activities/payment-services-and-electronic-money-0)
- [European Central Bank – Instant Payments Regulation](https://www.ecb.europa.eu/paym/retail/instant_payments/html/instant_payments_regulation.en.html)

**Perché serve**

Serve per capire le implicazioni regolatorie del modello scelto.

Da approfondire:

- SCA
- open banking
- instant payments
- responsabilità del merchant
- ruolo di PSP, acquirer e provider
- rischio operativo e antifrode

---

### 5. Rail, settlement e riconciliazione

**Fonti principali**

- [European Payments Council – SEPA Instant Credit Transfer Rulebook](https://www.europeanpaymentscouncil.eu/what-we-do/epc-payment-schemes/sepa-instant-credit-transfer/sepa-instant-credit-transfer-rulebook)
- [ISO 20022 – Official Overview](https://www.iso20022.org/iso-20022)
- [Swift – ISO 20022 / Training Catalogue](https://www.swift.com/myswift/services/training/swift-training-catalogue)

**Perché serve**

Non serve diventare specialista di messaggistica bancaria, ma bisogna capire le implicazioni su:

- settlement real-time vs batch
- riconciliazione
- structured data
- reporting
- accounting
- possibili evoluzioni verso A2A / instant funding / request-to-pay

---

## Ordine pratico consigliato

### Fase 1 – Base veloce

1. [CFTE – Payments Online Masterclass](https://courses.cfte.education/payments-online-masterclass-free-digital-payments-course/)
2. [Coursera – The Future of Payment Technologies](https://www.coursera.org/learn/paytech)

### Fase 2 – Regole e payment ecosystem

3. [Coursera – FinTech: Foundations, Payments, and Regulations](https://www.coursera.org/learn/wharton-fintech-overview-payments-regulations)
4. Materiali Banca d’Italia / EBA su PSD2, PSD3, PSR, SCA e instant payments

### Fase 3 – Specifico VLT/AWP

5. [EMVCo – Educational Videos](https://www.emvco.com/knowledge-hub-category/educational-videos/) + [EMVCo – Knowledge Hub](https://www.emvco.com/knowledge-hub/)
6. Studio su contactless, terminali embedded/unattended e approval process

### Fase 4 – Sicurezza e programma

7. [PCI Awareness Training](https://www.pcisecuritystandards.org/program_training_and_qualification/requirements_awareness/), se serve una base formalizzata
8. Mappa interna dei rischi, capability e dipendenze progettuali

---

## Temi core da padroneggiare

1. Payment ecosystem: issuer, acquirer, PSP, gateway, processor, merchant
2. Card payments: EMV, contactless, wallet, tokenization
3. Open banking / A2A
4. Instant payments / SEPA Instant
5. SCA, authentication e fraud prevention
6. PCI DSS e payment security
7. Terminali unattended / embedded acceptance
8. Accounting e reconciliation
9. Rollout operations su rete retail multi-site
10. Impatto regolatorio nel gaming: tracciabilità, AML, limiti, controlli, responsabilità operative

---

## Output da produrre

Per rendere la formazione spendibile, non basta completare i corsi.  
Ogni blocco deve generare un asset pratico.

### Output 1 – Payment Ecosystem Map

Mappa degli attori coinvolti:

- player / customer
- gaming machine
- terminal/device
- PSP
- acquirer
- issuer
- platform
- accounting
- DWH
- ADM/reporting

---

### Output 2 – VLT/AWP Payment Capability Map

Capability da presidiare:

- payment initiation
- authorization
- capture
- refund / reversal
- timeout handling
- reconciliation
- fraud monitoring
- reporting
- audit trail
- incident handling
- operational support

---

### Output 3 – As-Is / To-Be Architecture

Confronto tra:

- modello attuale con accettatore di banconote
- modello futuro con pagamento digitale
- impatti su macchina, piattaforma, accounting, operations e compliance

---

### Output 4 – Risk & Dependency Register

Registro dei principali rischi:

- compliance
- PCI/security
- device certification
- firmware/hardware dependency
- PSP/acquirer dependency
- ADM/accounting reconciliation
- rollout multi-site
- customer experience
- incident handling

---

## Da approfondire dopo

Questi temi non devono bloccare l’avvio, ma vanno lasciati come backlog di approfondimento:

- PCI DSS in dettaglio
- AML e antifrode specifica gaming
- chargeback e dispute management
- refund/reversal nei casi limite
- offline scenarios
- settlement e riconciliazione contabile
- integrazione con ADM / DWH / reporting
- responsabilità contrattuali tra PSP, acquirer, vendor e concessionario
- certificazione device / firmware / host
- impatti operativi su rete retail e punti vendita
- customer journey su macchina fisica

---

## Roadmap sintetica 6 settimane

| Settimana | Focus | Output |
|---|---|---|
| W1 | Base payments | Glossario + payment ecosystem map |
| W2 | Payment technologies | Sintesi card, wallet, A2A, instant payments |
| W3 | Regulation | One-pager PSD2/PSD3/PSR/SCA applicato a VLT/AWP |
| W4 | EMV/contactless/device | Mappa acceptance su device fisico |
| W5 | Security & PCI | Risk note su PCI/security responsibilities |
| W6 | Applicazione al contesto VLT/AWP | Capability map + backlog approfondimenti |

---

## Scelta iniziale consigliata

Partire con:

1. [CFTE – Payments Online Masterclass](https://courses.cfte.education/payments-online-masterclass-free-digital-payments-course/)
2. [Coursera – The Future of Payment Technologies](https://www.coursera.org/learn/paytech)
3. [Coursera – FinTech: Foundations, Payments, and Regulations](https://www.coursera.org/learn/wharton-fintech-overview-payments-regulations)
4. [EMVCo Educational Videos](https://www.emvco.com/knowledge-hub-category/educational-videos/) / [Knowledge Hub](https://www.emvco.com/knowledge-hub/)

Questa combinazione è sufficiente per costruire una base seria senza partire subito da corsi costosi.
