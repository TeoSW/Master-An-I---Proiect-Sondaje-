# 📊 Percepția Locuitorilor Județului Buzău asupra Calității Serviciilor Publice Locale

> Proiect academic realizat în cadrul cursului **Sondaje – Teorie și Aplicații**  
> Academia de Studii Economice din București | Facultatea de Cibernetică, Statistică și Informatică Economică  
> Student: **Constantin Teodor-Vasile** | București, 2026

---

## 📌 Descriere

Acest proiect prezintă proiectarea completă a unui **plan de sondaj stratificat în două stadii** pentru măsurarea percepției cetățenilor județului Buzău față de calitatea serviciilor publice locale. Baza empirică este **Recensământul Populației și Locuințelor din 2021**, iar eșantionul final vizează **2.013 persoane** distribuite proporțional pe 5 straturi geografico-demografice.

---

## 🎯 Obiective

- Definirea riguroasă a populației de interes (persoane cu vârsta ≥ 15 ani, rezidente în județul Buzău)
- Construirea bazei de sondaj din datele oficiale ale Recensământului 2021
- Calcularea volumului de eșantion cu ajustare pentru efectul de design și non-răspuns
- Stabilirea unui plan de eșantionare stratificat, reproductibil și reprezentativ
- Estimarea costurilor și resurselor necesare pentru desfășurarea sondajului

---

## 🗂️ Structura Proiectului

```
📁 proiect-sondaje-buzau/
├── 📄 Proiect_Sondaje.docx        # Documentul principal al proiectului
├── 📊 Baza_de_Date_-_Buzau.xlsx   # Baza de date cu cele 87 UAT-uri din județul Buzău
└── 📄 README.md
```

### Fișiere principale

| Fișier | Conținut |
|---|---|
| `Proiect_Sondaje.docx` | Metodologie completă, calcule, plan de sondaj, concluzii |
| `Baza_de_Date_-_Buzau.xlsx` | Date demografice per localitate, stratificare, alocarea interviurilor |

---

## 🧮 Metodologie

### Populația țintă
Persoane cu vârsta de **minimum 15 ani**, rezidente în județul Buzău la data de 1 decembrie 2021 — **N = 404.979 persoane**.

### Metoda de culegere a datelor
**Interviu față în față**, realizat de operatori de interviu deplasați în localitățile selectate.

### Calculul volumului de eșantion

| Parametru | Valoare |
|---|---|
| Nivel de încredere | 95% (z = 1,96) |
| Dispersie (maximă) | 0,25 (p = 0,5) |
| Eroare maximă admisă | ±3 puncte procentuale |
| Volum inițial (n₀) | 1.064 persoane |
| Efect de design (efectD) | 1,34 |
| Corecție non-răspuns (efectG) | 1,20 (~17% rată de non-răspuns) |
| **Volum final (nₚ)** | **2.013 persoane** |

### Stratificarea

Cele 87 de unități administrativ-teritoriale au fost grupate în **5 straturi**:

| Strat | Descriere | Nr. UAT-uri | Localități selectate | Interviuri alocate |
|---|---|---|---|---|
| 1 | Municipiul Buzău (auto-selectat) | 1 | 1 | 514 |
| 2 | Municipiul Râmnicu Sărat (auto-selectat) | 1 | 1 | 148 |
| 3 | Localități cu 4.000–10.000 locuitori | 23 | 5 | 675 |
| 4 | Localități cu 2.000–4.000 locuitori | 39 | 7 | 548 |
| 5 | Localități cu sub 2.000 locuitori | 23 | 5 | 128 |

### Planul de eșantionare în două stadii

**Stadiul 1 – Selectarea localităților**  
Selecție aleatoare simplă fără revenire în SPSS (modulul *Complex Samples*), stratificată după variabila `strat`, cu număr constant de unități per strat.

**Stadiul 2 – Selectarea secțiilor de votare**  
Selecție sistematică din Registrul Secțiilor de Votare (AEP):
- Orașe: 2 secții de votare per localitate
- Comune: 1 secție de votare per localitate

**Selecția gospodăriei**  
Itinerar sistematic cu punct de start aleator și pas de eșantionare calculat per secție.

**Selecția respondentului**  
Metoda **celei mai recente zile de naștere** din rândul membrilor gospodăriei cu vârsta ≥ 15 ani.

---

## 📈 Date utilizate

- **Recensământul României 2021** – populație rezidentă per localitate: [recensamantromania.ro](https://www.recensamantromania.ro/rezultate-rpl-2021/rezultate-provizorii/)
- **Registrul Secțiilor de Votare** – Autoritatea Electorală Permanentă: [roaep.ro](https://www.roaep.ro/management-electoral/wp-content/uploads/2015/08/REGISTRULSECTIILORDEVOTARE.pdf)

---

## 🛠️ Instrumente utilizate

- **Microsoft Excel / XLSX** – construirea și prelucrarea bazei de date
- **SPSS** – selecția aleatoare a localităților (modulul *Complex Samples*)
- **Microsoft Word** – redactarea documentului metodologic

---

## 📐 Rezultate cheie

- Eșantion final: **2.013 respondenți** în **19 localități** din județul Buzău
- Precizie garantată: **±3 puncte procentuale** la un nivel de încredere de **95%**
- Acoperire: municipii, orașe și comune din toate zonele geografice ale județului (urban, suburban, rural, montan)

---

## 📚 Bibliografie

- Recensământ România 2021 — https://www.recensamantromania.ro
- Registrul Secțiilor de Votare, AEP — https://www.roaep.ro

---

*Proiect academic | ASE București, 2026*
