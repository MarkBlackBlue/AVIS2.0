# PROMPTS DI COPYWRITING - PAGINE PRIORITÀ 1

Questi prompt sono ottimizzati per essere inviati a diverse istanze di Claude (Sonnet o Opus) per lavorare in parallelo. Ogni prompt include contesto, keyword target, struttura richiesta e tono di voce.

---

## STRATEGIA DI PARALLELIZZAZIONE
Per massimizzare l'efficienza, puoi distribuire i task tra 4 agenti (o 4 chat diverse):

*   **AGENTE A**: Homepage + Pagina "Prenota Donazione" (Focus: Conversione)
*   **AGENTE B**: Hub "Dona Sangue" (Focus: Guida Pillar - ~1500 parole)
*   **AGENTE C**: FAQ Donazione + Gruppi Sanguigni (Focus: Informazione Tecnica/Educativa)
*   **AGENTE D**: Convenzioni + 5x1000 + Testimonianze (Focus: Community e Sostegno)

---

## PROMPT 1 (PER AGENTE A) - HOMEPAGE E PRENOTA
**Obiettivo**: Creare una Home ad alto impatto emotivo e una pagina di prenotazione chiara.

```markdown
Sei un Senior Copywriter esperto in ambito sanitario e associazionistico. Devi scrivere i testi per la nuova HOMEPAGE e la pagina PRENOTA di AVIS Frosinone.

LINEE GUIDA GENERALI:
- Target: Cittadini di Frosinone (18-65 anni).
- Tono: Caldo, rassicurante, motivazionale ("Ciociaro, Sei Amore nel Sangue").
- Lingua: Italiano colloquiale ma impeccabile.

TASK 1: HOMEPAGE
- Scrivi una Hero Section con H1 (emozionale), Sottotitolo (chiarificatore) e CTA.
- Articola 6 Slide/Sezioni:
  1. Perché donare (4 benefit chiave).
  2. Requisiti rapidi (check-list visiva).
  3. Dove donare (Ospedale Spaziani, Cassino, Sora).
  4. Convenzioni (anteprima benefit).
  5. Volontariato (invito all'azione).
  6. 5x1000 (sostegno economico).

TASK 2: PAGINA PRENOTA DONAZIONE
- H1: "Prenota la tua donazione a Frosinone".
- Testo rassicurante sulla semplicità della procedura.
- Istruzioni chiare per prenotare via Telefono, WhatsApp o Form.
- Nota sui documenti da portare (ID + Tessera Sanitaria).

KEYWORD DA INTEGRARE: "avis frosinone", "donazione sangue frosinone", "prenotare donazione sangue frosinone".

OUTPUT: Markdown con H1, H2, liste puntate e indicazioni per i bottoni (CTA).
```

---

## PROMPT 2 (PER AGENTE B) - HUB "DONA SANGUE"
**Obiettivo**: Scrivere la guida definitiva alla donazione (Pillar Page).

```markdown
Sei un Medical Copywriter specializzato in divulgazione scientifica. Devi scrivere la GUIDA PILLAR "Dona Sangue" per il sito di AVIS Frosinone.

LUNGHEZZA: Circa 1500-2000 parole.
STRUTTURA RICHIESTA:
1. Intro: L'importanza del gesto.
2. Chi può donare: Requisiti fisici e stile di vita.
3. Controindicazioni: Temporanee e permanenti (usa i dati del Ministero/AVIS).
4. Il processo: Step-by-step (dall'accettazione al ristoro).
5. Tipi di donazione: Sangue intero vs Plasma (aferesi).
6. Diritti del donatore: Il permesso lavoro retribuito.

REQUISITI:
- Usa i dati tecnici presenti nel file `inventario_contenuti.md` (es. 450ml per il sangue, frequenze di donazione).
- Tono: Autorevole ma accessibile.
- Formattazione: Usa H2 e H3 per la leggibilità.

KEYWORD TARGET: "come donare sangue", "requisiti donazione sangue", "controindicazioni donazione sangue", "donazione plasma".

OUTPUT: Articolo completo in Markdown.
```

---

## PROMPT 3 (PER AGENTE C) - FAQ E GRUPPI SANGUIGNI
**Obiettivo**: Fornire risposte rapide e informazioni sulla compatibilità.

```markdown
Sei un esperto di comunicazione sanitaria. Devi redigere la sezione FAQ e la pagina GRUPPI SANGUIGNI di AVIS Frosinone.

TASK 1: FAQ (Almeno 25 domande)
- Dividi in categorie: Requisiti, Procedura, Salute/Farmaci, Post-donazione.
- Risposte brevi (40-60 parole) e dirette.
- Esempi: "Posso donare se ho un tatuaggio?", "Cosa mangio prima?", "Posso donare con il ciclo?".

TASK 2: GRUPPI SANGUIGNI
- Spiegazione del sistema AB0 e fattore Rh.
- Focus sul Donatore Universale (0-) e Ricevente Universale (AB+).
- Crea una tabella di compatibilità testuale descrittiva (accessibile).

TONO: Pratico, veloce, informativo.

KEYWORD: "gruppi sanguigni compatibilità", "0 negativo donatore universale", "faq donazione sangue".

OUTPUT: Markdown strutturato.
```

---

## PROMPT 4 (PER AGENTE D) - CONVENZIONI, 5X1000 E TESTIMONIANZE
**Obiettivo**: Rafforzare il senso di comunità e trasparenza.

```markdown
Sei un Community Manager e Copywriter. Devi scrivere le pagine "sociali" di AVIS Frosinone.

TASK 1: CONVENZIONI PER DONATORI
- Presenta i partner attuali (Duferco, Farmacia Mastrangeli, Otovision, etc.).
- Enfatizza il valore del "Premio al Donatore".
- Scrivi una CTA per i commercianti che vogliono convenzionarsi.

TASK 2: SOSTIENICI (5x1000)
- Spiega come inserire il Codice Fiscale 92001460606.
- Trasparenza: Spiega come vengono usati i fondi (scuole, promozione, attrezzature).

TASK 3: TESTIMONIANZE (Template)
- Scrivi 3 brevi storie di donatori (ispirate a profili reali: il giovane alla prima donazione, il donatore veterano, la donna che dona plasma).
- Usa citazioni potenti.

TONO: Emozionale, trasparente, comunitario.

OUTPUT: Markdown per le 3 sezioni.
```
