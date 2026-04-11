# ARCHITETTURA SITO - AVIS Frosinone 2026

**Principi guida**:
1. Massimo 3 click da homepage a qualsiasi contenuto
2. Ogni pagina ha 1 obiettivo primario (donatori, volontari, commercianti, 5×1000)
3. Schema.org completo per ogni tipo di pagina
4. Internal linking semantico (topic clusters)
5. Breadcrumb sempre visibili
6. Mobile-first (80% traffico da smartphone stimato)

---

## STRUTTURA GERARCHICA

```
Home (Organization schema)
│
├─ DONA SANGUE (hub principale - HowTo schema)
│  ├─ Perché donare (Article)
│  ├─ Chi può donare (Article + FAQ schema)
│  │  ├─ Requisiti base
│  │  ├─ Controindicazioni temporanee
│  │  └─ Controindicazioni permanenti
│  ├─ Come donare (HowTo schema)
│  │  ├─ Cosa fare prima
│  │  ├─ Durante la donazione
│  │  └─ Dopo la donazione
│  ├─ Dove donare a Frosinone (LocalBusiness schema × 3)
│  │  ├─ Ospedale Spaziani
│  │  ├─ AO Cassino
│  │  └─ AO Sora
│  ├─ Prenota ora ⭐ CTA (Action schema)
│  ├─ Tipi di donazione (CollectionPage)
│  │  ├─ Sangue intero
│  │  ├─ Plasma (aferesi)
│  │  ├─ Piastrine
│  │  └─ Donazioni multiple
│  ├─ Gruppi sanguigni (MedicalWebPage schema)
│  │  ├─ Compatibilità (tabella interattiva)
│  │  ├─ Donatore universale (0-)
│  │  └─ Ricevente universale (AB+)
│  └─ FAQ Donazione ⭐ (FAQPage schema)
│
├─ CHI SIAMO (AboutPage schema)
│  ├─ AVIS Comunale Frosinone (Organization details)
│  ├─ Storia AVIS (Article)
│  ├─ Statuto (WebPage)
│  ├─ Organigramma (WebPage)
│  ├─ La nostra sede (Place schema)
│  └─ Recapiti (ContactPage schema)
│
├─ CONVENZIONI ⭐ (CollectionPage)
│  ├─ Per donatori (OfferCatalog schema)
│  │  └─ [Lista commercianti con benefit]
│  └─ Diventa partner (WebPage + CTA)
│     └─ Form adesione convenzione
│
├─ BLOG / NEWS (Blog schema)
│  ├─ [Articoli con Article schema + breadcrumb]
│  └─ Categorie:
│     ├─ Salute e donazione
│     ├─ Eventi AVIS Frosinone
│     ├─ Storie di donatori
│     ├─ News mondo AVIS
│     └─ Guide pratiche
│
├─ TESTIMONIANZE ⭐ NUOVO (CollectionPage)
│  └─ [Video + testo con Person + Review schema]
│
├─ 5×1000 / DONAZIONI ⭐ (DonateAction schema)
│  ├─ Come destinare il 5×1000
│  ├─ Donazione libera (form PayPal/bonifico)
│  └─ Rendicontazione trasparente
│
├─ VOLONTARIATO ⭐ (JobPosting schema?)
│  ├─ Diventa volontario AVIS
│  ├─ Cosa facciamo
│  └─ Candidatura (form)
│
├─ EVENTI (CollectionPage)
│  ├─ Calendario donazioni ⭐ (iCalendar + Event schema)
│  ├─ Raccolte straordinarie
│  └─ Iniziative sociali
│
└─ CONTATTI (ContactPage schema)
   ├─ Form contatto (vs-forms)
   ├─ WhatsApp (+39 377 4901081)
   ├─ Email (info@avisfrosinone.it)
   ├─ Telefono
   └─ Mappa Google (embedded)
```

---

## PAGINE PRIORITÀ 1 (lancio sito)

### 1. HOMEPAGE ⭐⭐⭐

**Obiettivo**: Convertire visitatori in donatori o lead  
**Schema.org**: Organization + MedicalOrganization  
**CTA principali** (sopra fold):
1. "Prenota donazione" (button primario)
2. "Controlla se puoi donare" (quiz interattivo 3 domande)
3. "WhatsApp" (floating button)

**Struttura slide** (modello esistente ottimizzato):

**Hero section**:
- H1: "Ciociaro, Sei Amore nel Sangue!"
- Sottotitolo: "Ti bastano 15 minuti per salvare 3 vite"
- Video background: donatore felice post-donazione (15 sec loop)
- CTA: "Prenota ora" + "Scopri come donare"

