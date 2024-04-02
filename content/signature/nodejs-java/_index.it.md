---
############################# Static ############################
layout: "landing"
date: 2024-04-02T11:33:18
draft: false
#operation: 
#signaturetype: 
#fileformat: 
#productName: Node.js
lang: it
#productCode: nodejs-java
#otherformats: 
#breadcrumb: Put  signature on  for JavaScript
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Drop-down ############################
supported_platforms:
  items:
    # supported_platforms loop
    - title: ".NET"
      tag: "net"
    # supported_platforms loop
    - title: "Java"
      tag: "java"
    # supported_platforms loop
    - title: "Node.js"
      tag: "nodejs-java"

############################# Head ############################
head_title: "API di firma digitale Node.js - GroupDocs.Signature"
head_description: "Integra firme elettroniche sicure nelle app Node.js con GroupDocs.Signature. Semplifica i flussi di lavoro per la firma dei documenti in modo semplice ed efficiente."

############################# Header ############################
title: "Firmare documenti<br>con l'API Node.js"
description: "Firma documenti digitali e immagini su qualsiasi piattaforma utilizzando le nostre API flessibili e soluzioni basate su app per programmatori e utenti finali."
words:
  for: "per"

actions:
  main: "Scarica da NPM"
  main_link: "https://www.npmjs.com/package/@groupdocs/groupdocs.signature/"
  alt: "Licenza"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/nodejs-java/"
  title: "Pronti per iniziare?"
  description: "Prova gratuitamente le funzionalità di GroupDocs.Signature o richiedi una licenza"

release:
  title: "Rilasciata la versione {0}"
  notes: "Scopri le novità"
  downloads: "Download"

code:
  title: "Firma dei PDF tramite Node.js"
  more: "Altri esempi"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Node.js-via-Java/"
  install: "npm i @groupdocs/groupdocs.signature"
  content: |
    ```javascript {style=abap}   
    // Seleziona il documento PDF
    let signature = new Signature("sample.pdf");
    
    // Fornire testo
    let options = new TextSignOptions("John Smith");
    
    // Imposta il colore
    options.ForeColor = Color.Red;
    
    // Firma il documento e salvalo su file
    signature.Sign("signed.pdf", options);
    
    ```

############################# Overview ############################
overview:
  enable: true
  title: "Panoramica di GroupDocs.Signature"
  description: "Libreria di firma dei documenti pronta per essere utilizzata nelle applicazioni Node.js"
  features:
    # feature loop
    - title: "Soluzione di firma digitale per documenti aziendali con Node.js"
      content: "GroupDocs.Signature for Node.js via Java offre una serie completa di opzioni di firma digitale per PDF, documenti Office e immagini. Sono disponibili testo, codici a barre, immagini, certificati digitali e metadati. L'elaborazione semplificata dei documenti garantisce efficienza."

    # feature loop
    - title: "Manipolazione avanzata dei documenti firmati"
      content: "GroupDocs.Signature ti consente di elaborare documenti firmati. Cerca e convalida le firme utilizzando vari criteri. Inoltre, estrai informazioni dettagliate sul documento o genera immagini di anteprima delle pagine."

    # feature loop
    - title: "Diversi formati di output"
      content: "La nostra soluzione fornisce un controllo completo sul formato di output dei documenti firmati. Posiziona con precisione le firme su qualsiasi pagina e personalizza il loro aspetto. Salva i documenti firmati in numerosi formati supportati e, facoltativamente, proteggili con password."

############################# Platforms ############################
platforms:
  enable: true
  title: "Indipendenza dalla piattaforma"
  description: "GroupDocs.Signature for Node.js via Java esegue l'elaborazione dei documenti con vari sistemi operativi"
  items:
    # platform loop
    - title: "Amazon"
      image: "amazon"
    # platform loop
    - title: "Docker"
      image: "docker"
    # platform loop
    - title: "Azure"
      image: "azure"
    # platform loop
    - title: "VS Code"
      image: "vs_code"
    # platform loop
    - title: "ReSharper"
      image: "resharper"
    # platform loop
    - title: "macOS"
      image: "finder"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "NuGet"
      image: "nuget"

