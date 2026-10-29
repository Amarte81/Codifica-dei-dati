# Lezione Interattiva sulla Codifica dei Dati Multimediali (TPSIT — 3° Anno ITIS)

Materiale didattico interattivo completo sulla **Codifica dei Dati e delle Informazioni Multimediali** pensato per gli studenti del **3° anno di TPSIT (Tecnologie e Progettazione di Sistemi Informatici e di Telecomunicazioni)** degli Istituti Tecnici Industriali.

🌐 **Sito Live (GitHub Pages):** [https://amarte81.github.io/Codifica-dei-dati-Multimediali/](https://amarte81.github.io/Codifica-dei-dati-Multimediali/)

Progettato con doppia ergonomia:
- 🖥️ **PC / LIM (Formato 16:9):** navigazione **a Slide interattive** affiancate su due colonne, scorciatoie da tastiera (`←` / `→` / `Esc`) e barra di avanzamento.
- 📱 **Smartphone (Formato 9:16, schermo ~6 pollici):** modalità **Scroll Continuo verticale** automatico di tutte le schede e dei laboratori, pulsanti touch-friendly, canvas responsivi e indice rapido scorrevole (testabile anche da PC tramite il pulsante **📱 Vista 9:16 Scroll**).

---

## 📚 Struttura del Materiale Didattico

Il progetto è articolato in **due parti principali** collegate tra loro argomento per argomento, più un **Generatore e Risolutore Interattivo di Esercizi**:

### 🎞️ Parte 1: Slide di Spiegazione con Laboratori Interattivi (12 Slide / Schede)
Ogni slide contiene spiegazioni sintetiche, **simulazioni interattive dal vivo**, **collegamento diretto al capitolo corrispondente della Spiegazione Dettagliata (Parte 2)** e **link a video didattici esterni di approfondimento**:

1. **Fondamenti della Codifica & Testi (ASCII / Unicode / UTF-8):** dato vs informazione, regola $M \le 2^n \iff n = \lceil \log_2 M \rceil$, codifica dei caratteri con **Traduttore Live Testo → ASCII / Hex / Binario / UTF-8**.
2. **Segnali Analogici vs Digitali:** grandezze continue vs discrete, catena **ADC / DAC**, immunità al rumore e **Simulatore Interattivo di Disturbo e Rigenerazione Digitale**.
3. **Campionamento e Quantizzazione (Teoria ADC & PCM):** frequenza di campionamento $f_c = 1/T_c$, **Teorema di Shannon-Nyquist ($f_c \ge 2 f_{\max}$)**, **Aliasing**, livelli di quantizzazione $L = 2^n$, errore di quantizzazione e codifica **PCM**.
4. **Laboratorio Interattivo — Campionamento e Quantizzazione sull'Immagine del Prof. Cristaldi Marco Rosario:**
   - Modifica in tempo reale della **risoluzione di campionamento spaziale** (da $320\times320$ fino a $8\times8$ pixel con griglia visibile) e della **quantizzazione cromatica** (da $24\text{ bit TrueColor}$ fino a $1\text{ bit B/N}$, scala di grigi e tavolozze ridotte) su un ritratto del **Prof. Marco Rosario Cristaldi** (con possibilità di caricare anche qualsiasi altra foto).
   - **Lente Ispeziona-Pixel** che mostra coordinate $(x,y)$, valori RGB, codice `#HEX`, **codifica binaria del pixel** e peso in memoria.
5. **Codifica delle Immagini: Raster, Vettoriali e il Mix nei Videogiochi:**
   - Immagini **Raster (Bitmap)** (RGB, RGBA, CMYK, DPI/PPI) vs **Immagini Vettoriali** (primitive matematiche, curve di Bézier, SVG).
   - **Come funzionano le immagini nei Videogiochi (Mix Vettoriale + Raster):** mesh poligonali 3D vettoriali (wireframe di triangoli) + **Texture Mapping** raster + **Rasterizzazione GPU**, **Anti-Aliasing** e **HUD/UI ibrido** con simulatore interattivo a livelli e zoom comparato $1\times\text{–}8\times$.
6. **Codifica dei Suoni (Audio Digitale):** frequenza (suoni bassi/gravi vs acuti/alti, $20\text{ Hz}\text{–}20\text{ kHz}$), ampiezza, standard di campionamento ($8\text{ kHz}$, $44{,}1\text{ kHz}$, $48\text{ kHz}$, $96\text{ kHz}$), profondità in bit ($8$, $16$, $24\text{ bit}$), canali (Mono, Stereo, Surround) e bitrate.
7. **Laboratorio Interattivo — Campionamento e Quantizzazione di un Breve Suono (Basse + Acute):**
   - Oscilloscopio interattivo che mostra l'**onda sonora "analogica"** (composta da una componente **bassa/grave** e una **acuta/alta**) confrontata con l'**onda campionata e quantizzata a gradini** e l'errore di quantizzazione.
   - **Sintetizzatore Web Audio API reale:** permette di **ascoltare** la differenza tra il suono originale e quello ricampionato/quantizzato, udendo la perdita delle componenti acute/aliasing quando si abbassa $f_c$ e il fruscio/distorsione *bitcrush* quando si riducono i bit!
8. **Codifica dei Video & Confronto Frame Rate (FPS):**
   - Persistenza della visione, risoluzione spaziale (720p, 1080p, 4K), scansione e **Frame Rate (FPS)**.
   - **Arena Interattiva Multi-FPS:** mette a confronto in tempo reale lo stesso movimento a **6 FPS, 15 FPS, 30 FPS e 60 FPS** (più slider personalizzabile $1\text{–}60\text{ FPS}$) mostrando la differenza di fluidità e l'impatto sul peso del flusso video ($\text{MB/s}$).
9. **Calcolo delle Dimensioni di Immagini, Suoni e Video:** formulario completo (bit, Byte, multipli decimali SI $1000$ vs binari IEC $1024$) e **Calcolatore Multimediale Live 3-in-1**.
10. **Generatore di Esercizi su Immagini, Suoni e Video:** estrazione casuale di problemi graduati con verifica immediata, **svolgimento commentato passo-passo** e **Risolutore Libero** per esercizi personalizzati.
11. **Compressione dei File Multimediali (Lossless vs Lossy):** rapporto di compressione, **RLE (Run-Length Encoding)**, **Huffman/LZ77**, compressione psico-visiva/acustica (`JPEG`, `MP3`) e compressione temporale video (**I-Frame, P-Frame, B-Frame** in `H.264`/`H.265`) con **Simulatore RLE e Lossy**.
12. **Riepilogo Generale TPSIT & Autovalutazione.**

---

### 📖 Parte 2: Spiegazione Dettagliata Completa (10 Capitoli Teorico-Pratici)
Un manuale approfondito con ricerca istantanea, menu a tendina per argomento, teoria completa, schemi, formule dimostrate, **approfondimenti espandibili** e **3 esempi svolti per ogni capitolo a difficoltà crescente (🟢 Base → 🟡 Intermedio → 🔴 Avanzato)**.

---

## 🚀 Utilizzo Locale

Apri direttamente il file [`index.html`](./index.html) in qualsiasi browser web moderno su PC o smartphone (nessuna installazione o dipendenza esterna richiesta).
