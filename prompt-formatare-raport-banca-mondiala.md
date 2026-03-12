# Prompt — Formatare unitară raport Banca Mondială (Word / .docx)

---

**Instrucțiuni pentru Claude Opus 4.6:**

Am atașat un raport redactat pentru Banca Mondială. Am nevoie să creezi un document Word (.docx) nou, curat, complet reformatat, respectând **strict** următoarele reguli:

---

## 1. REGULA DE AUR: NU MODIFICA TEXTUL

- **NU ai voie să modifici, reformulezi, adaugi, ștergi sau rearanjezi niciun cuvânt, propoziție sau paragraf din textul original.**
- Textul trebuie copiat caracter cu caracter, fără nicio intervenție editorială.
- Dacă găsești greșeli de tipar, formulări neclare sau inconsistențe — le lași exact cum sunt. Nu corectezi nimic.

---

## 2. FONT ȘI DIMENSIUNE — UNIFORMITATE PE TOT DOCUMENTUL

Aplică următorul stil pe întregul document, fără excepții:

| Element | Font | Dimensiune | Stil | Spațiere |
|---|---|---|---|---|
| **Titlul documentului** | Times New Roman | 16 pt | Bold, centrat | Spațiu după: 24 pt |
| **Titlu capitol (Heading 1)** | Times New Roman | 14 pt | Bold, numerotare arabă (1, 2, 3…) | Spațiu înainte: 18 pt, după: 12 pt |
| **Titlu secțiune (Heading 2)** | Times New Roman | 12 pt | Bold, numerotare tip 1.1, 1.2… | Spațiu înainte: 12 pt, după: 6 pt |
| **Titlu subsecțiune (Heading 3)** | Times New Roman | 12 pt | Bold italic, numerotare tip 1.1.1… | Spațiu înainte: 10 pt, după: 6 pt |
| **Text normal (body)** | Times New Roman | 12 pt | Regular, justified | Line spacing: 1.15, spațiu după: 6 pt |
| **Note de subsol** | Times New Roman | 10 pt | Regular | Line spacing: single |
| **Tabele / figuri — titlu** | Times New Roman | 10 pt | Bold, centrat deasupra | Spațiu după: 4 pt |
| **Tabele — conținut** | Times New Roman | 10 pt | Regular | — |
| **Header / Footer** | Times New Roman | 9 pt | Italic | Număr pagină centrat în footer |

---

## 3. NOTE DE SUBSOL — CU FUNCȚIA AUTOMATĂ FOOTNOTES A WORD

- **Toate notele de subsol trebuie inserate folosind funcția nativă de Footnotes din Word** (Insert → References → Footnote), NU scrise manual în text.
- Fiecare notă va avea un număr de referință automat, generat de Word, care se actualizează automat la renumerotare.
- Numerotarea notelor de subsol: continuă pe tot documentul (nu se resetează la fiecare capitol).
- Dacă în documentul original notele sunt puse manual (ex: numere scrise de mână cu text la finalul paginii), le transformi în footnotes automate Word, păstrând exact textul original al fiecărei note.

---

## 4. STRUCTURĂ DOCUMENT — FORMATUL DIN PRIMELE DOUĂ CAPITOLE

- Analizează structura primelor două capitole ale documentului original (cum sunt organizate titlurile, secțiunile, subsecțiunile, listele, paragrafele).
- Aplică **exact aceeași structură și ierarhie** pe restul documentului, de la capitolul 3 până la final.
- Concret:
  - Dacă primele două capitole folosesc numerotare de tip **1. → 1.1 → 1.1.1**, aplică același sistem peste tot.
  - Dacă primele două capitole au bullet points cu un anumit stil, păstrează acel stil pe tot documentul.
  - Dacă există un pattern de introducere la început de capitol, urmată de secțiuni tematice, menține acel pattern.
- **NU schimba ordinea conținutului. NU muta secțiuni dintr-un capitol în altul. NU reorganiza logic textul. Doar aplică formatarea.**

---

## 5. ELEMENTE SUPLIMENTARE

- **Cuprins (Table of Contents):** Generează un cuprins automat la începutul documentului, bazat pe stilurile Heading 1/2/3.
- **Page breaks:** Fiecare capitol nou (Heading 1) începe pe o pagină nouă.
- **Margini:** 2.5 cm pe toate cele 4 laturi.
- **Pagină:** A4, orientare portrait.
- **Numerotare pagini:** Arabă, centrat în footer, începând de la pagina de după cuprins.

---

## 6. OUTPUT

- Generează fișierul în format **.docx** (compatibil Microsoft Word).
- Numele fișierului: `Raport_Banca_Mondiala_formatat.docx`
- Nu include comentarii, tracked changes sau markup-uri — documentul trebuie să fie curat și final.

---

## REZUMAT FINAL

✅ Text = identic cu originalul, caracter cu caracter
✅ Font = Times New Roman peste tot, dimensiuni conform tabelului
✅ Footnotes = automate Word (nu manuale)
✅ Structură = uniformă, bazată pe modelul din primele 2 capitole
✅ Cuprins = automat
✅ Format = .docx, A4, margini 2.5 cm
