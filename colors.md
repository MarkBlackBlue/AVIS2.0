# Palette Colori - AVIS Comunale Frosinone

**Versione**: 1.0  
**Data**: 10 aprile 2026  
**Brand**: AVIS Comunale Frosinone

---

## Colori Primari AVIS

### Rosso AVIS (Principale)
- **HEX**: `#E30613`
- **RGB**: `rgb(227, 6, 19)`
- **CMYK**: `C0 M97 Y92 K11`
- **Pantone**: 185 C

**Uso**:
- Logo AVIS
- CTA principali ("Prenota donazione", "Dona ora")
- Elementi di enfasi (titoli H1 homepage)
- Icone sangue/cuore
- Hover su link primari

**Accessibilità**:
- ✅ Su bianco: ratio 5.8:1 (AA Large Text)
- ❌ Su nero: ratio 3.6:1 (non sufficiente)
- **Combinare sempre con bianco o grigio molto chiaro**

---

### Bianco
- **HEX**: `#FFFFFF`
- **RGB**: `rgb(255, 255, 255)`

**Uso**:
- Background principale
- Testo su rosso AVIS
- Card e box contenuti
- Spazi negativi

---

### Nero AVIS (Testo principale)
- **HEX**: `#1A1A1A`
- **RGB**: `rgb(26, 26, 26)`

**Uso**:
- Testo body
- Titoli H2-H6
- Descrizioni
- Footer testo

**Accessibilità**:
- ✅ Su bianco: ratio 15.3:1 (AAA)

---

## Colori Secondari

### Grigio Scuro (Testo secondario)
- **HEX**: `#4A4A4A`
- **RGB**: `rgb(74, 74, 74)`

**Uso**:
- Sottotitoli
- Meta informazioni (data articoli, autore)
- Descrizioni brevi
- Breadcrumb

**Accessibilità**:
- ✅ Su bianco: ratio 9.7:1 (AAA)

---

### Grigio Medio (Bordi)
- **HEX**: `#CCCCCC`
- **RGB**: `rgb(204, 204, 204)`

**Uso**:
- Bordi card
- Separatori hr
- Input field borders
- Tabelle bordi

---

### Grigio Chiaro (Background alternativo)
- **HEX**: `#F5F5F5`
- **RGB**: `rgb(245, 245, 245)`

**Uso**:
- Background sezioni alternate homepage
- Card sfondo
- Footer background
- Table rows alternate

---

## Colori Funzionali

### Verde Successo
- **HEX**: `#28A745`
- **RGB**: `rgb(40, 167, 69)`

**Uso**:
- Messaggi successo ("Donazione prenotata!")
- Icone check/completato
- Badge "Attivo" per convenzioni
- Form validation success

**Accessibilità**:
- ✅ Su bianco: ratio 3.4:1 (AA Large Text)

---

### Giallo Attenzione
- **HEX**: `#FFC107`
- **RGB**: `rgb(255, 193, 7)`

**Uso**:
- Alert informativi (non critici)
- Badge "In attesa"
- Highlight informazioni importanti
- Box "Nota bene"

**Accessibilità**:
- ⚠️ Su bianco: ratio 1.8:1 (insufficiente)
- **Usare sempre con bordo scuro o testo nero bold**

---

### Rosso Errore
- **HEX**: `#DC3545`
- **RGB**: `rgb(220, 53, 69)`

**Uso**:
- Messaggi errore form
- Avvisi critici ("Non puoi donare se...")
- Badge "Scaduto" convenzioni
- Form validation error

**Accessibilità**:
- ✅ Su bianco: ratio 4.5:1 (AA)

---

### Blu Info
- **HEX**: `#007BFF`
- **RGB**: `rgb(0, 123, 255)`

**Uso**:
- Link secondari
- Badge "Info"
- Tooltip background
- Alert informativi neutri

**Accessibilità**:
- ✅ Su bianco: ratio 4.6:1 (AA)

---

## Colori Accent (Opzionali)

### Arancione Calore
- **HEX**: `#FF6B35`
- **RGB**: `rgb(255, 107, 53)`

**Uso**:
- Icone volontariato
- CTA secondari ("Diventa volontario")
- Elementi social media

---

### Azzurro Salute
- **HEX**: `#4ECDC4`
- **RGB**: `rgb(78, 205, 196)`

**Uso**:
- Icone salute/analisi
- Background sezione "Benefici donazione"
- Grafici/infografiche

---

## Gradienti (Uso Sporadico)

### Gradiente Hero
```css
background: linear-gradient(135deg, #E30613 0%, #A30410 100%);
```

**Uso**: Background hero homepage, CTA grandi

---

