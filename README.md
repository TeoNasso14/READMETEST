# 📌 Installazione e Configurazione Plugin & Modifiche al Tema

## 1. Modifiche alle Pagine e ai Componenti Esistenti
### 📝 Pagina **Formazione - Panoramica**
- Rimuovere "- Panoramica" da:
  - Titolo
  - Breadcrumbs
  - Slug

### ✉️ Modifica **Scrivimi mail** (accessibile dalla Homepage)
- Aggiungere la classe `d-none` all'elemento originale.

### 📝 Modifica del Margine in **Privacy Policy, Media Policy e Note Legali**
1. Seleziona il contenuto della pagina e fai clic su **Modifica il layout**.
2. Vai su **Modifica > Layout**.
3. Modifica il margine superiore impostandolo a `-2rem`.
4. Salva le modifiche.

---
## 2. 🔧 Modifiche al Footer
1. Vai su **Aspetto > Editor del Tema**.
2. Apri il file `footer.php`.
3. Sostituisci l'intero contenuto con il file `footer.php` presente in `utils/templates`.
4. Salva le modifiche.

---
## 3. 🏗️ Modifiche al Menu
### Contenuto
1. Vai su **Aspetto > Editor del Tema**.
2. Apri il file `menu.php`.
3. Sostituisci l'intero contenuto con il file `menu.php` presente in `utils/templates`.
4. Salva le modifiche.
### Elementi
1. Vai su **Aspetto > Menu**.
2. Aggiungi o modifica gli elementi del menu secondo le tue necessità.
  -> Accessibilità per (link personalizzato) con al suo interno
      -> Pubbliche Amministrazioni
      -> Soggetti privati
      -> Cittadini
      -> Designer e developers
  -> Formazione
  -> Risorse 
  -> PNRR (tipo sidebar)
3. Salva le modifiche.

---
## 4. 🔍 Modifiche al Search Form
1. Vai su **Aspetto > Editor del Tema**.
2. Apri il file `searchform.php`.
3. Alla riga 4, aggiungi `type="submit"` al tag del pulsante.
4. Salva le modifiche.

---
## 5. 📦 Installazione del Plugin "AgidUtility"
### ✅ Verifica **Max Upload Size**
Prima di procedere con l'installazione, assicurati che il valore di `max upload size` sia adeguato. Puoi verificarlo in:
- **Strumenti > Salute del Sito**
- Oppure eseguendo `phpinfo()`

### 📥 Installazione
1. Vai su **Plugin > Aggiungi Nuovo**.
2. Clicca su **Carica Plugin**.
3. Trascina il file `AgidUtility.zip`.
4. Clicca su **Installa Ora**, poi **Attiva**.

---
## 6. 🛠️ Installazione e Configurazione di ACF Plugin
1. Vai su **Plugin > Aggiungi Nuovo**.
2. Cerca **"Advanced Custom Fields Pro"**.
3. Installa e attiva il plugin.
4. Importa i campi personalizzati necessari da `assets`.

---
## 7. 📄 Creazione della Pagina "Domande Frequenti"
1. Vai su **Pagine > Aggiungi Nuova**.
2. Imposta il titolo **"Domande Frequenti"**.
3. Inserisci il seguente shortcode nel contenuto della pagina:
   ```md
   [filter_categories]
   ```
4. Seleziona come **template** la versione senza sidebar.
5. Imposta lo **slug** a `domande-frequenti`.
6. Salva e pubblica la pagina.

---
## 8. 🏗️ Configurazione della Sidebar
- Importare i seguenti elementi:
  - **PNRR**
  - **Guida alla Piattaforma**
- [TODO] Correggere eventuali link presenti nella sidebar.

---
## 9. 🖼️ Importazione Immagini per "Guida alla Piattaforma"
1. Vai su **Media > Aggiungi Nuovo**.
2. Carica le immagini necessarie per la pagina "Guida alla Piattaforma".

---
## 10. 🌐 Importazione e Caricamento della Favicon
1. Vai su **Aspetto > Personalizza > Denominazione del Sito**.
2. Carica la favicon nel formato consigliato (`.ico`, `.png`, `.svg`).
3. Salva le modifiche.

---
## 🔔 Note Finali
- 🔄 **Esegui un backup** del sito prima di apportare modifiche ai file del tema.
- ✅ Dopo ogni modifica, verifica il **corretto funzionamento del sito**.
- 🛠️ Per eventuali problemi, controlla la **console degli errori del browser** o i **log di WordPress**.

---

**🎯 Fine della procedura.** ✅

