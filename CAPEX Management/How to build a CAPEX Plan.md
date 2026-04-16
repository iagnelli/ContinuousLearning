**il piano Capex non parte dai soldi. Parte dal parco target.**
Prima decidono **quante VLT vogliono**, **di che tipo**, **in quali anni**, **con quale mix premium/classico**, e solo dopo traducono quel disegno in euro.

---

# 1) Lezione formativa: come si costruisce un piano Capex come questo

## A. Il Capex non è un budget “sparato”

Un piano Capex serio si costruisce così:

1. **definisco lo scenario target**
2. **quantifico i volumi**
3. **distinguo nuovo vs retrofit vs refurbished**
4. **associo costi unitari**
5. **spalmo gli investimenti sugli anni**
6. **aggiungo extra Capex e Opex**
7. **porto tutto in sintesi manageriale**

Ed è esattamente quello che qui hanno fatto.

---

## B. Il vero motore del piano: il disegno del parco

Dagli screenshot Excel si vede che il modello nasce da queste domande:

* quante VLT totali ci saranno per anno?
* quante saranno premium?
* quante NEXT?
* quanti cabinet nuovi servono?
* quanti cabinet vecchi posso recuperare / retrofit?
* come cambia il mix per piattaforma e per cabinet?

Quindi la logica è:

**parco target → composizione del parco → investimenti necessari**

Non il contrario.

---

## C. Primo concetto chiave: EOP

Nell’Excel compare **VLT NEXT eop**.

**EOP = End of Period**, cioè consistenza a fine anno.

Esempio:

* 2027: **2.070**
* 2028–2031: **1.582**

Poi nel 2028 aggiungono **5% contingency**, che porta **1.582 → 1.660**.

Questa è una logica classica di piano:

* il target “pulito” è 1.582
* ma per IMAC / sostituzioni / buffer operativo tengono 5% in più
* quindi il numero “gestito/da considerare” diventa **1.660**

### Cosa imparare

Quando leggi un Capex plan, chiediti sempre:

* il volume è un target netto o include buffer?
* la contingency è una prudenza tecnica o un vero fabbisogno?

---

## D. Secondo concetto: premium mix

La prima slide PPT deriva da qui.

Nel file si vede:

* VLT avg totale per anno
* cabinet premium per anno
* incidenza premium %

Per esempio:

* 2024: 1.290 premium su 15.586 → circa **8%**
* 2025: 1.800 su 15.778 → **11%**
* 2026: 3.027 su 15.750 → **19%**
* 2027: 3.587 su 15.740 → **23%**
* 2028: 3.919 su 12.880 → **30%-31%**
* 2031: 5.479 su 12.880 → **43%**

Quindi il messaggio del business è:

**il parco totale scende, ma il peso del premium cresce.**

### Cosa imparare

Questa è una classica logica di **portfolio transformation**:

* meno asset totali
* più qualità/marginalità per asset
* più investimenti selettivi
* saving ops attesi

---

## E. Terzo concetto: premium non vuol dire una sola cosa

Nel piano premium ci sono almeno tre famiglie NEXT:

* **Optimus**
* **Vantage**
* **Curvo**

Nel riepilogo:

* Optimus: **600**
* Vantage: fino a **860**
* Curvo: fino a **200**

Quindi il premium mix non è uniforme: stanno disegnando un’evoluzione del parco con una diversa composizione per tipologia di cabinet.

### Cosa imparare

In un piano Capex non devi guardare solo “quanti asset”, ma:

* di che tipo
* a quale costo unitario
* con quale ruolo nel modello target

---

## F. Quarto concetto: nuovo acquisto vs retrofit vs refurbished

Qui c’è una parte molto istruttiva.

Nel file Excel distinguono:

### 1. **New cabinet**

Nuovi cabinet premium/target.

### 2. **Old cabinet / old cabinet G930**

Cabinet già esistenti, ancora sfruttabili o trasformabili.

### 3. **Swap old vs new**

Sostituzione progressiva del vecchio.

### 4. **Kit retrofit**

Costo per aggiornare macchine esistenti:

* board G930
* printer
* NFC payment
* altri componenti
* workforce

### 5. **Cabinet refurbished cumulative**

Vecchi cabinet recuperati / tenuti in uso / progressivamente azzerati:

* Storm
* Slantop
* Artemis

Questa è la vera intelligenza del piano:
**non comprano tutto nuovo**. Mischiano:

* nuovo
* retrofit
* recupero hardware
* phase-out del vecchio

### Cosa imparare

