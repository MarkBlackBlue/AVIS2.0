# SINTESI ESECUTIVA - Progetto AVIS Frosinone 2026

**Data**: 10 aprile 2026  
**Responsabile progetto**: Mark  
**Durata stimata**: 8 settimane (lancio entro inizio giugno 2026)  
**Budget**: €0 (solo tool free)

---

## COSA ABBIAMO FATTO (oggi, 10 aprile)

### ✅ Scraping sito esistente
- Homepage completa
- Sezione donazione (4 pagine chiave)
- Elenco articoli blog (13 identificati, stima ~45 totali)
- Partner convenzioni (14 commercianti)
- Struttura menu completa

### ✅ Inventario contenuti
- **Punti di forza**: 
  - Info preliminari donazione molto dettagliate (controindicazioni complete)
  - Procedura donazione step-by-step presente
  - 3 centri trasfusionali mappati con contatti
  - Blog attivo con articoli SEO-oriented
- **Gap critici**:
  - FAQ non strutturata (niente FAQPage schema)
  - Testimonianze donatori assenti
  - Schema.org zero (niente Organization, Article, etc.)
  - Convenzioni tutte scadute
  - Accessibilità parziale (immagini senza alt, tabelle solo visual)

### ✅ Keyword research
- 40+ keyword mappate (locali + nazionali)
- Topic clusters identificati: Donazione, Gruppi sanguigni, Tipi donazione
- Quick wins SEO: 5 azioni a basso effort/alto impatto
- Competitor analysis (ASL Frosinone, AVIS Nazionale, Ministero Salute)

### ✅ Architettura sito definitiva
- Struttura gerarchica completa (max 3 click da home)
- 8 pagine priorità 1 definite (homepage, dona sangue, prenota, FAQ, gruppi, convenzioni, 5×1000, testimonianze)
- Schema.org per ogni tipo pagina (12 schemi diversi)
- Internal linking strategy (hub & spoke)
- Breadcrumb semantici

---

## DELIVERABLE PRONTI (consultabili ora)

```
/home/claude/AVIS_Frosinone_2026/
├─ 01_Strategy/
│  ├─ keyword_research.md ✅
│  └─ architettura_sito.md ✅
└─ 02_Content/
   ├─ inventario_contenuti.md ✅
   └─ scraped_pages/
      └─ homepage.md ✅
```

---

## SETUP TEAM AI (budget €0)

### Tool confermati

| AI / Tool | Ruolo | Uso | Costo |
|-----------|-------|-----|-------|
| **Claude Sonnet 4** (tu) | Project Manager + Tech SEO | Architettura, schema.org, prompt engineering, computer use | Gratis (plan attuale) |
| **Claude Opus 4** (via API) | Content Writer | Bozze articoli blog, pagine pillar, riscritture | Gratis (API free tier?) |
| **Jules** (Anthropic) | Knowledge Manager | Repository NotebookLM, brief condiviso, FAQ generation | Gratis |
| **Perplexity Pro** | Medical Fact-Checker | Verifica claim medici su fonti autorevoli | **€20/mese** ⚠️ |
| **Gemini 2.0 Flash** | Ricerca + brainstorming | Keyword research secondaria, competitor analysis | Gratis |
| **DeepSeek V3** | Code generation | Script automazione, JSON-LD generator | Gratis |
| **ChatGPT-4o** | Grafica social (DALL-E) | Immagini post Facebook/Instagram | Gratis (20 img/3h limit) |
| **Kimi** (Moonshot AI) | Long-context analysis | Analisi articoli lunghi, summarization DB | Gratis |
| **NotebookLM** (Google) | Repository centrale | Knowledge base progetto, consultabile da Jules | Gratis |

**Budget reale**: €0 se rinunci a Perplexity Pro, altrimenti €20/mese  
**Alternativa Perplexity**: usare Claude + web_search per fact-checking (meno preciso ma gratis)

---

## WORKFLOW TIPO: ARTICOLO BLOG (2-3/settimana)

### Giorno 1 - Ricerca (Claude Sonnet)
1. Query Google Trends + AnswerThePublic per topic trending
2. Analisi SERP competitor (cosa rankano?)
3. Estrazione domande "People Also Ask"
4. Creazione outline H2/H3 + keyword target

