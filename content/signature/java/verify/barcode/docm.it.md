---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Verify
signaturetype: Barcode
fileformat: Docm
productName: Java
lang: it
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Barcode signature on Docm for Java

############################# Head ############################
head_title: "Verifica delle firme Barcode per i file Docm tramite Java"
head_description: "Utilizza solo poche righe di codice Java per verificare i documenti Docm e le relative firme Barcode."

############################# Header ############################
title: "Verifica delle firme Barcode per i file Docm"
description: "L'API per Java offre l'opportunità di verificare le firme Barcode nei documenti Docm. La verifica delle firme elettroniche all'interno dei tuoi documenti Docm potrebbe essere eseguita in modo rapido e semplice."
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
    title: "Scopri le nuove funzionalità dell'API GroupDocs.Signature for Java"
    content: |
        L'API [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) offre un'ampia gamma di modi per elaborare numerosi formati di documenti utilizzando le firme elettroniche. Sono supportati molti tipi di firme digitali come testi, immagini, certificati digitali, codici a barre, codici QR, timbri o metadati. I clienti possono aggiungere, rimuovere, modificare, convalidare o cercare firme digitali in PDF, documenti MS Word, cartelle di lavoro MS Excel, presentazioni MS PowerPoint, file Adobe Photoshop e vari formati di immagine. È disponibile un numero sorprendente di funzioni e impostazioni aggiuntive.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Come convalidare le firme Barcode nel tuo documento Docm"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) include funzioni utili come la verifica delle firme Barcode apposte in Docm documenti. Usa questa opportunità senza implementare codice aggiuntivo.
        
        * In primo luogo, istanziare la classe Signature fornendo come parametro del costruttore il percorso di un documento che dovrebbe essere verificato.
        * In secondo luogo, crea un nuovo oggetto VerifyOptions e imposta tutte le proprietà richieste.
        * Infine, richiama il metodo Verify dell'oggetto di Signature passando l'istanza di VerifyOptions.
        * Quindi elaborare i risultati della verifica.

    title_right: "Requisiti di sistema"
    content_right: |
        GroupDocs.Signature for Java sono supportati su tutte le principali piattaforme e sistemi operativi. Prima di eseguire il codice seguente, assicurati di avere i seguenti prerequisiti installati sul tuo sistema.

        * Sistemi operativi: Microsoft Windows, Linux, MacOS
        * Ambienti di sviluppo: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Scarica l'ultima versione di GroupDocs.Signature for Java da [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Docm file
        String filePath = "input.docm";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Provide verification options
        BarcodeVerifyOptions options = new BarcodeVerifyOptions();

        // process only specified page 
        options.setPageNumber(2);
        options.setAllPages(false);
        // specify text match type
        options.setMatchType(TextMatchType.Contains);
        // specify text pattern to search
        options.setText("Special signature");
                            
        // Verify document signatures
        VerificationResult result = signature.verify(options);

        //process result
        if (result.isValid())
        {
            //..
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Firma con Barcode firme Demo live"
    content: |
       Aggiungi subito varie firme elettroniche al file Docm visitando il sito Web [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Verifica altre firme Barcode utilizzando Java"
    content: |
        "Verifica delle firme elettroniche apposte nei vari documenti. Controlla la qualità delle firme nei formati di file più diffusi come mostrato di seguito."
    format: 
       
       
back_to_top:
    enable: true
---