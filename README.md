# 📱 StickerSmash — Esplorando Expo Framework

Questo repository contiene la mia prima applicazione sviluppata con **Expo Framework** e **React Native**. Il progetto nasce come esercitazione pratica per comprendere come funziona la gestione delle pagine e la navigazione all'interno di un'app per smartphone.

---

## 🚀 Funzionalità Implementate Finora

- [x] **Architettura Expo:** Configurazione dell'ambiente di sviluppo locale nativo ed esecuzione dell'app tramite browser (per aggirare i firewall di rete).
- [x] **Navigazione a Schede (Tab Navigation):** Creazione di una barra di menu inferiore (`(tabs)`) che permette di spostarsi fluidamente tra la schermata **Home** e la schermata **About (Informazioni)**.
- [x] **Gestione dei Percorsi Errati (404 Fallback):** Creazione della schermata speciale `+not-found.tsx`. Se si inserisce un indirizzo sbagliato o inesistente, l'app mostra una schermata di errore personalizzata ("Oops! Not Found") con un link sicuro per ritornare alla Home.

---

## 🛠️ Concetti Chiave Appresi

* **File-based Routing:** Con Expo Router, la struttura delle cartelle crea automaticamente i percorsi dell'app (es. il file `about.tsx` diventa la pagina delle informazioni).
* **Layout Annidati (Nested Layouts):** Organizzazione dello Stack principale per gestire contemporaneamente sia i menu in basso (`tabs`), sia le schermate di errore totali.
* **Risoluzione Problemi di Cache:** Uso del comando `npx expo start -c` per svuotare la cache del server e forzare Expo a leggere i nuovi spostamenti delle cartelle.

---

## 📂 Struttura Attuale del Progetto

```text
StickerSmash/
└── app/                  # Cartella principale della nostra applicazione
    ├── (tabs)/           # Gruppo della navigazione a schede in basso
    │   ├── _layout.tsx   # Gestore della barra dei menu (Home / About)
    │   ├── index.tsx     # Schermata principale (Home screen)
    │   └── about.tsx     # Schermata delle informazioni (About screen)
    ├── _layout.tsx       # Il "capo supremo" dell'app (Root Layout)
    └── +not-found.tsx    # La pagina di salvataggio se l'indirizzo è sbagliato
```

---

***PAGINA PRINCIPALE***

<img width="1526" height="990" alt="Immagine 2026-05-29 131818" src="https://github.com/user-attachments/assets/d4a9bfac-8814-480d-9ed0-a1a57aa20e5e" />