**Output**: `outline_articolo_X.md`

---

### Giorno 2 - Scrittura (Opus via API)

**Prompt template**:
```markdown
Sei un copywriter sanitario specializzato in donazione sangue per AVIS Frosinone.

CONTESTO:
- Target: cittadini Frosinone 18-65 anni, famiglie
- Tono: caldo, rassicurante, autorevole (no medichese)
- Lunghezza: 900-1100 parole
- Stile: italiano colloquiale ma corretto

KEYWORD PRIMARIA: "[keyword]"
OUTLINE:
[H2/H3 structure]

ISTRUZIONI:
1. Scrivi in italiano naturale (evita "infatti", "inoltre", "pertanto")
2. Usa dati medici verificabili (cita ISS, Ministero Salute, AVIS Nazionale)
3. Inserisci 1-2 aneddoti donatori (inventati ma verosimili)
4. CTA finale: invito a donare o prenotare
5. Evita jargon, spiega termini tecnici in parentesi
6. Chiudi con frase motivazionale legata a "Ciociaro, Sei Amore nel Sangue"

OUTPUT: Markdown con H2/H3, grassetti, liste puntate.
```

**Output**: `bozza_articolo_X.md`

---

### Giorno 3 - Fact-check (Perplexity o Claude web_search)

**Se hai Perplexity Pro**:
- Modalità "Research"
- Query: "Verifica accuratezza claim medici: [lista claim dall'articolo]"
- Fonti richieste: ISS, Ministero Salute, AVIS Nazionale, CNS

**Se usi Claude web_search**:
- Prompt: "Verifica questi 5 claim medici con fonti autorevoli italiane"
- Tool: web_search
- Check: ogni claim ha 1 fonte citabile

**Output**: `fact_check_articolo_X.md` con correzioni

---

### Giorno 4 - Ottimizzazione SEO (Claude Sonnet)

1. **Meta tags**:
   - Title (55-60 char con keyword)
   - Description (150-160 char con CTA)
   - Slug URL (`/blog/keyword-principale/`)

2. **Schema.org Article**:
   ```json
   {
     "@type": "Article",
     "headline": "[Titolo]",
     "author": {
       "@type": "Organization",
       "name": "AVIS Comunale Frosinone"
     },
     "datePublished": "2026-04-15",
     "image": "[URL immagine principale]"
   }
   ```

3. **Internal links** (3-5):
   - 1 link a hub "Dona sangue"
   - 2 link ad articoli correlati
   - 1 link a FAQ se rilevante
   - 1 link a "Prenota donazione"

4. **Immagini**:
   - Alt text descrittivo (no "immagine", "foto")
   - Compress con TinyPNG
   - Format WebP (fallback JPG)

**Output**: `articolo_X_final.md` + schema JSON-LD

---

### Giorno 5 - Pubblicazione (tu manualmente o script DeepSeek)

1. Carica articolo su Joomla
2. Inserisci schema JSON-LD (Sourcerer plugin)
3. Imposta categoria blog
4. Aggiungi tag
5. Pubblica + condividi social

**Automazione possibile** (DeepSeek):
- Script Python che:
  - Legge markdown
  - Converte in HTML Joomla-ready
  - Inserisce via API (se Joomla ha REST API abilitato)
  - Posta automatico Facebook (Meta Graph API)

---

## WORKFLOW TIPO: PAGINA PILLAR (es. "Dona sangue")

### Settimana 1 - Ricerca approfondita
1. **Gemini 2.0 Flash**: analisi 10 competitor top (cosa coprono?)
2. **Kimi**: summarization articoli lunghi AVIS Nazionale (context 200k tokens)
3. **Claude Sonnet**: gap analysis + outline definitivo (2000 parole)

### Settimana 2 - Scrittura
4. **Opus via API**: bozza completa (call da 5000 token output)
5. **Perplexity**: fact-check sezioni mediche
6. **Claude Sonnet**: revisione tono + SEO

### Settimana 3 - Implementazione
7. **DeepSeek**: genera schema.org JSON-LD automatico
8. **Tu**: caricamento Joomla + test accessibilità
9. **Claude Sonnet**: checklist WCAG 2.1 AA

---