**Slide 1: Perché donare** (background immagine cuore stilizzato)
- H2: "Perché donare il sangue?"
- 4 card benefit (icone custom):
  - Salute sotto controllo (analisi gratuite)
  - Autosufficienza locale (scorte Frosinone)
  - Salva 3 vite per donazione
  - Permesso lavoro retribuito
- Link: "Tutti i benefici →"

**Slide 2: Requisiti** (background chiaro, checklist visiva)
- H2: "Puoi donare se hai:"
- 3 requisiti visuali grandi:
  - 18-60 anni (icona torta compleanno)
  - Min 50kg (icona bilancia)
  - Stile vita sano (icona cuore sport)
- CTA: "Controlla tutti i requisiti →"

**Slide 3: Dove donare** (mappa Frosinone con pin)
- H2: "3 centri trasfusionali a Frosinone"
- Mini-card per ogni centro:
  - Ospedale Spaziani (principale)
  - AO Cassino
  - AO Sora
- CTA: "Prenota in 2 click →"

**Slide 4: Convenzioni** (immagini loghi partner)
- H2: "14 convenzioni attive per i nostri donatori"
- Carosello loghi (autoplay)
- CTA: "Scopri gli sconti →"

**Slide 5: Volontariato** (foto gruppo volontari)
- H2: "Unisciti alla nostra squadra"
- Testo breve: "Cerchiamo giovani motivati..."
- CTA: "Diventa volontario →"

**Slide 6: 5×1000** (visual codice fiscale)
- H2: "Sostienici con il 5×1000"
- CF: 92001460606 (grande, copyable)
- CTA: "Come fare →"

**Footer completo** (presente in tutte le pagine):
- Colonna 1: Info AVIS (indirizzo, CF, contatti)
- Colonna 2: Link rapidi (dona, convenzioni, blog, FAQ)
- Colonna 3: Link istituzionali (AVIS Nazionale, Ministero, CNS)
- Colonna 4: Social (Facebook, Instagram, YouTube)
- Copyright + Privacy/Cookie/Termini

**Schema JSON-LD**:
```json
{
  "@context": "https://schema.org",
  "@type": ["Organization", "MedicalOrganization"],
  "name": "AVIS Comunale Frosinone",
  "url": "https://avisfrosinone.it",
  "logo": "https://avisfrosinone.it/images/logo-avis-frosinone.svg",
  "image": "https://avisfrosinone.it/images/og-home.jpg",
  "description": "Associazione volontariato donazione sangue a Frosinone. Dona sangue, salva vite. Controlli gratuiti e convenzioni per donatori.",
  "telephone": "+39-377-4901081",
  "email": "info@avisfrosinone.it",
  "address": {
    "@type": "PostalAddress",
    "streetAddress": "Via Mazzini, 70",
    "addressLocality": "Frosinone",
    "postalCode": "03100",
    "addressCountry": "IT"
  },
  "parentOrganization": {
    "@type": "Organization",
    "name": "AVIS Nazionale",
    "url": "https://avis.it"
  },
  "areaServed": {
    "@type": "City",
    "name": "Frosinone"
  },
  "sameAs": [
    "https://facebook.com/avisfrosinone",
    "https://instagram.com/avisfrosinone"
  ],
  "contactPoint": {
    "@type": "ContactPoint",
    "telephone": "+39-377-4901081",
    "contactType": "customer service",
    "availableLanguage": "Italian"
  }
}
```

---

### 2. DONA SANGUE - HUB ⭐⭐⭐

**URL**: `/dona-sangue/`  
**H1**: "Come donare sangue a Frosinone: la guida completa"  
**Schema**: HowTo  

**Contenuto** (1500 parole):
- Intro: perché questa guida (problema → soluzione)
- TOC (table of contents linkabile)
- Sezione 1: Chi può donare (requisiti con checklist)
- Sezione 2: Come funziona (step-by-step con numeri)
- Sezione 3: Dove donare (3 centri con mappa)
- Sezione 4: Cosa portare (documenti)
- Sezione 5: Cosa aspettarsi (tempistiche reali)
- CTA finale: "Prenota la tua donazione"

**Internal links** (minimo 8):
- → Requisiti completi
- → Controindicazioni
- → Cosa mangiare prima
- → Durante la donazione
- → Dopo la donazione
- → Gruppi sanguigni
- → FAQ
- → Testimonianze

