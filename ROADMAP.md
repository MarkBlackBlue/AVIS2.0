# ROADMAP - AVIS 2.0

**Durata totale**: 8 settimane  
**Inizio**: 10 aprile 2026  
**Target go-live**: 5 giugno 2026

---

## 📊 Overview Progetto

| Sprint | Periodo | Focus | Completamento |
|--------|---------|-------|---------------|
| Sprint 1 | 10-23 aprile | Foundation | 15% (giorno 1/14) |
| Sprint 2 | 24 apr - 7 mag | Content Core | 0% |
| Sprint 3 | 8-21 maggio | Expansion | 0% |
| Sprint 4 | 22 mag - 5 giu | Launch | 0% |

---

## SPRINT 1 (Settimane 1-2): FOUNDATION

**Periodo**: 10-23 aprile 2026  
**Obiettivo**: Sito navigabile con pagine core pronte

### 🎯 Deliverable

#### Settimana 1 (10-16 aprile)

**Design & Architettura**
- [ ] Wireframe homepage (Figma/sketch) - **@Mark** - 4h
  - Layout mobile-first 375px
  - Desktop breakpoint 1200px
  - Usa colori da `colors.md`
  - 6 sezioni slide come da architettura

**Schema.org Foundation**
- [ ] 8 template JSON-LD - **@Claude** - 30min
  - Organization (homepage)
  - HowTo (dona sangue)
  - FAQPage (FAQ)
  - DonateAction (5×1000)
  - LocalBusiness (convenzioni)
  - Article (blog template)
  - ContactPage (contatti)
  - MedicalWebPage (gruppi sanguigni)

**Copywriting**
- [ ] Homepage copy (2000 parole) - **@Claude-Opus** - 1h
  - Hero + 6 sezioni slide
  - SEO ottimizzato per "AVIS Frosinone"
  - CTA chiari per ogni sezione

- [ ] Pagina "Dona Sangue" hub - **@Claude-Opus** - 2h
  - 2000 parole pillar content
  - Schema HowTo integrato
  - 5+ internal link
  - TOC (table of contents)

#### Settimana 2 (17-23 aprile)

**Content Core**
- [ ] FAQ strutturata (30 domande) - **@Claude + Opus** - 3h
  - 5 categorie (Requisiti, Procedura, Frequenza, Analisi, Benefici)
  - Risposte 40-60 parole
  - Schema FAQPage JSON-LD

- [ ] Pagina "Prenota Donazione" - **@Mark** - 2h
  - Form VS-Forms (nome, email, tel, centro, data)
  - CTA rosso AVIS
  - Alternative: click-to-call, WhatsApp

**Tech Setup**
- [ ] Accesso Joomla 6 backend - **@Mark** - 15min
  - Credenziali admin
  - URL staging
  - FTP se necessario

**Quality Assurance**
- [ ] Test accessibilità WCAG 2.1 AA - **@Claude + Mark** - 2h
  - WAVE audit
  - axe DevTools
  - Lighthouse report
  - Fix critical issues

### ✅ Milestone Sprint 1

**Criterio successo**: Homepage + 4 pagine priorità 1 live su staging con schema.org implementato

**Output concreti**:
1. Homepage pubblicata (wireframe → copy → Joomla)
2. Pagina "Dona sangue" live
3. FAQ page live
4. Pagina "Prenota" live
5. Tutti con schema.org corretto
6. Accessibility report con score >90

---

## SPRINT 2 (Settimane 3-4): CONTENT CORE

**Periodo**: 24 aprile - 7 maggio 2026  
**Obiettivo**: Topic cluster "Donazione" completo + conversione pages

### 🎯 Deliverable

#### Settimana 3 (24-30 aprile)

**Blog Articles** (SEO-optimized)
- [ ] Art. 1: "Requisiti donazione sangue" - **@Opus** - 2h
  - Keyword: "requisiti donazione sangue"
  - 900 parole + checklist visiva
  - Schema Article

- [ ] Art. 2: "Controindicazioni complete" - **@Opus** - 2h
  - Keyword: "controindicazioni donazione"
  - Lista temporanee vs permanenti
  - Fact-check Perplexity

- [ ] Art. 3: "Cosa mangiare prima donazione" - **@Opus** - 1.5h
  - Keyword: "cosa mangiare prima donazione"
  - Esempi colazione/pranzo
  - Infografica suggerita