############################# File formats ############################
formats:
  enable: true
  title: "Formati di file supportati"
  description: |
    GroupDocs.Signature for Node.js via Java facilita le operazioni per i [formati di file più diffusi](https://docs.groupdocs.com/signature/java/supported-document-formats/).
  groups:
    # group loop
    - color: "green"
      content: |
        ### Formati Microsoft Office
        * **Word:**  DOCX, DOC, DOCM, DOT, DOTX, DOTM, RTF
        * **Excel:** XLSX, XLS, XLSM, XLSB, XLTM, XLT, XLTM, XLTX, XLAM, SXC, SpreadsheetML
        * **PowerPoint:** PPT, PPTX, PPS, PPSX, PPSM, POT, POTM, POTX, PPTM
    # group loop
    - color: "blue"
      content: |
        ### Immagini e altri formati
        * **Portatile:** PDF
        * **immagini:** JPG, BMP, PNG, TIFF, GIF, DICOM, WEBP
        * **Altri formati di ufficio:** ODT, OTT, OTS, ODS, ODP, OTP, ODG
      # group loop
    - color: "red"
      content: |
        ### Altri formati
        * **ragnatela:** HTML, MHTML
        * **Archivi:** ZIP, TAR, 7Z
        * **Certificati:** PFX

############################# Features ############################
features:
  enable: true
  title: "Funzionalità di GroupDocs.Signature"
  description: "Firma PDF, documenti Office e immagini con firme digitali"

  items:
    # feature loop
    - icon: "sign"
      title: "Firme aziendali"
      content: "Utilizza vari tipi di firma per firmare i documenti. Posiziona le firme digitali con precisione su qualsiasi posizione della pagina."

    # feature loop
    - icon: "custom"
      title: "Personalizzazione dell'aspetto della firma"
      content: "Personalizza gli aspetti visivi delle firme regolando colore, carattere, bordi, rotazione e altro per ottenere il risultato desiderato."

    # feature loop
    - icon: "password"
      title: "Documenti protetti da password"
      content: "Per molti formati di documenti supportati, proteggi i documenti firmati con una password per una maggiore sicurezza."

    # feature loop
    - icon: "protect"
      title: "Prevenire modifiche non autorizzate"
      content: "Proteggi i documenti aziendali cruciali firmati con certificati digitali da alterazioni non autorizzate."

    # feature loop
    - icon: "convert"
      title: "Formati di output desiderati"
      content: "Ottieni facilmente documenti firmati in qualsiasi formato supportato. Converti facilmente documenti MS Word in formato PDF."

    # feature loop
    - icon: "preview"
      title: "Anteprima dei documenti"
      content: "Salva le singole pagine del documento come immagini per esigenze future."

    # feature loop
    - icon: "search"
      title: "Ricerca di firme"
      content: "Recupera informazioni sulle firme aggiunte in precedenza nei tuoi documenti."

    # feature loop
    - icon: "validate"
      title: "Convalida del documento"
      content: "Verificare l'autenticità delle firme presentate in qualsiasi documento."

    # feature loop
    - icon: "update"
      title: "Gestione delle firme"
      content: "Elimina, riposiziona o modifica qualsiasi firma inserita su qualsiasi pagina del documento."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Esempi di codici"
  description: "Esempi illustrativi che mostrano le operazioni tipiche di GroupDocs.Signature for Node.js via Java"
  items:
    # code sample loop
    - title: "Contrassegna il PDF con i codici QR"
      content: |
        Incorporando [codici a barre](https://docs.groupdocs.com/signature/java/esign-document-with-qr-code-signature/) in pagine specifiche di documenti PDF è possibile semplificare i processi aziendali. Questa sezione fornisce un esempio di aggiunta di un codice QR utilizzando GroupDocs.Signature for Node.js via Java.
        {{< landing/code title="Come inserire il codice QR nel PDF.">}}
        ```javascript {style=abap}
        // Carica il documento da firmare
        let signature = new Signature("file_to_sign.pdf");
        
        // Crea opzioni di codice QR con testo predefinito
        let options = new QrCodeSignOptions("The document is approved by John Smith");
        
        // Configura il tipo di codifica del codice QR e la posizione sulla pagina
        options.EncodeType = QrCodeTypes.QR;
        options.Left = 100;
        options.Top = 100;
            
        // Firma il documento e salvalo come file dei risultati
        signature.Sign("file_with_QR.pdf", options);
        
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Proteggere un DOCX con una Firma Digitale"
      content: |
        [Proteggi i tuoi documenti](https://docs.groupdocs.com/signature/java/esign-document-with-digital-signature/) con firme basate su certificati digitali. La firma digitale protegge i tuoi documenti aziendali dalla modifica dei contenuti.
        {{< landing/code title="Ecco come garantire l'integrità del documento.">}}
        ```javascript {style=abap}   
        // Caricare il documento da firmare digitalmente
        let signature = new Signature("file_to_sign.docx");
        
        // Specificare le opzioni di firma digitale e fornire il percorso del file del certificato
        let options = new DigitalSignOptions("certificate.pfx");

        // Imposta la password del certificato
        options.Password = "1234567890";

        // Firma il documento e salvalo nel percorso desiderato
        signature.Sign("digitally_signed.docx", options);

        ```
        {{< /landing/code >}}

---