**Breadcrumb**: Home > Dona sangue

---

### 3. PRENOTA DONAZIONE ⭐⭐⭐

**URL**: `/prenota-donazione/`  
**H1**: "Prenota la tua donazione di sangue a Frosinone"  
**Schema**: Action  

**Contenuto**:
- Step 1: Scegli il centro trasfusionale (radio button)
  - Ospedale Spaziani (consigliato - tutti i giorni)
  - AO Cassino (ven/sab)
  - AO Sora (lun-ven)
- Step 2: Contattaci per prenotare
  - Option A: Telefono (0775 8822370 Spaziani) - click-to-call
  - Option B: WhatsApp (+39 377 4901081) - link diretto
  - Option C: Form (nome, email, tel, centro preferito, data preferita)
- Conferma: "Ti ricontatteremo entro 24h"

**Note visibili**:
- "Porta documento + tessera sanitaria"
- "Tempo totale: 30-60 minuti"
- "Giornata lavorativa retribuita"

**CTA alternative**: "Ho domande" → link FAQ

---

### 4. FAQ DONAZIONE ⭐⭐⭐

**URL**: `/faq-donazione-sangue/`  
**H1**: "Domande frequenti sulla donazione di sangue"  
**Schema**: FAQPage  

**Categorie** (accordion):

**A. Requisiti e idoneità** (10 domande)
1. Chi può donare il sangue?
2. C'è un'età massima per donare?
3. Qual è il peso minimo richiesto?
4. Posso donare se ho tatuaggi?
5. Posso donare durante il ciclo mestruale?
6. Posso donare in gravidanza?
7. Posso donare se prendo farmaci?
8. Posso donare dopo il vaccino COVID?
9. Posso donare se ho fatto sport?
10. Quanto deve essere la pressione?

**B. Procedura donazione** (8 domande)
1. Come si prenota una donazione?
2. Quanto dura la donazione?
3. Cosa devo portare?
4. Cosa mangio prima di donare?
5. Quanto sangue viene prelevato?
6. Fa male donare sangue?
7. Cosa succede dopo la donazione?
8. Posso guidare dopo?

**C. Frequenza e tipi** (6 domande)
1. Ogni quanto posso donare?
2. Quante volte all'anno?
3. Differenza tra sangue e plasma?
4. Cos'è l'aferesi?
5. Posso scegliere cosa donare?
6. Meglio sangue o plasma?

**D. Analisi e salute** (5 domande)
1. Quali analisi mi fanno?
2. Quando ricevo i risultati?
3. Cosa succede se risulto positivo?
4. Ricevo il gruppo sanguigno?
5. La donazione fa dimagrire?

**E. Benefici donatori** (4 domande)
1. Ho diritto al permesso lavoro?
2. Quali convenzioni offrite?
3. Le analisi sono gratis?
4. Posso donare il 5×1000?

**Formato risposta**:
- Risposta breve (40-60 parole)
- Link approfondimento se necessario
- Schema Question/Answer per ogni FAQ

**Esempio schema**:
```json
{
  "@type": "Question",
  "name": "Ogni quanto posso donare il sangue?",
  "acceptedAnswer": {
    "@type": "Answer",
    "text": "Tra due donazioni di sangue intero devono passare almeno 90 giorni (3 mesi). Per il plasma, l'intervallo è di 30 giorni. Gli uomini possono donare fino a 4 volte l'anno, le donne in età fertile fino a 2 volte (4 se in menopausa)."
  }
}
```

---

### 5. GRUPPI SANGUIGNI ⭐⭐

**URL**: `/gruppi-sanguigni/`  
**H1**: "Gruppi sanguigni: compatibilità e donazione"  
**Schema**: MedicalWebPage  

**Contenuto**:
- Intro: sistema AB0 e fattore Rh (200 parole divulgative)
- Tabella compatibilità (HTML accessibile + visual)
- Sezione per ogni gruppo (8 box):
  - 0 Rh- (donatore universale - box evidenziato)
  - 0 Rh+
  - A Rh-
  - A Rh+
  - B Rh-
  - B Rh+
  - AB Rh- (ricevente universale - box evidenziato)
  - AB Rh+
- FAQ inline (5 domande):
  - Qual è il gruppo più raro?
  - Perché 0- è importante?
  - Posso cambiare gruppo sanguigno?
  - Come scopro il mio gruppo?
  - Gruppo sanguigno e personalità?
- CTA: "Scopri il tuo gruppo donando sangue"