**Pagine Conversione**
- [ ] Convenzioni per donatori - **@Claude + Mark** - 3h
  - Aggiornamento 14 partner (rinnovo)
  - Schema LocalBusiness × 14
  - CTA "Diventa partner" per commercianti

#### Settimana 4 (1-7 maggio)

**Blog Articles** (continua)
- [ ] Art. 4: "Gruppi sanguigni spiegati" - **@Opus** - 2h
  - Keyword: "gruppi sanguigni compatibilità"
  - Tabella HTML accessibile
  - Schema MedicalWebPage

- [ ] Art. 5: "Differenza sangue/plasma" - **@Opus** - 1.5h
  - Keyword: "differenza sangue plasma"
  - Confronto visual
  - Link a "Tipi donazione"

**Conversione Pages**
- [ ] Pagina 5×1000 - **@Opus + Mark** - 2h
  - Schema DonateAction
  - CF 92001460606 grande e copiabile
  - Guida PDF scaricabile
  - Trasparenza uso fondi

**Tech Implementation**
- [ ] Setup GA4 - **@Mark** - 1h
  - Eventi custom: click CTA, form submit, tel/WhatsApp
  - Conversioni: prenota, 5×1000, convenzioni
  - Dashboard custom

- [ ] Internal linking audit - **@Claude** - 1h
  - Min 10 link aggiunti tra pagine
  - Hub & spoke implementation
  - Breadcrumb check

### ✅ Milestone Sprint 2

**Criterio successo**: 5 articoli blog live + 2 pagine conversione funzionanti + GA4 tracking attivo

**Output concreti**:
1. Blog con 5 articoli pubblicati
2. Convenzioni page aggiornata con partner attivi
3. 5×1000 page con form/donazioni
4. GA4 dashboard con primi dati
5. Sitemap.xml aggiornato e submitted a GSC

---

## SPRINT 3 (Settimane 5-6): EXPANSION

**Periodo**: 8-21 maggio 2026  
**Obiettivo**: Testimonianze + eventi + social boost

### 🎯 Deliverable

#### Settimana 5 (8-14 maggio)

**Testimonianze Donatori**
- [ ] Raccolta 3 video interviste - **@Mark** - 4h
  - Donatori diversi (uomo/donna, età diverse)
  - Durata: 60-90 sec ciascuno
  - Setup: smartphone + microfono esterno

- [ ] Trascrizioni + copy - **@Kimi (transcribe) + Opus** - 2h
  - Sottotitoli per accessibilità
  - Copy scritto 150-200 parole per donatore
  - Schema Person + Review

- [ ] Pagina testimonianze - **@Mark** - 2h
  - Video player embedded
  - Testo affiancato
  - CTA: "Condividi la tua storia"

**Eventi & Calendario**
- [ ] Calendario eventi (iCalendar) - **@Mark** - 2h
  - Integrazione iCalendar plugin
  - Eventi ricorrenti (raccolte mensili)
  - Schema Event per ogni raccolta

#### Settimana 6 (15-21 maggio)

**Social Media Campaign**: "Maggio mese donatori"

- [ ] Calendario editoriale (20 post) - **@Claude** - 1h
  - 10 Facebook + 10 Instagram
  - Topic: testimonianze, FAQ, urgenze, convenzioni
  - Pianificazione 1-31 maggio

- [ ] Copy post social - **@ChatGPT-4o** - 2h
  - Tono caldo, call-to-action chiare
  - Hashtag locali: #AvisFrosinone #DonaVita
  - Emoji uso moderato

- [ ] Grafiche DALL-E - **@ChatGPT-4o** - 3h
  - 5 grafiche custom (hero, donatori, gruppi, urgenze, 5×1000)
  - Palette colori AVIS
  - Watermark logo

**Email Marketing**
- [ ] Setup Acymailing - **@Mark** - 1.5h
  - Import 500 contatti da vecchio sito
  - Template newsletter brand AVIS
  - Opt-in GDPR compliant

- [ ] Prima newsletter "Benvenuti nuovo sito" - **@Opus** - 1h
  - Oggetto: "Il nuovo sito AVIS Frosinone è online!"
  - Highlight: FAQ, convenzioni, prenota
  - CTA: visita sito

### ✅ Milestone Sprint 3

