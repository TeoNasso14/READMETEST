# 📌 Installazione e Configurazione Plugin & Modifiche al Tema

## 🔧 0. Prerequisiti
1. Assicurati che il valore di `max upload size` sia adeguato. Puoi verificarlo in:
   - **🛠️ Strumenti > Salute del Sito**
   - Oppure eseguendo `phpinfo()`
   - 10mb comunque verificare la versione della cartella prima di procedere
2. Assicurarsi che le versioni di plugin e wordpress siano allineate con quelle in collaudo

## 🏗️ 1. Modifiche alle Pagine e ai Componenti Esistenti
### 📝 Pagina **Formazione - Panoramica**
- Rimuovere "- Panoramica" da:
  - 🏷️ Titolo
  - 🔗 Breadcrumbs
  - 🆔 Slug

### ✉️ Modifica **Scrivimi mail** (accessibile dalla Homepage)
- Aggiungere la classe `d-none` all'elemento originale.

### 📝 Modifica del Margine in **Privacy Policy, Media Policy e Note Legali**
1. Seleziona il contenuto della pagina e fai clic su **🖋️ Modifica il layout**.
2. Vai su **⚙️ Modifica > Layout**.
3. Modifica il margine superiore impostandolo a `-2rem`.
4. 💾 Salva le modifiche.

### 📝 Modifiche alle Pagine **Media Policy, Note Legali, Privacy Policy**
- ✏️ Modificare breadcrumb e titolo delle pagine per adeguare l'utilizzo delle minuscole.
- 🔍 In **Note Legali**, verificare il comportamento del link esterno spuntando l'opzione per l'apertura in un'altra scheda.

---
## 🏗️ 2. Modifiche al Footer
1. Vai su **🎨 Aspetto > Editor del Tema**.
2. Apri il file `footer.php`.
3. 📂 Sostituisci l'intero contenuto con il file `footer.php` presente in `utils/templates`.
4. 💾 Salva le modifiche.

---
## 🏗️ 3. Modifiche al Single Faq
1. Vai su **🎨 Aspetto > Editor del Tema**.
2. Apri il file `single-faq.php`.
3. 📂 Sostituisci l'intero contenuto con il file `single-faq.php` presente in `utils/templates`.
4. 💾 Salva le modifiche.


---
## 📌 5. Modifiche al Menu
### 📑 Contenuto
1. Vai su **🎨 Aspetto > Editor del Tema**.
2. Apri il file `menu.php`.
3. 📂 Sostituisci l'intero contenuto con il file `menu.php` presente in `utils/templates`.
4. 💾 Salva le modifiche.
### 🔗 Elementi
1. Vai su **🎨 Aspetto > Menu**.
2. ➕ Aggiungi o modifica gli elementi del menu secondo le tue necessità.
  - **📂 Accessibilità per** (link personalizzato) con al suo interno:
    - 🏛️ Pubbliche Amministrazioni
    - 👤 Soggetti privati
    - 🏠 Cittadini
    - 💻 Designer e developers
  - 📚 Formazione
  - 📎 Risorse
  - 🇪🇺 PNRR (tipo sidebar)
3. 💾 Salva le modifiche.

---
## 🔍 5. Modifiche al Search Form
1. Vai su **🎨 Aspetto > Editor del Tema**.
2. Apri il file `searchform.php`.
3. 🛠️ Alla riga 4, aggiungi `type="submit"` al tag del pulsante.
4. 💾 Salva le modifiche.

---
## 📦 6. Installazione del Plugin "AgidUtility"
### ✅ Verifica **Max Upload Size**
Prima di procedere con l'installazione, assicurati che il valore di `max upload size` sia adeguato. Puoi verificarlo in:
- **🛠️ Strumenti > Salute del Sito**
- Oppure eseguendo `phpinfo()`

### 📥 Installazione
1. Vai su **🔌 Plugin > Aggiungi Nuovo**.
2. Clicca su **📤 Carica Plugin**.
3. 📂 Trascina il file `AgidUtility.zip`.
4. Clicca su **📥 Installa Ora**, poi **✅ Attiva**.

---
## 🛠️ 7. Installazione e Configurazione dei vari plugins

### 🛠️ 1. Installazione e Configurazione di Advanced Editor Tool
1. Vai su **🔌 Plugin > Aggiungi Nuovo**.
2. 🔎 Cerca **"Advanced Editor Tool"**.
3. 📥 Installa e attiva il plugin.
4. Vai su **Plugin > Advanced Editor Tool > Impostazioni > Importa**.
5. 📂 Importa le impostazioni da `resources`.

### 🛠️ 2. Installazione e Configurazione di ACF Plugin
1. Vai su **🔌 Plugin > Aggiungi Nuovo**.
2. 🔎 Cerca **"Advanced Custom Fields Pro"**.
3. 📥 Installa e attiva il plugin.
4. Vai su **ACF > Strumenti**.
5. 📂 Importa i campi personalizzati necessari da `resources`.


---
## 📄 8. Creazione della Pagina "Domande Frequenti"
1. Vai su **📑 Pagine > Aggiungi Nuova**.
2. ✏️ Imposta il titolo **"Domande Frequenti"**.
3. Inserisci il seguente shortcode nel contenuto della pagina:
   ```md
   [filter_categories]
   ```
4. Seleziona come **🖼️ template** la versione senza sidebar.
5. 🆔 Imposta lo **slug** a `domande-frequenti`.
6. 💾 Salva e pubblica la pagina.

## 📥 9. Importazione dei Contenuti di FAQ, Risorse e Sidebar
1. Vai su **📂 Strumenti > Importa**.
2. Seleziona **WordPress** e clicca su **Installa Ora**.
3. 📂 Carica i file necessari dalla cartella `resources`.
4. 💾 Salva le modifiche.

---
## 🏗️ 10. Configurazione della Sidebar
- 🛠️ Correzione dei link della sidebar:
  1. 🔌 Installare il plugin **remove CPT base**.
  2. Durante la configurazione selezionare **Sidebar**.

---
## 🖼️ 11. Importazione Immagini per "Guida alla Piattaforma", "Footer" e "Favicon"
1. Vai su **📂 Media > Aggiungi Nuovo**.
2. 📤 Carica le immagini necessarie dalla cartella `resources/media`.

---
## 🌐 12. Importazione e Caricamento della Favicon
1. Vai su **🎨 Aspetto > Personalizza > Denominazione del Sito**.
2. 📤 Carica la favicon nel formato consigliato (`.ico`, `.png`, `.svg`).
3. 💾 Salva le modifiche.

---
## 🔔 Note Finali
- 🔄 **Esegui un backup** del sito prima di apportare modifiche ai file del tema.
- ✅ Dopo ogni modifica, verifica il **corretto funzionamento del sito**.
- 🛠️ Per eventuali problemi, controlla la **console degli errori del browser** o i **log di WordPress**.

---

**🎯 Fine della procedura.** ✅