**Tabella HTML** (accessibile):
```html
<table role="table" aria-label="Compatibilità gruppi sanguigni">
  <caption>Chi può donare a chi - Gruppi sanguigni</caption>
  <thead>
    <tr>
      <th scope="col">Il mio gruppo</th>
      <th scope="col">Posso donare a</th>
      <th scope="col">Posso ricevere da</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th scope="row">0 Rh-</th>
      <td>Tutti</td>
      <td>Solo 0 Rh-</td>
    </tr>
    <!-- ... -->
  </tbody>
</table>
```

---

### 6. CONVENZIONI ⭐⭐⭐

**URL**: `/convenzioni-donatori/`  
**H1**: "Convenzioni e sconti per donatori AVIS Frosinone"  
**Schema**: OfferCatalog  

**Intro**: "Essere donatore AVIS Frosinone ti dà accesso a 14 convenzioni con attività commerciali della città. Basta mostrare la tessera associativa."

**Lista commercianti** (card per ognuno):

**Energia e servizi**:
1. **Duferco Energia** - Sconto 15% bollette luce/gas
   - Indirizzo: Online
   - Tel: XXX
   - Come attivarla: Codice promo AVIS2026

**Salute e benessere**:
2. **Farmacia Mastrangeli** - 10% su integratori e cosmesi
3. **Otovision** - 20% su occhiali e lenti
4. **Beautyfull Medical Spa** - Sconto trattamenti estetici
5. **Still Point Dr. Cristini** - Prima visita osteopatica gratis

**Ristorazione**:
6. **Real Caffè** - Caffè omaggio donatori

**Servizi professionali**:
7. **Geom. Carlo Pavia** - Consulenza catastale gratuita
8. **Finelli srl** - Sconto 10% materiali edili

**Sport e tempo libero**:
9. **Folgore** - Abbonamento palestra scontato
10. **Fotomania Fotografi** - 15% servizi fotografici

**Altro**:
11. **BP Cassinate** (banca)
12. **Geslan** (assistenza anziani)
13. **Peronti** (?)

**CTA commercianti**: 
"Vuoi convenzionarti con AVIS? Offri uno sconto ai nostri donatori e ti promuoviamo sul sito, social e newsletter."  
→ Link: `/convenzioni/diventa-partner/`

**Schema per ogni commerciante**:
```json
{
  "@type": "LocalBusiness",
  "name": "Duferco Energia",
  "image": "logo-duferco.png",
  "description": "Fornitore energia elettrica e gas - Sconto 15% per donatori AVIS",
  "offers": {
    "@type": "Offer",
    "description": "Sconto 15% su bollette luce e gas",
    "eligibleCustomerType": "Donatori AVIS Frosinone"
  }
}
```

---

### 7. 5×1000 / DONAZIONI ⭐⭐

**URL**: `/5x1000/`  
**H1**: "Sostieni AVIS Frosinone con il 5×1000"  
**Schema**: DonateAction  

**Contenuto**:

**Sezione 1: Cos'è il 5×1000**
- Spiegazione semplice (non costa nulla, scelta in dichiarazione redditi)
- Quanto vale per noi (trasparenza: "Nel 2025 abbiamo ricevuto €X da Y donatori")

**Sezione 2: Come destinarlo**
- Step visuali (infografica):
  1. Compila dichiarazione redditi (730, Unico, CU)
  2. Trova riquadro "Sostegno volontariato"
  3. Firma
  4. Inserisci CF: **92001460606** (box copiabile grande)
- Download PDF guida illustrata

**Sezione 3: Cosa facciamo con le donazioni**
- Lista trasparente (con percentuali):
  - 40% Campagne sensibilizzazione scuole
  - 30% Organizzazione raccolte sangue
  - 20% Formazione volontari
  - 10% Spese gestione

**Sezione 4: Donazione libera** (opzionale)
- Form donazione PayPal/Stripe
- Bonifico bancario (IBAN visibile)
- CTA: "Dona ora"

**Schema**:
```json
{
  "@type": "DonateAction",
  "recipient": {
    "@type": "Organization",
    "name": "AVIS Comunale Frosinone",
    "taxID": "92001460606"
  },
  "description": "Destina il tuo 5×1000 ad AVIS Frosinone per sostenere la donazione di sangue"
}
```

---

### 8. TESTIMONIANZE ⭐ NUOVO

**URL**: `/testimonianze-donatori/`  
**H1**: "Le storie dei nostri donatori"  
**Schema**: CollectionPage (con Person + Review)  

**Contenuto**: 6-10 testimonianze (video + testo)

