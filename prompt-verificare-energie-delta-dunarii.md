# Prompt pentru Verificarea Veridicității - Capitolul Energie din Strategia Integrată de Dezvoltare Durabilă a Deltei Dunării

## Instrucțiuni de utilizare

> **Model recomandat:** Claude Opus 4.6 Extended Thinking
> **Mod de utilizare:** Copiază promptul de mai jos și atașează documentul (PDF/DOCX) ca fișier în conversație.
> **Notă:** Pentru rezultate optime, activează "Extended Thinking" și setează un buget generos de tokens pentru gândire (maxim disponibil).

---

## PROMPT

```
Ești un expert senior în politici energetice europene, dezvoltare durabilă, legislație UE în domeniul energiei, și un fact-checker riguros. Ai cunoștințe aprofundate despre:
- Strategia energetică a UE și a României
- Directivele europene privind energia regenerabilă (RED II/RED III), eficiența energetică (EED), și tranziția energetică
- Specificul energetic al Deltei Dunării și al zonelor protejate Natura 2000 / Rezervația Biosferei
- Programele de finanțare europene (PNRR, Fondul pentru Modernizare, PODD, LIFE, Horizon Europe etc.)
- Statistici energetice naționale și europene (Eurostat, INS, ANRE, IRENA, IEA)

## CONTEXT

Documentul atașat reprezintă o contribuție la **capitolul de energie** din **Strategia Integrată de Dezvoltare Durabilă a Deltei Dunării**, elaborat cu sprijinul inteligenței artificiale. Tocmai pentru că a fost generat cu asistență AI, există riscul prezenței de **halucinații** (informații fabricate, date statistice inventate, referințe bibliografice inexistente, cifre eronate).

## SARCINI

Realizează următoarele sarcini în mod sistematic și riguros:

### SARCINA 1: Evaluare generală a veridicității

Parcurge **întregul document** și evaluează fiecare afirmație factuală, cifră, dată statistică, referință legislativă sau instituțională din perspectiva:
- **Corectitudinii factuale** - informația corespunde realității?
- **Actualității** - datele sunt actuale sau depășite?
- **Relevanței contextuale** - informațiile sunt relevante pentru Delta Dunării și contextul energetic românesc/european?
- **Coerenței interne** - există contradicții între diferite secțiuni ale documentului?

### SARCINA 2: Atenție specială la textul evidențiat cu galben (highlighted)

Identifică toate pasajele **evidențiate/highlight cu galben** din document. Pentru fiecare:
- Verifică riguros dacă informația este **veridică și verificabilă**
- Dacă este corectă → confirmă explicit cu formularea: **[VERIFICAT ✓]**
- Dacă este parțial corectă → marchează cu: **[PARȚIAL CORECT ⚠️]** și oferă corectura
- Dacă este incorectă/fabricată → marchează cu: **[INCORECT ✗ - HALUCINAȚIE]** și oferă informația corectă sau recomandă eliminarea

### SARCINA 3: Verificarea extensivă a notelor de subsol existente

Pentru **fiecare notă de subsol** din document:
1. Verifică dacă **sursa citată există în realitate** (publicație, document oficial, raport, directivă, site web)
2. Verifică dacă **titlul, autorul, anul, pagina** sunt corecte
3. Verifică dacă **conținutul citat corespunde** cu ceea ce se pretinde în text
4. Clasifică fiecare notă:
   - **[NOTĂ REALĂ ✓]** - sursa există și este corect citată
   - **[NOTĂ SUSPECTĂ ⚠️]** - sursa ar putea exista, dar detaliile nu pot fi confirmate integral; necesită verificare manuală suplimentară
   - **[NOTĂ FABRICATĂ ✗]** - sursa nu există sau este evident inventată → propune eliminarea sau înlocuirea cu o sursă reală

### SARCINA 4: Completarea referințelor lipsă și identificarea halucinațiilor

Pentru fiecare **afirmație factuală din text care NU are notă de subsol**:
1. Evaluează dacă informația este **verificabilă și corectă**
2. **Dacă DA** (informația este reală și verificabilă):
   - Creează o **notă de subsol nouă** cu o referință reală, completă, în format academic
   - Format: Autor/Instituție, *Titlu*, An, URL (dacă disponibil)
   - Marchează nota nouă cu: **[NOTĂ ADĂUGATĂ - NOU]**
3. **Dacă NU** (informația este o halucinație sau nu poate fi verificată):
   - Marchează direct în text cu: **[⚠️ HALUCINAȚIE IDENTIFICATĂ - de eliminat sau reformulat]**
   - Explică de ce informația este considerată fabricată
   - Propune o **reformulare corectă** bazată pe date reale, acolo unde este posibil

## FORMAT DE LIVRARE

### A. Document revizuit
Produce **versiunea revizuită completă** a documentului cu:
- Toate marcajele inline ([VERIFICAT ✓], [INCORECT ✗], etc.)
- Notele de subsol corectate, eliminate sau adăugate
- Halucinațiile semnalizate vizibil
- Reformulările propuse inserate ca [PROPUNERE: text alternativ]

### B. Raport de verificare (în chat)
După document, produce un **raport structurat** care include:

1. **Sumar executiv** - evaluare generală a calității și veridicității documentului (scor procentual estimat de veridicitate)
2. **Statistici:**
   - Număr total de afirmații factuale verificate
   - Număr de afirmații confirmate ca veridice
   - Număr de afirmații parțial corecte
   - Număr de halucinații identificate
   - Număr total de note de subsol verificate
   - Note reale / suspecte / fabricate
   - Note noi adăugate
3. **Lista detaliată a halucinațiilor** - cu localizare (secțiune, paragraf), natura halucinației, și corectura propusă
4. **Lista notelor de subsol fabricate** - cu propuneri de înlocuire
5. **Lista notelor de subsol adăugate** - cu justificare
6. **Recomandări generale** pentru îmbunătățirea documentului
7. **Evaluare a riscurilor** - ce secțiuni necesită cea mai urgentă revizuire umană expertă
8. **Disclaimer** - limitările acestei verificări (cunoștințe până la data de cutoff, imposibilitatea accesării unor baze de date, etc.)

## REGULI IMPORTANTE

- **NU inventa** referințe sau note de subsol. Dacă nu poți identifica o sursă reală, spune explicit acest lucru.
- **NU confirma** o informație doar pentru că "sună plauzibil". Dacă nu o poți verifica, marchează ca [NECESITĂ VERIFICARE MANUALĂ].
- **FII CONSERVATOR** în evaluări - e preferabil să semnalezi un fals pozitiv decât să lași o halucinație nedetectată.
- Folosește **cunoștințele tale până la data de cutoff** și semnalează explicit când o informație ar putea fi mai recentă decât cunoștințele tale.
- Pentru **legislația UE și românească**, verifică cu atenție numerele directivelor, regulamentelor, legilor, OUG-urilor etc.
- Pentru **date statistice** (MW instalați, procente de energie regenerabilă, etc.), verifică ordinul de mărime și consistența cu surse cunoscute.
- Acordă atenție specială **denumirilor de programe, proiecte și instituții** - sunt frecvent halucinante în textele generate AI.

## LIMBA

Documentul este în limba română. Răspunde integral în limba română, atât documentul revizuit cât și raportul.

Începe acum analiza documentului atașat.
```

---

## Note suplimentare pentru utilizator

### Cum să folosești acest prompt eficient:

1. **Pregătirea documentului:**
   - Asigură-te că highlight-urile galbene sunt vizibile în fișierul atașat (PDF-ul trebuie să păstreze marcajele)
   - Dacă folosești DOCX, highlight-urile sunt păstrate automat

2. **Configurare Claude:**
   - Folosește **Claude Opus 4.6** cu **Extended Thinking** activat
   - Setează bugetul de gândire la maximum
   - Dacă documentul este lung, poți împărți verificarea pe secțiuni

3. **Iterare:**
   - După prima verificare, poți cere clarificări suplimentare pe secțiuni specifice
   - Poți cere o a doua trecere focusată doar pe notele de subsol
   - Verificarea manuală a elementelor marcate ca [NECESITĂ VERIFICARE MANUALĂ] rămâne esențială

4. **Follow-up recomandat:**
   ```
   Concentrează-te acum exclusiv pe secțiunea [X] și verifică în profunzime
   fiecare afirmație. Pentru notele de subsol noi pe care le-ai creat,
   furnizează și URL-uri funcționale acolo unde este posibil.
   ```