Questo è un concetto da imparare molto bene:
**Capex efficiency = non solo comprare, ma decidere cosa riusare, adattare o sostituire.**

---

# 2) Come calcolano i costi

## A. Costi unitari cabinet

Nel file si vedono chiaramente:

### Costo cabinet

* **Curvo = €5.500**
* **Vantage = €4.500**
* **Old Cabinet = €0**

### Costo kit

* **Curvo = €1.847**
* **Vantage = €1.847**
* **Old Cabinet = €1.847**

Quindi il costo “cabinet + kit” per il nuovo è circa:

* **Curvo = 5.500 + 1.847 = 7.347**
* **Vantage = 4.500 + 1.847 = 6.347**

Il vecchio cabinet non ha costo di cabinet, ma ha comunque costo di kit se va adattato.

---

## B. Kit retrofit - investimenti

Dal foglio vediamo costi unitari come:

* **Board G930 = €832**
* **Printer = €365**
* **Pagamento NFC = €120**
* **Others = €200**
* **Workforce retrofit = €230**
* **Workforce NFC + recupero HW = €100**

Questi costi vengono poi moltiplicati per le quantità annue.

Esempio visibile:

* NFC:

  * 1.200 x 120 = **144.000**
  * 1.450 x 120 = **174.000**
  * 1.590 x 120 = **190.800**
  * 1.660 x 120 = **199.200**

Questa è una prova chiara della logica:
**costo unitario × numero di macchine coinvolte = investimento annuo**

### Cosa imparare

Quando vedi un Capex plan, cerca sempre:

* driver volumetrico
* costo unitario
* moltiplicazione annua
* eventuale cumulato

---

## C. Totale investimenti annui

Nel foglio “Kit Retrofit - investimenti €” si vede:

### Totale investimenti principali

* **2028: 2.338.170 €**
* **2029: 2.070.750 €**
* **2030: 1.331.820 €**
* **2031: 958.300 €**

Poi aggiungono:

### Others Capex

Cash Desk:

* **128.800**
* **64.400**
* **64.400**
* **0**

Quindi:

### Totale Capex

* **2028: 3.185.140 €**
* **2029: 2.980.900 €**
* **2030: 2.048.040 €**
* **2031: 1.551.600 €**

che in slide diventa arrotondato:

* **3,2**
* **3,0**
* **2,0**
* **1,6**

### Cosa imparare

Le slide executive quasi sempre:

* semplificano
* arrotondano
* comprimono
* non mostrano il dettaglio tecnico del calcolo

L’Excel è il modello; la slide è il messaggio.

---

# 3) Come leggere l’Opex in questo piano

Nel foglio vediamo:

### Opex

* **Licenze IT per server centrale (private cloud) = 100.000 €**
* Wallet = vuoto
* Cross Ticketing = vuoto

Quindi al momento il piano:

* ha messo un Opex certo per licenze/server
* **non ha ancora valorizzato wallet e cross ticketing**

Questo si riflette nella slide, dove infatti c’è:

* **0,1 mln** nel primo anno
* poi **0,0**
* e negli highlights: **XXk€ IT per Cross Ticketing; wallet; capacity NEXT…**

### Cosa imparare

Quando in un business case vedi “XXk” o celle vuote, significa:
**la voce è riconosciuta, ma non ancora stimata.**

Questa è una lezione molto importante:
un piano economico non è sempre completo; a volte è un **placeholder strutturato**.

---

# 4) Cosa è confluito sulle slide dall’Excel

Adesso te lo mappo in modo chiaro.

## Slide PPT 1 — Incremento incidenza cabinet premium

Questa deriva direttamente dal foglio Excel con:

### Dati confluiti

* **VLT avg**
* **Cabinet premium**
* **Inc % premium**
* breakdown premium per piattaforma:

  * Novomatic
  * Cristaltec
  * IGT
  * WMG
  * Next

### Come è stato trasformato

Excel:

* usa numeri assoluti tipo 15.586, 1.290, 3.027, 5.479

Slide:

* li converte in milioni/decimali tipo:

  * 15,6
  * 1,3
  * 3,0
  * 5,5

### Inoltre confluiscono

Le righe percentuali per piattaforma diventano la tabella in basso della slide:

* Novo
* Cristaltec
* IGT
* WMG
* Next

### Highlights slide derivano da Excel + assunzioni

* incremento costante premium
* rinnovo Storm e Slantop con Vantage
* cabinet curvo
* riduzione costi ops
* aumento investimenti NEXT
* avg IMAC annuale #500 VLT

Alcune di queste cose non sono un puro calcolo, ma una **lettura manageriale** del modello.

---