**Formato singola testimonianza**:
- Video 60-90 sec (donatore che racconta)
- Nome, età, anni come donatore
- Citazione pull-quote grande
- Testo breve (150-200 parole)
- Foto ritratto donatore

**Esempio**:
> **Marco, 34 anni, donatore da 8 anni**  
> "Ho iniziato a donare per caso, un collega mi ha portato. Ora non riesco più a smettere: sapere che quel gesto di 15 minuti può salvare una vita mi riempie il cuore. E le analisi gratuite mi tengono la salute sotto controllo!"

**CTA finale**: "Vuoi condividere la tua storia? Scrivici"

**Schema per ogni testimonianza**:
```json
{
  "@type": "Person",
  "name": "Marco R.",
  "jobTitle": "Donatore AVIS dal 2018",
  "review": {
    "@type": "Review",
    "reviewRating": {
      "@type": "Rating",
      "ratingValue": "5"
    },
    "reviewBody": "Ho iniziato a donare per caso..."
  }
}
```

---

## SCHEMA.ORG - RIEPILOGO PER TIPO PAGINA

| Tipo pagina | Schema principale | Schema secondari |
|-------------|-------------------|------------------|
| Homepage | Organization, MedicalOrganization | - |
| Dona sangue (hub) | HowTo | WebPage |
| FAQ | FAQPage | Question/Answer (×30) |
| Gruppi sanguigni | MedicalWebPage | - |
| Convenzioni | OfferCatalog | LocalBusiness (×14) |
| Singola convenzione | LocalBusiness | Offer |
| 5×1000 | DonateAction | Organization |
| Testimonianze | CollectionPage | Person, Review |
| Articolo blog | Article, NewsArticle | Person (author) |
| Eventi | CollectionPage | Event (×N) |
| Contatti | ContactPage | Organization |
| Volontariato | WebPage | (JobPosting?) |

---

## INTERNAL LINKING STRATEGY

### Hub & Spoke Model

**Hub 1: DONA SANGUE** → spoke:
- Requisiti
- Come donare
- Dove donare
- Tipi donazione
- FAQ
- Gruppi sanguigni

**Hub 2: CHI SIAMO** → spoke:
- Storia
- Statuto
- Organigramma
- Sede

**Hub 3: PER DONATORI** → spoke:
- Convenzioni
- 5×1000
- Testimonianze

**Hub 4: BLOG** → spoke:
- Categoria 1-5
- Articoli singoli

### Link da footer (sitewide)

**Link priorità 1** (ogni pagina):
- Dona sangue
- Prenota donazione
- FAQ
- Convenzioni
- Contatti

**Link priorità 2**:
- Chi siamo
- Blog
- 5×1000
- Eventi

### Breadcrumb markup

Ogni pagina ha breadcrumb con schema BreadcrumbList:
```json
{
  "@type": "BreadcrumbList",
  "itemListElement": [{
    "@type": "ListItem",
    "position": 1,
    "name": "Home",
    "item": "https://avisfrosinone.it"
  },{
    "@type": "ListItem",
    "position": 2,
    "name": "Dona sangue",
    "item": "https://avisfrosinone.it/dona-sangue"
  },{
    "@type": "ListItem",
    "position": 3,
    "name": "Requisiti",
    "item": "https://avisfrosinone.it/dona-sangue/requisiti"
  }]
}
```

---

## SITEMAP.XML PRIORITÀ

```xml
<url>
  <loc>https://avisfrosinone.it/</loc>
  <priority>1.0</priority>
  <changefreq>weekly</changefreq>
</url>
<url>
  <loc>https://avisfrosinone.it/dona-sangue/</loc>
  <priority>0.9</priority>
  <changefreq>monthly</changefreq>
</url>
<url>
  <loc>https://avisfrosinone.it/prenota-donazione/</loc>
  <priority>0.9</priority>
  <changefreq>monthly</changefreq>
</url>
<url>
  <loc>https://avisfrosinone.it/faq/</loc>
  <priority>0.8</priority>
  <changefreq>monthly</changefreq>
</url>
<!-- Blog: priority 0.6, changefreq weekly -->
```

---

## PROSSIMI STEP

1. ✅ Architettura definita
2. ⏳ Wireframe homepage (Figma/sketch)
3. ⏳ Copywriting pagine priorità 1 (8 pagine)
4. ⏳ Implementazione schema.org (JSON-LD generator)
5. ⏳ Setup Google Search Console + submit sitemap
6. ⏳ Test accessibilità WCAG 2.1 AA