**Criterio successo**: Testimonianze live + calendario funzionante + 20 post social pubblicati + prima newsletter inviata

**Output concreti**:
1. Sezione testimonianze con 3 video
2. Calendario eventi con almeno 6 raccolte mappate
3. 20 post social pubblicati e performanti
4. Database 500 contatti su Acymailing
5. Newsletter inviata con >30% open rate

---

## SPRINT 4 (Settimane 7-8): LAUNCH & GROWTH

**Periodo**: 22 maggio - 5 giugno 2026  
**Obiettivo**: Go-live + outreach convenzioni + crescita

### 🎯 Deliverable

#### Settimana 7 (22-28 maggio)

**Preparazione Go-Live**
- [ ] Migrazione DNS - **@Mark + hosting** - 1h
  - Punta avisfrosinone.it a nuovo Joomla
  - Backup completo sito vecchio
  - Verifica propagazione DNS (24-48h)

- [ ] Redirect 301 vecchio→nuovo - **@Mark** - 2h
  - Route66 plugin configurazione
  - Mappa URL vecchi → nuovi
  - Test tutti i redirect principali

- [ ] Submit sitemap GSC - **@Claude** - 15min
  - Google Search Console
  - Sitemap.xml aggiornato
  - Request indexing pagine priorità 1

**Outreach Convenzioni**
- [ ] Template email commercianti - **@Opus** - 1h
  - Oggetto: "Convenzione AVIS Frosinone: valore per i tuoi clienti"
  - Personalizzazione per settore
  - CTA: call o meeting

- [ ] Lista 20 commercianti target - **@Mark** - 2h
  - Ricerca locale Frosinone
  - Segmenti: salute, ristorazione, servizi, retail
  - Contatti (email, telefono)

- [ ] Invio email + follow-up - **@Mark** - 3h
  - Invio personalizzato a 20 target
  - Follow-up dopo 7 giorni
  - Tracking risposte

#### Settimana 8 (29 mag - 5 giu)

**Go-Live & Monitoring**
- [ ] Go-live sito - **@Team** - 4h
  - Annuncio social/email
  - Monitoring uptime prime 48h
  - Fix bug urgenti

- [ ] Firma nuove convenzioni - **@Mark** - variabile
  - Target: 5 commercianti
  - Contratti formali
  - Pubblicazione su sito

**Analytics & Optimization**
- [ ] Dashboard GA4 custom - **@Mark** - 2h
  - KPI principali visibili
  - Report settimanale automatico
  - Alerts per anomalie

- [ ] Post-launch fixes - **@Team** - 4h
  - Bug fix prioritari
  - Typo correzioni
  - Link rotti fix
  - Performance optimization

**Content Continuity**
- [ ] Piano editoriale blog (3 mesi) - **@Claude** - 2h
  - 50 topic mappati
  - Calendario giugno-agosto
  - Assegnazione responsabilità

### ✅ Milestone Sprint 4 (FINALE)

**Criterio successo**: Sito live su dominio principale + 5 nuove convenzioni firmate + traffico stabile

**Output concreti**:
1. avisfrosinone.it punta a nuovo sito ✅
2. Tutti i redirect 301 funzionanti ✅
3. Sitemap submitted e prime pagine indicizzate ✅
4. 5 nuove convenzioni attive e pubblicate ✅
5. GA4 con primi 7 giorni dati ✅
6. Piano editoriale 3 mesi pronto ✅

---

## POST-LAUNCH (Da giugno in poi): CRESCITA

### Content Machine (ongoing)

**Frequenza pubblicazione**:
- 2 articoli blog/settimana (mar + ven)
- 1 testimonianza video/mese
- 1 campagna social/mese (tematica)
- Newsletter mensile (report donazioni + news)

**Responsabilità**:
- Copy articoli: Claude Opus (bozza) → Claude Sonnet (review)
- Fact-check medico: Perplexity o Claude web_search
- Pubblicazione Joomla: Mark
- Social media: ChatGPT-4o (copy + grafiche)

### SEO Monitoring (mensile)

**KPI da tracciare**:
- Posizionamento keyword principali (GSC)
- Featured snippet ottenuti (target: 3+)
- Traffico organico vs mese precedente (target: +15%/mese)
- Click-through rate medio (target: >5%)
- Pagine indicizzate (target: 50+ entro luglio)