## Slide PPT 2 — Investimenti Capex rinnovo parco macchine NEXT

Questa viene da due aree Excel fuse insieme:

### Blocco 1 — volumi target

Dal foglio “Deep dive Next” / riepilogo:

* VLT NEXT eop
* contingency 5%
* VLT Next tot
* VLT Premium cum
* Curvo
* Vantage
* Optimus
* Cabinet refurbished cum
* Storm / Slantop / Artemis

### Blocco 2 — costi

Dal foglio “Kit Retrofit - investimenti €”:

* costi cabinet
* costi kit
* cash desk
* IT
* Opex licenze server

### Come è stato trasformato in slide

Excel:

* contiene numeri puntuali in euro e molte componenti

Slide:

* li sintetizza in:

  * **Capex € mln**
  * **Opex € mln**
  * highlights lato business

---

# 5) Cosa NON è confluito completamente sulle slide

Molte cose dell’Excel restano fuori.

## Restano fuori o molto compresse:

* costi unitari di dettaglio (G930, printer, NFC, workforce)
* logica puntuale del retrofit
* “swap old vs new”
* costi dettagliati per anno dei componenti
* distinzione precisa tra nuovo cabinet e riuso old cabinet
* tutte le ipotesi operative dietro il recupero HW
* le celle vuote / ancora da stimare per wallet e cross ticketing

### Lezione importante

Le slide mostrano il **risultato aggregato**, non il **motore del modello**.

---

# 6) Cosa ti deve insegnare questo piano Capex, sul serio

## Lezione 1

**Il business case nasce da assunzioni.**
Se le assunzioni cambiano, il piano cambia.

Qui le assunzioni chiave sono:

* rinnovo concessione
* riduzione parco VLT
* introduzione NFC
* rinnovo NEXT dalla data concessione
* introduzione cabinet curvo
* EOL di alcune componenti

---

## Lezione 2

**Capex non significa solo acquisto di nuovo.**
Significa anche:

* retrofit
* recovery
* refurbishment
* workforce
* kit
* extra operations hardware

---

## Lezione 3

**Un buon piano distingue Capex e Opex.**
Qui lo fanno abbastanza bene:

* Capex = cabinet, kit, cash desk, IT setup
* Opex = licenze server, wallet/cross ticketing futuri

---

## Lezione 4

**L’IT spesso arriva come placeholder.**
Nel tuo caso è fondamentale: il modello è abbastanza avanzato su hardware/cabinet, ma **ancora immaturo sulle voci IT**.

Questa è una lezione molto forte anche per il tuo ruolo:
l’IT deve evitare di farsi “riempire a posteriori” come numero generico.

---

## Lezione 5

**Le slide semplificano.**
Per questo non devi mai fermarti alla slide se vuoi capire davvero.

---

# 7) Come trasformare questo in crescita professionale

Questa analisi ti può insegnare a leggere 5 cose:

### 1. Capacity planning

Come un target numerico di parco trascina l’infrastruttura.

### 2. Asset strategy

Come si decide cosa tenere, cosa adattare, cosa sostituire.

### 3. Cost model

Come si passa da quantità → costo unitario → totale annuo → sintesi executive.

### 4. Governance

Come distinguere:

* costi certi
* costi stimati
* costi mancanti
* assunzioni non validate

### 5. Posizionamento LinkedIn

Che il tema “digital payments” è in realtà:

* platform evolution
* cost model
* hardware modernization
* operational change

---

# 8) La frase più formativa che ti lascerei

Se dovessi sintetizzare questa lezione in una sola frase:

**Un piano Capex maturo non dice solo quanto spenderai: ti racconta quale futuro operativo stai cercando di costruire, con quali asset, con quali ipotesi e con quali compromessi.**

---

# 9) Cosa farei adesso al tuo posto

Io farei tre cose:

### A. Studiare il lessico del piano

* EOP
* contingency
* premium mix
* retrofit
* refurbished
* swap old vs new
* Capex vs Opex

### B. Evidenziare le assunzioni deboli

* wallet
* cross ticketing
* capacity NEXT
* nuovo tasso di guasto con NFC
* saving ops

### C. Estrarre 4 insight LinkedIn-safe

Per esempio:

* payments are never just a payment feature
* cost models start from asset choices
* innovation becomes real when operations can sustain it
* estimates are only credible when assumptions are explicit

Se vuoi, nel prossimo messaggio ti preparo la **fase 2 della lezione**:
una spiegazione ancora più pratica, voce per voce, di **come leggere ogni riga del tuo Excel come farebbe un PM senior / governance lead**.