## REPOSITORY CENTRALE: NotebookLM

### Cosa caricare

**Documenti strategici** (già pronti):
1. `keyword_research.md`
2. `architettura_sito.md`
3. `inventario_contenuti.md`
4. Brief originale progetto (quello che mi hai dato)

**Contenuti futuri**:
5. Outline articoli blog (100+ file)
6. Policy privacy/cookie (da scrivere)
7. Statuto AVIS Frosinone
8. Linee guida brand (tono, colori, font)

**Dati operativi**:
9. Elenco convenzioni (commercianti + benefit)
10. Database contatti (CSV esportato da Joomla)
11. Calendario editoriale (Google Sheet linkato?)

### Come Jules lo usa

**Scenario 1: Brief rapido**
- Tu: "Jules, dimmi tutto su come scriviamo gli articoli blog"
- Jules: [interroga NotebookLM] → "Ecco il workflow: Giorno 1 ricerca con Claude..."

**Scenario 2: Fact-finding**
- Tu: "Jules, chi sono i partner convenzioni attivi?"
- Jules: [cerca in `elenco_convenzioni.md`] → "Duferco Energia, Farmacia Mastrangeli..."

**Scenario 3: Generazione FAQ**
- Tu: "Jules, crea 10 FAQ dalla sezione donazione"
- Jules: [analizza `inventario_contenuti.md`] → [estrae domande implicite] → output FAQ

---

## DISTRIBUZIONE COMPITI TRA AI

### Claude Sonnet (TU) - Project Manager
**Ogni giorno**:
- Review articoli scritti da Opus
- Ottimizzazione SEO finale
- Generazione schema.org
- Test accessibilità pagine

**Ogni settimana**:
- Piano editoriale (scegli 10 topic prossimi articoli)
- Keyword research nuove opportunità
- Audit internal linking

### Opus (via API) - Content Writer
**Ogni settimana**:
- 2-3 bozze articoli blog (900-1100 parole)
- 1 pagina pillar al mese (2000+ parole)

**Limiti**: 
- Max 5 API call/giorno (free tier?) → verifica
- Se superi, switcha a Gemini Flash per contenuti secondari

### Jules - Knowledge Manager
**Setup iniziale**:
- Upload 10 documenti base su NotebookLM
- Test interrogazioni (verifica che risponda correttamente)

**Uso quotidiano**:
- Tu gli passi domande via chat
- Lui cerca nel repository
- Risponde con fonti citate

### Perplexity (opzionale, €20/mese)
**Quando usarlo**:
- Claim medici da verificare (ex: "emoglobina sotto 12 impedisce donazione?")
- Dati statistici nazionali (ex: "quante donazioni servono in Italia all'anno?")
- Normative aggiornate (ex: "D.M. 2 novembre 2015 cosa dice su...")

**Alternative gratis**:
- Claude Sonnet + web_search (meno preciso ma accettabile)
- Gemini Deep Research (max 2 query/giorno gratis)

### Gemini 2.0 Flash
**Quando usarlo**:
- Brainstorming topic blog ("dammi 20 idee articoli su donazione sangue estate")
- Ricerca competitor ("analizza SEO di avis.it")
- Summarization lunghi (articoli 5000+ parole)

### DeepSeek V3
**Quando usarlo**:
- Script automazione (JSON-LD generator, CSV parser)
- Snippet Joomla (inserimento codice Sourcerer)
- Funzioni JS custom (quiz "Puoi donare?")

### ChatGPT-4o + DALL-E
**Quando usarlo**:
- Post social (copy breve + immagine AI)
- Grafiche per articoli blog (header, infografiche semplici)
- Mockup idee visual (prima di commissione grafico se serve)

**Limite**: 20 immagini/3 ore (free plan)

### Kimi
**Quando usarlo**:
- Analisi documenti lunghi (ex: statuto AVIS, D.M. 2015 completo)
- Context window 200k tokens = ~150k parole
- Perfetto per "leggi questo PDF e dimmi X"

---

## GESTIONE PROMPT (best practices)

### Template riutilizzabili