**Tool**:
- Google Search Console (settimanale)
- GA4 dashboard (giornaliero)
- Ahrefs/Ubersuggest free (mensile, se disponibile)

### Conversione Optimization (mensile)

**A/B Test**:
- CTA homepage ("Prenota ora" vs "Scopri se puoi donare")
- Form "Prenota donazione" (campi obbligatori vs facoltativi)
- Colori CTA (rosso AVIS vs arancione)

**Tracking**:
- Form contatti compilati (target: +20%/mese)
- Click "Prenota donazione" (target: +25%/mese)
- Telefonate ricevute (call tracking se possibile)
- WhatsApp messaggi (GA4 eventi)

### Outreach Continuo

**Convenzioni** (mensile):
- 5 nuovi commercianti contattati
- 2 convenzioni firmate (target)
- 1 rinnovo convenzione esistente

**Partnership** (trimestrale):
- Scuole Frosinone (campagne sensibilizzazione)
- Aziende locali (giornate donazione in sede)
- Eventi città (sponsorizzazioni, stand informativi)

---

## 📊 METRICHE SUCCESSO PROGETTO

### SEO (6 mesi)
- ✅ Top 3 "donazione sangue frosinone"
- ✅ Top 10 per 10+ keyword correlate
- ✅ 3+ featured snippet
- ✅ Traffico organico +150%
- ✅ Backlink +20

### Conversione (6 mesi)
- ✅ Nuovi donatori +30%/mese media
- ✅ Form contatti +200%
- ✅ Click CTA +300%
- ✅ 5×1000 donatori +50%

### Contenuti (6 mesi)
- ✅ 100+ articoli blog pubblicati
- ✅ 10+ testimonianze video
- ✅ 200+ post social
- ✅ 10+ convenzioni attive

### Business (6 mesi)
- ✅ 10 convenzioni commercianti attive
- ✅ €X raccolti tramite donazioni/5×1000
- ✅ 500+ iscritti newsletter Acymailing
- ✅ Uptime sito >99.5%

---

## 🚨 BLOCCHI / RISCHI

### Blocco Critico
**Accesso Joomla 6 non disponibile**
- **Impatto**: Alto - blocca implementazione
- **Mitigazione**: Mark setup entro settimana 1
- **Piano B**: Staging su hosting temporaneo

### Rischio Alto
**Database vecchio sito non recuperabile**
- **Impatto**: Medio - perdita contatti newsletter
- **Mitigazione**: Backup manuale tabelle Joomla
- **Piano B**: Rebuild lista da zero (form iscrizione)

### Rischio Medio
**Logo AVIS Frosinone non disponibile**
- **Impatto**: Basso - estetica compromessa
- **Mitigazione**: Uso logo AVIS Nazionale placeholder
- **Piano B**: Design logo custom temporaneo

### Rischio Basso
**Commercianti non interessati convenzioni**
- **Impatto**: Basso - feature non critica
- **Mitigazione**: Amplia raggio ricerca (paesi limitrofi)
- **Piano B**: Convenzioni nazionali (Duferco, etc.)

---

## 📞 CHECK-IN SCHEDULE

**Daily standup** (asincrono, GitHub):
- Cosa ho fatto ieri
- Cosa faccio oggi
- Blocchi/domande

**Weekly review** (ogni lunedì):
- Avanzamento vs ROADMAP
- Aggiustamenti priorità
- Decisioni architetturali

**Sprint review** (fine ogni 2 settimane):
- Demo deliverable completati
- Retrospettiva cosa è andato bene/male
- Planning sprint successivo

**Monthly stakeholder update**:
- Report a AVIS Frosinone (board)
- KPI progresso
- Budget status (se applicabile)

---

## 🎯 PROSSIMA AZIONE IMMEDIATA

**Oggi (10 aprile)**:
- [ ] Schema.org templates (Claude) - 30min
- [ ] Wireframe homepage (Mark) - 4h

**Domani (11 aprile)**:
- [ ] Copywriting homepage (Opus) - 1h
- [ ] Setup Joomla staging (Mark) - 1h

**Questa settimana**:
- [ ] Completare tutti i task Settimana 1 (vedi sopra)

---

**Ultimo aggiornamento**: 10 aprile 2026  
**Prossima review**: 17 aprile 2026 (metà Sprint 1)  
**Responsabile ROADMAP**: Jules (aggiornamenti settimanali)
