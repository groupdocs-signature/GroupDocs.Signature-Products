---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Qrcode
codetype: G S1 Q R
fileformat: Dotx
productName: Java
lang: it
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put  Qrcode signature on Dotx for Java

############################# Head ############################
head_title: "eSign Dotx documento con G S1 Q R codice QR in Java"
head_description: "Crea il codice QR G S1 Q R e inseriscilo nel file Dotx utilizzando Java con un breve pezzo di codice Java. Usa l'API per la firma dei documenti di GroupDocs per firmare elettronicamente i tuoi documenti e file aziendali con il codice QR."

############################# Header ############################
title: "Genera G S1 Q R firma del codice QR per il documento Dotx in Java"
description: "Firma i tuoi documenti e contratti Dotx con il codice QR G S1 Q R. Genera la firma del codice QR in modo rapido e semplice."
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true

    left:
        img_alt: "GroupDocs.Signature for Java"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocs-signature-java.png"
        product: "GroupDocs.Signature"
        platform: "Java"



############################# About ############################
about:
    enable: true
    title: "Informazioni su GroupDocs.Signature for Java API per le firme del codice QR"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) è un'API matura per la creazione e la generazione di firme QR Code per i documenti. Gli utenti possono generare firme QR Code fornendo testo per scaricarlo o condividerlo sui social media come immagine. Il documento firmato può essere scansionato con API o semplicemente tramite la fotocamera mobile! Firma elettronicamente i tuoi contratti commerciali e documenti ufficiali aggiungendo la firma del codice QR e manipolalo. Qualsiasi firma del codice QR conterrà informazioni personalizzate univoche per identificare il firmatario o autorizzare il documento. Inoltre, il contenuto del QR Code può essere crittografato e decrittografato con chiavi personali in modo programmatico. Ciò apre molte possibilità di condividere dati sensibili all'interno dei documenti pubblici. Dopo la firma, l'utente può aggiornare, verificare, eliminare, visualizzare in anteprima o cercare i codici QR all'interno di PDF, documenti MS Word, cartelle di lavoro MS Excel, presentazioni MS PowerPoint, file Adobe Photoshop e vari formati di immagine. I codici QR possono essere ulteriormente personalizzati.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Passaggi per firmare Dotx con Qrcode in Java"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) offre la possibilità di firmare documenti Dotx con firme Qrcode in modo rapido e semplice.
        
        * Crea un'istanza della classe Signature che fornisce il file Dotx che dovrebbe firmare come percorso o flusso di memoria
        * Crea un'istanza della classe SignOptions e imposta tutti i dati richiesti.
        * Richiama il metodo Signature.Sign() passando il file di output Dotx o il flusso di memoria

    title_right: " Requisiti di sistema"
    content_right: |
        GroupDocs.Signature for Java sono supportati su tutte le principali piattaforme e sistemi operativi. Prima di eseguire il codice seguente, assicurati di avere i seguenti prerequisiti installati sul tuo sistema.

        * Sistemi operativi: Microsoft Windows, Linux, MacOS
        * Ambienti di sviluppo: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Ricevi l'ultimo GroupDocs.Signature for Java da [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Dotx file
        String filePath = "input.dotx";
        // Set up output file
        String outputFilePath = "output.dotx";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // create barcode option with predefined barcode text
        BarcodeSignOptions options = new BarcodeSignOptions("John Smith");

        // setup Barcode encoding type
        options.setEncodeType(QrCodeTypes.G S1 Q R);

        // set signature position
        options.setLeft(50);
        options.setTop(50);
        options.setWidth(200);
        options.setHeight(50);

        // sign Dotx document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Firma di documenti Dotx con Qrcode Demo live"
    content: |
       Firma subito il file Dotx con varie firme visitando il sito web [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Demo online gratuita ti aspetta.

              
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-barcode"
          title: "About G S1 Q R QrCode"
          content: |
            Il codice QR GS1 è una variante del codice QR conforme alle specifiche GS1. È stato progettato specificamente per condividere informazioni estese sull'imballaggio, come numero di lotto, ID prodotto e quantità.
          characterset: |
             Lettere maiuscole e minuscole e caratteri speciali $%*+-./: tutti con Application Identifier corretti
          textcapacity: |
             Fino a 7089 caratteri numerici, 4296 caratteri alfanumerici
          image: |
             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

          link: ""

############################# More Formats ############################
more_formats:
    enable: true
    title: "Altre firme Qrcode supportate per Java"
    content: |
        "Puoi anche firmare Dotx con altri tipi di firma. Si prega di consultare l'elenco di seguito."
    format: 
        
       
back_to_top:
    enable: true
---