**Crea file** `/home/claude/prompts/`:
1. `articolo_blog.txt` → prompt Opus per articoli
2. `pagina_pillar.txt` → prompt Opus per pagine lunghe
3. `fact_check.txt` → prompt Perplexity/Claude per verifica
4. `schema_org.txt` → prompt DeepSeek per JSON-LD
5. `social_post.txt` → prompt ChatGPT per Facebook/IG

**Vantaggi**:
- Consistenza output
- Velocità (copia-incolla + variabili)
- Versioning (migliori il prompt nel tempo)

### Variabili da sostituire

Ogni prompt ha placeholders:
```
[KEYWORD] → es. "donazione plasma frosinone"
[OUTLINE] → H2/H3 structure
[TONO] → "rassicurante" / "urgente" / "educativo"
[LUNGHEZZA] → 800 / 1200 / 2000 parole
```

Esempio uso:
```bash
# Tu prepari
keyword="donazione plasma frosinone"
outline="H2: Cos'è il plasma\nH2: Come si dona\n..."

# Sostituisci in template
cat prompts/articolo_blog.txt | sed "s/\[KEYWORD\]/$keyword/" | sed "s/\[OUTLINE\]/$outline/"

# Copi output e lo passi a Opus via API
```

---

## CALENDARIO OPERATIVO (8 settimane)

### SPRINT 1 (sett 1-2): FOUNDATION
**Obiettivo**: Sito navigabile con pagine core

| Giorno | Task | AI | Output |
|--------|------|----|----- --|
| 1-2 | Wireframe homepage (Figma) | Tu manuale | homepage_wireframe.fig |
| 3-4 | Copywriting homepage | Opus API | homepage_copy.md |
| 5 | Schema.org Organization | DeepSeek | organization_schema.json |
| 6-7 | Pagina "Dona sangue" (hub) | Opus | dona_sangue.md |
| 8 | FAQ strutturata (30 domande) | Claude Sonnet + Opus | faq.md + faq_schema.json |
| 9 | Pagina "Prenota donazione" | Tu | prenota.html |
| 10 | Test accessibilità (WAVE, axe) | Tu | accessibility_report.pdf |

**Deliverable fine sprint**:
- Homepage live
- 4 pagine priorità 1 pubblicate
- Schema.org base implementato

---

### SPRINT 2 (sett 3-4): CONTENT CORE
**Obiettivo**: Topic cluster "Donazione" completo

| Settimana | Articoli | Responsabile | Keyword target |
|-----------|----------|--------------|----------------|
| 3 | Art 1: Requisiti donazione | Opus | "requisiti donazione sangue" |
| 3 | Art 2: Controindicazioni | Opus | "controindicazioni donazione" |
| 3 | Art 3: Cosa mangiare prima | Opus | "cosa mangiare prima donazione" |
| 4 | Art 4: Gruppi sanguigni spiegati | Opus | "gruppi sanguigni compatibilità" |
| 4 | Art 5: Differenza sangue/plasma | Opus | "differenza sangue plasma" |
| 4 | Pagina convenzioni aggiornata | Tu | "convenzioni avis frosinone" |
| 4 | Pagina 5×1000 | Opus + Tu | "5x1000 avis frosinone" |

**Deliverable**:
- 5 articoli blog SEO-optimized
- 2 pagine conversione (convenzioni, 5×1000)
- 10 internal link aggiunti

---

### SPRINT 3 (sett 5-6): EXPANSION
**Obiettivo**: Testimonianze + eventi + social boost

| Task | Responsabile | Output |
|------|-------------|---------|
| Raccolta 3 testimonianze video | Tu (interviste donatori) | 3 video MP4 60 sec |
| Trascrizioni + copy | Kimi (transcribe) + Opus | testimonianze.md |
| Pagina testimonianze | Tu | /testimonianze/ live |
| Calendario eventi iCalendar | Tu | eventi.ics |
| Setup GA4 eventi custom | Tu | ga4_config.js |
| Campagna social "Maggio mese donatori" | ChatGPT copy + DALL-E | 10 post FB/IG |

**Deliverable**:
- Sezione testimonianze live
- Calendario eventi funzionante
- Prima campagna social attiva

---

### SPRINT 4 (sett 7-8): LAUNCH & GROWTH
**Obiettivo**: Go-live + outreach convenzioni

