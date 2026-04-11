# TEMPLATE SCHEMA.ORG - PAGINE PRIORITÀ 1 (AVIS Frosinone)

Questi template JSON-LD sono pronti per essere inseriti nelle rispettive pagine tramite il plugin Sourcerer su Joomla.

---

## 1. HOMEPAGE
**Tipo**: `Organization` + `MedicalOrganization`

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
  ]
}
```

---

## 2. DONA SANGUE (HUB)
**Tipo**: `HowTo` (Spiegazione del processo)

```json
{
  "@context": "https://schema.org",
  "@type": "HowTo",
  "name": "Come donare il sangue a Frosinone",
  "description": "Guida passo dopo passo per diventare donatore AVIS a Frosinone.",
  "totalTime": "PT60M",
  "step": [
    {
      "@type": "HowToStep",
      "name": "Prenotazione",
      "text": "Prenota la tua donazione online o via WhatsApp per evitare attese."
    },
    {
      "@type": "HowToStep",
      "name": "Accettazione e Anamnesi",
      "text": "Compila il questionario informativo e colloquio con il medico."
    },
    {
      "@type": "HowToStep",
      "name": "Donazione",
      "text": "Prelievo di sangue o plasma in totale sicurezza (circa 10-20 minuti)."
    },
    {
      "@type": "HowToStep",
      "name": "Ristoro",
      "text": "Dopo la donazione, goditi un ristoro gratuito offerto da AVIS."
    }
  ]
}
```

---

## 3. PRENOTA DONAZIONE
**Tipo**: `Action` (ReserveAction)

```json
{
  "@context": "https://schema.org",
  "@type": "ReserveAction",
  "target": {
    "@type": "EntryPoint",
    "urlTemplate": "https://avisfrosinone.it/prenota-donazione/",
    "actionPlatform": [
      "http://schema.org/DesktopWebPlatform",
      "http://schema.org/MobileWebPlatform"
    ]
  },
  "agent": {
    "@type": "Organization",
    "name": "AVIS Comunale Frosinone"
  },
  "actionStatus": "http://schema.org/PotentialActionStatus",
  "result": {
    "@type": "Reservation",
    "name": "Prenotazione Donazione Sangue"
  }
}
```

---

## 4. FAQ DONAZIONE
**Tipo**: `FAQPage`

```json
{
  "@context": "https://schema.org",
  "@type": "FAQPage",
  "mainEntity": [
    {
      "@type": "Question",
      "name": "Chi può donare il sangue?",
      "acceptedAnswer": {
        "@type": "Answer",
        "text": "Possono donare tutte le persone tra i 18 e i 60 anni (fino a 65 per donatori abituali), con un peso superiore a 50kg e in buono stato di salute."
      }
    },
    {
      "@type": "Question",
      "name": "Quanto tempo deve passare tra due donazioni?",
      "acceptedAnswer": {
        "@type": "Answer",
        "text": "Per il sangue intero devono passare almeno 90 giorni. Per il plasma l'intervallo è di 30 giorni."
      }
    }
  ]
}
```

---

## 5. GRUPPI SANGUIGNI
**Tipo**: `MedicalWebPage`

```json
{
  "@context": "https://schema.org",
  "@type": "MedicalWebPage",
  "name": "Compatibilità Gruppi Sanguigni",
  "lastReviewed": "2026-04-10",
  "aspect": ["compatibilità", "caratteristiche", "emergenze"],
  "medicalAudience": "Patient"
}
```

---

## 6. CONVENZIONI
**Tipo**: `OfferCatalog`

```json
{
  "@context": "https://schema.org",
  "@type": "OfferCatalog",
  "name": "Convenzioni per Donatori AVIS Frosinone",
  "itemListElement": [
    {
      "@type": "Offer",
      "itemOffered": {
        "@type": "Service",
        "name": "Sconto 15% Bollette Luce e Gas - Duferco Energia"
      }
    },
    {
      "@type": "Offer",
      "itemOffered": {
        "@type": "Service",
        "name": "Sconto 10% Farmacia Mastrangeli"
      }
    }
  ]
}
```

---

## 7. 5x1000
**Tipo**: `DonateAction`

```json
{
  "@context": "https://schema.org",
  "@type": "DonateAction",
  "recipient": {
    "@type": "Organization",
    "name": "AVIS Comunale Frosinone",
    "taxID": "92001460606"
  },
  "description": "Sostieni AVIS Frosinone destinando il tuo 5x1000. Inserisci il Codice Fiscale 92001460606 nella tua dichiarazione dei redditi."
}
```

---

## 8. TESTIMONIANZE
**Tipo**: `CollectionPage` con `Review`

```json
{
  "@context": "https://schema.org",
  "@type": "CollectionPage",
  "name": "Storie di Donatori - AVIS Frosinone",
  "mainEntity": [
    {
      "@type": "Review",
      "itemReviewed": {
        "@type": "Organization",
        "name": "AVIS Comunale Frosinone"
      },
      "reviewBody": "Donare sangue è un gesto semplice che mi fa sentire utile per la comunità. A Frosinone il personale è fantastico.",
      "author": {
        "@type": "Person",
        "name": "Marco R."
      }
    }
  ]
}
```
