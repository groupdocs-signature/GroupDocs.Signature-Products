---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Search
signaturetype: Qrcode
fileformat: Ott
productName: Java
lang: it
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Search Qrcode signatures at Ott with Java

############################# Head ############################
head_title: "Cerca le firme Qrcode nel file Ott in Java"
head_description: "Usa Java per cercare le firme Qrcode nei file Ott utilizzando poche righe di codice."

############################# Header ############################
title: "Cerca le firme Qrcode nel file Ott"
description: "L'API nativa Java consente di cercare firme Qrcode in file Ott già firmati. Esegui una ricerca avanzata di firme elettroniche all'interno dei tuoi documenti Ott utilizzando poche righe di codice."
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true

    left:
        img_alt: "GroupDocs.Signature for Java"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocsature-java.png"
        product: "GroupDocs.Signature"
        platform: "Java"



############################# About ############################
about:
    enable: true
    title: "Informazioni sull'API GroupDocs.Signature for Java"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) fornisce l'API Java per l'elaborazione di documenti utilizzando vari tipi di firma come testi, immagini, certificati digitali, codici a barre, codici QR, timbri o metadati. Gli utenti possono aggiungere, eliminare, aggiornare, verificare o cercare firme elettroniche all'interno di PDF, documenti MS Word, cartelle di lavoro MS Excel, presentazioni MS PowerPoint, file Adobe Photoshop e vari formati di immagine, con supporto aggiuntivo per la personalizzazione delle proprietà delle firme secondo necessità.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Come cercare le firme Qrcode in Ott"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) consente agli sviluppatori di Java di cercare più facilmente le firme Qrcode nei file Ott dalle loro applicazioni implementando alcuni semplici passaggi.
        
        * Crea una nuova istanza della classe Signature e passa il percorso del documento di origine come parametro del costruttore.
        * Crea un'istanza dell'oggetto SearchOptions in base alle tue esigenze e specifica le opzioni di ricerca.
        * Chiama il metodo di ricerca dell'istanza della classe Signature e passa ad esso SearchOptions.
        * Elabora i risultati della ricerca in base alle tue richieste.

    title_right: "Requisiti di sistema"
    content_right: |
        GroupDocs.Signature for Java sono supportati su tutte le principali piattaforme e sistemi operativi. Prima di eseguire il codice seguente, assicurati di avere i seguenti prerequisiti installati sul tuo sistema.

        * Sistemi operativi: Microsoft Windows, Linux, MacOS
        * Ambienti di sviluppo: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Scarica l'ultima versione di GroupDocs.Signature for Java da [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Ott file
        String filePath = "input.ott";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Create search options
        QrCodeSearchOptions options = new QrCodeSearchOptions();

        // specify special pages to search on 
        options.setAllPages(false);
        // single page number
        options.setPageNumber(1);
        // specify text match type
        options.setMatchType(TextMatchType.Contains);
        // specify text pattern to search
        options.setText("Text signature");
        // return  Qrcode images for processing
        options.setReturnContent(true);
        // set up type of returned  Qrcode images
        options.setReturnContentType(FileType.PNG);
                            
        // search for Qrcode signatures in Ott document
        List<QrCodeSignature> signatures = signature.search(QrCodeSignature.class, options);

        // process signatures which were found 
        signatures.forEach(item -> System.out.println(item.toString()));
        ```

############################# Demos ############################
demos:
    enable: true
    title: "Cerca Qrcode firme elettroniche Demo live"
    content: |
       Cerca subito nel documento varie firme elettroniche nei file Ott visitando il sito Web [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).

        
############################# More Formats ############################
more_formats:
    enable: true
    title: "Cerca altre firme Qrcode utilizzando Java"
    content: |
        "Le firme elettroniche ricercano in vari documenti. Trova le firme da uno dei formati di file più diffusi come mostrato di seguito."
    format: 
           
       
back_to_top:
    enable: true
---