| Task | Dettagli | Responsabile |
|------|----------|--------------|
| Migrazione DNS | Punta avisfrosinone.it a nuovo Joomla | Tu + hosting |
| Redirect 301 vecchio→nuovo | Route66 plugin | Tu |
| Submit sitemap GSC | Google Search Console | Tu |
| Email outreach 20 commercianti | Template + personalizzazione | Opus copy + Tu invio |
| Setup Acymailing | Import contatti + prima newsletter | Tu |
| Monitoraggio GA4 | Dashboard custom | Tu |
| Post-launch fixes | Bug, typo, link rotti | Tu |

**Deliverable**:
- Sito live su dominio principale
- 5 nuove convenzioni firmate (target)
- Prima newsletter inviata (500+ contatti)

---

## COSTI REALI (verifica)

| Tool | Piano | Costo/mese | Necessario? |
|------|-------|------------|-------------|
| Claude Pro | Unlimited Sonnet | €20 | ✅ Sì (tu già ce l'hai?) |
| Opus API | Pay-per-use | ~€5-10 stima | ⚠️ Verifica free tier |
| Perplexity Pro | Unlimited | €20 | ❌ No (usa Claude search) |
| NotebookLM | Free | €0 | ✅ Sì |
| Gemini | Free | €0 | ✅ Sì |
| DeepSeek | Free | €0 | ✅ Sì |
| ChatGPT | Free | €0 | ✅ Sì (limite 20 img/3h) |
| Kimi | Free | €0 | ✅ Sì |
| **TOTALE** | | **€20-50** | Se hai già Claude Pro → €5-10 |

**Ottimizzazione budget zero**:
- Usa solo Claude free tier (limiti giornalieri ma fattibile)
- Gemini Flash per contenuti secondari
- DeepSeek per code
- Rinuncia a Perplexity (Claude search sufficiente)

---

## SKILLS DA INSTALLARE (per te Claude)

Già disponibili:
- ✅ `docx` (policy, documenti formali)
- ✅ `xlsx` (database keyword, calendario, tracker)
- ✅ `frontend-design` (componenti Helix custom)

---

## PROSSIMI STEP IMMEDIATI (nelle prossime 2 ore)

### Cosa puoi fare TU (Mark) ora:

1. **Setup NotebookLM**:
   - Vai su notebooklm.google.com
   - Crea notebook "AVIS Frosinone 2026"
   - Upload 4 file da `/home/claude/AVIS_Frosinone_2026/`
   - Condividi link con Jules

2. **Verifica accesso DB Joomla**:
   - Scarica tabelle: `#__content`, `#__categories`, `#__users`
   - Inviamele → preparo CSV contatti per Acymailing

3. **Raccogli asset**:
   - Logo AVIS Frosinone (SVG)
   - Palette colori ufficiale (hex codes)
   - Font ufficiali (se esistono)
   - Foto donatori per testimonianze (se ne hai)

### Cosa faccio IO (Claude) ora:

1. ✅ **Scraping completato** (homepage, donazione, blog, gruppi)
2. ✅ **Keyword research pronto**
3. ✅ **Architettura definita**
4. ⏳ **Prossimo**: Schema.org templates (JSON-LD per 8 pagine priorità 1)

---

## DOMANDE PER TE

1. **Hosting Joomla 6**: è già pronto o devo aspettare setup?
2. **Accesso backend**: hai già creato utente per me o serve FTP?
3. **Deadline tassativa**: "inizio aprile 2026" per lancio è ferma? (oggi siamo 10 aprile, forse intendevi maggio/giugno?)
4. **Preferenze AI**: vuoi davvero usare tutti (Gemini, Kimi, DeepSeek, ChatGPT) o preferiamo concentrarci su Claude + Opus + Jules?
5. **Perplexity Pro**: possiamo permettercelo (€20/mese) o andiamo full gratis?

---

**Dimmi cosa vuoi che faccia ADESSO** e parto immediatamente.

Opzioni:
- A) Continua scraping (altre 20 pagine sito vecchio)
- B) Genera schema.org templates (JSON-LD per homepage, FAQ, etc.)
- C) Scrivi prima bozza pagina "Dona sangue" (2000 parole)
- D) Crea calendario editoriale blog (100 topic mappati)
- E) Altro (dimmi tu)