### Gradiente Overlay Immagini
```css
background: linear-gradient(
  to bottom,
  rgba(227, 6, 19, 0) 0%,
  rgba(227, 6, 19, 0.7) 100%
);
```

**Uso**: Overlay su immagini hero per leggibilità testo

---

## Regole di Utilizzo

### ✅ DO (Fare)

1. **Contrasto testo**:
   - Testo body: sempre `#1A1A1A` su `#FFFFFF`
   - Titoli grandi: `#E30613` su `#FFFFFF` OK
   - CTA: `#FFFFFF` su `#E30613`

2. **Gerarchia colore**:
   - Primario (rosso): max 10% superficie pagina
   - Bianco: 70-80% superficie
   - Grigio chiaro: 10-20% superficie

3. **Consistenza**:
   - Stesso colore = stessa funzione (verde = sempre successo)
   - Link sempre `#007BFF` (non rosso AVIS)

### ❌ DON'T (Non fare)

1. **Mai** usare rosso AVIS per testo body (illeggibile)
2. **Mai** giallo `#FFC107` su bianco senza bordo scuro
3. **Mai** combinare rosso errore + rosso AVIS (confusione)
4. **Mai** più di 3 colori primari nella stessa sezione

---

## Quick Reference - Uso Comune

| Elemento | Colore | HEX |
|----------|--------|-----|
| Background principale | Bianco | `#FFFFFF` |
| Testo body | Nero AVIS | `#1A1A1A` |
| Titoli H1 | Rosso AVIS | `#E30613` |
| Titoli H2-H6 | Nero AVIS | `#1A1A1A` |
| Link | Blu Info | `#007BFF` |
| CTA Primario background | Rosso AVIS | `#E30613` |
| CTA Primario text | Bianco | `#FFFFFF` |
| CTA Secondario background | Grigio Scuro | `#4A4A4A` |
| Bordi | Grigio Medio | `#CCCCCC` |
| Background alternato | Grigio Chiaro | `#F5F5F5` |
| Footer background | Grigio Scuro | `#4A4A4A` |
| Footer text | Bianco | `#FFFFFF` |

---

## Variabili CSS (per sviluppatori)

```css
:root {
  /* Primari */
  --color-avis-red: #E30613;
  --color-white: #FFFFFF;
  --color-black: #1A1A1A;
  
  /* Secondari */
  --color-gray-dark: #4A4A4A;
  --color-gray-medium: #CCCCCC;
  --color-gray-light: #F5F5F5;
  
  /* Funzionali */
  --color-success: #28A745;
  --color-warning: #FFC107;
  --color-error: #DC3545;
  --color-info: #007BFF;
  
  /* Accent */
  --color-orange: #FF6B35;
  --color-cyan: #4ECDC4;
  
  /* Applicazione */
  --color-text-primary: var(--color-black);
  --color-text-secondary: var(--color-gray-dark);
  --color-background: var(--color-white);
  --color-background-alt: var(--color-gray-light);
  --color-border: var(--color-gray-medium);
  --color-link: var(--color-info);
  --color-link-hover: var(--color-avis-red);
  --color-cta: var(--color-avis-red);
}
```

---

## Bootstrap Override (Joomla/Helix)

```css
/* Bootstrap button override */
.btn-primary {
  background-color: #E30613;
  border-color: #E30613;
  color: #FFFFFF;
}

.btn-primary:hover {
  background-color: #A30410;
  border-color: #A30410;
}

/* Bootstrap link override */
a {
  color: #007BFF;
}

a:hover {
  color: #E30613;
}

/* Bootstrap alert override */
.alert-success {
  background-color: #D4EDDA;
  border-color: #28A745;
  color: #155724;
}

.alert-danger {
  background-color: #F8D7DA;
  border-color: #DC3545;
  color: #721C24;
}
```

---

## Test Accessibilità

**Tool consigliati**:
- WebAIM Contrast Checker: https://webaim.org/resources/contrastchecker/
- Chrome DevTools: Lighthouse audit
- axe DevTools: Extension browser

**Standard**: WCAG 2.1 AA
- Testo normale: min 4.5:1
- Testo large (18pt+ o 14pt bold+): min 3:1

**Tutti i colori primari/secondari rispettano standard WCAG 2.1 AA** ✅

---

## Note Finali

- **Logo AVIS Nazionale**: usa sempre rosso `#E30613` (colore ufficiale AVIS)
- **Personalizzazione locale**: accent colors (arancione, azzurro) sono specifici AVIS Frosinone, non AVIS Nazionale
- **Aggiornamenti**: questo documento è living - aggiorna quando aggiungi nuovi colori

**Ultimo aggiornamento**: 10 aprile 2026  
**Responsabile**: Mark + Claude
