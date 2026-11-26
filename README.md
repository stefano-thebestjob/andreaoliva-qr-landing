# Andrea Oliva & Partners S.r.l. – QR landing page

## English

A single static page (`index.html`, no dependencies, no external requests) meant to be opened by scanning a QR code. It shows the main company data from the Italian Business Register extract dated 11/04/2026 (REA number, tax/VAT code, registered office, PEC, contact details) and a **Save contact** button that downloads a vCard (`Andrea-Oliva-Partners.vcf`) for the phone's address book. The page is in English.

### Hosting
- **GitHub Pages:** repository *Settings > Pages > Build and deployment > Deploy from a branch*, branch `main`, folder `/ (root)`. The page will be available at `https://stefano-thebestjob.github.io/andreaoliva-qr-landing/`.
- **Own hosting:** upload `index.html` to the hosting of andreaoliva.eu (for example in a folder such as `/info/`).

### Generating the QR code
Once the final public URL is known, paste it into any QR code generator (use a static, non-expiring QR code) and download it as SVG or high-resolution PNG. Scan it with a phone to test before printing.

### Editing the data
Visible data is plain HTML in `index.html`. The contact card is the `vcard` array in the `<script>` block at the bottom of the file (vCard 3.0; escape commas and semicolons with a backslash).

### TODO
- Add a regular (non-PEC) email address: see the `TODO` comment in the Contact section and add an `EMAIL;TYPE=WORK:` line to the vCard.
- Add the logo (`logo.png`) – not added yet; the page currently uses a text wordmark.
- Refresh the Business Register data (REA, PEC, etc.) when a newer extract is available; update the date in the footer.
- The professional register registration number is not in the extract and is not shown.

## Italiano

Pagina statica unica (`index.html`, senza dipendenze né richieste esterne) pensata per essere aperta inquadrando un QR code. Mostra i dati principali della visura camerale dell'11/04/2026 (numero REA, codice fiscale/partita IVA, sede legale, PEC, contatti) e un pulsante **Save contact** che scarica una scheda contatto (`Andrea-Oliva-Partners.vcf`) per la rubrica dello smartphone. Il testo della pagina è in inglese.

### Pubblicazione
- **GitHub Pages:** *Settings > Pages > Build and deployment > Deploy from a branch*, branch `main`, cartella `/ (root)`. Indirizzo: `https://stefano-thebestjob.github.io/andreaoliva-qr-landing/`.
- **Hosting proprio:** caricare `index.html` sull'hosting di andreaoliva.eu (per esempio in una cartella come `/info/`).

### Creare il QR code
Con l'indirizzo pubblico definitivo, incollarlo in un generatore di QR code (scegliere un QR statico, senza scadenza) e scaricarlo in SVG o PNG ad alta risoluzione. Provare la scansione prima della stampa.

### Modificare i dati
I dati visibili sono HTML semplice in `index.html`. La scheda contatto è l'array `vcard` nel blocco `<script>` in fondo al file (vCard 3.0; virgole e punti e virgola vanno preceduti da una barra rovesciata).

### Da fare
- Aggiungere un indirizzo email ordinario (non PEC): vedere il commento `TODO` nella sezione Contact e aggiungere una riga `EMAIL;TYPE=WORK:` alla vCard.
- Aggiungere il logo (`logo.png`), non ancora inserito; per ora la pagina usa un wordmark testuale.
- Aggiornare i dati del Registro Imprese (REA, PEC, ecc.) con una visura più recente e la data nel piè di pagina.
- Il numero di iscrizione al ruolo agenti non è nella visura e non viene mostrato.
