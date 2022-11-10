---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Metadata
fileformat: Gif
productName: Java
lang: it
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Metadata signature on Gif for Java

############################# Head ############################
head_title: "Aggiungi firme elettroniche di metadati a documenti Gif tramite Java"
head_description: "Usa i metadati come firme elettroniche nascoste all'interno dei tuoi documenti Gif utilizzando un paio di righe di codice Java. Usa l'API per la firma dei documenti di GroupDocs per firmare elettronicamente i tuoi documenti e file aziendali con informazioni sui metadati."

############################# Header ############################
title: "Le firme elettroniche dei metadati per il documento Gif tramite Java sono semplici e facili da usare!"
description: "Firma elettronicamente i tuoi documenti e contratti Gif con voci di metadati nascoste. Genera metadati per PDF, documenti MS Word, cartelle di lavoro MS Excel, presentazioni MS PowerPoint e vari formati di immagine senza problemi e codifica aggiuntiva."
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
    title: "Informazioni su GroupDocs.Signature for Java API delle firme dei metadati"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) è un'API popolare per la firma elettronica di documenti digitali. Sono disponibili firme come testi, immagini, certificati digitali, codici a barre, codici QR, timbri o metadati. Le firme possono essere posizionate su PDF, documenti MS Word, cartelle di lavoro MS Excel, presentazioni MS PowerPoint, file Adobe Photoshop e vari formati di immagine. I clienti possono firmare il proprio documento e aggiornare, cercare, verificare, eliminare o visualizzare in anteprima le firme elettroniche che sono state apposte su tali documenti. Inoltre, vengono fornite molte abilità per la personalizzazione delle firme.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Passaggi per firmare Gif con Metadata in Java"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) offre la possibilità di firmare documenti Gif con firme Metadata in modo rapido e semplice.
        
        * Crea un'istanza della classe Signature che fornisce il file Gif che dovrebbe firmare come percorso o flusso di memoria
        * Crea un'istanza della classe SignOptions e imposta tutti i dati richiesti.
        * Richiama il metodo Signature.Sign() passando il file di output Gif o il flusso di memoria

    title_right: " Requisiti di sistema"
    content_right: |
        GroupDocs.Signature for Java sono supportati su tutte le principali piattaforme e sistemi operativi. Prima di eseguire il codice seguente, assicurati di avere i seguenti prerequisiti installati sul tuo sistema.

        * Sistemi operativi: Microsoft Windows, Linux, MacOS
        * Ambienti di sviluppo: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Ricevi l'ultimo GroupDocs.Signature for Java da [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Gif file
        String filePath = "input.gif";
        // Set up output file
        String outputFilePath = "output.gif";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // instantiate metadata signing options
        MetadataSignOptions options = new MetadataSignOptions();

        // Specify different Metadata Signatures and add them to options signature collection
        // set start id
        int imgsMetadataId = 41996;
        // setup int value
        ImageMetadataSignature mdSign_DocId = new ImageMetadataSignature(imgsMetadataId++, 123456); // int
        options.getSignatures().add(mdSign_DocId);
        // setup Author property
        ImageMetadataSignature mdSign_Author = new ImageMetadataSignature(imgsMetadataId++, "Mr.Scherlock Holmes"); // string
        options.getSignatures().add(mdSign_Author);
        // setup data of sign date
        ImageMetadataSignature mdSign_Date = new ImageMetadataSignature(imgsMetadataId++, new Date()); // DateTime
        options.getSignatures().add(mdSign_Date);
        // setup double
        ImageMetadataSignature mdSign_Amnt = new ImageMetadataSignature(imgsMetadataId++, 123.456); //decimal value
        options.getSignatures().add(mdSign_Amnt);

        // sign Gif document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Firma di documenti Gif con Metadata Demo live"
    content: |
       Firma subito il file Gif con varie firme visitando il sito web [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Demo online gratuita ti aspetta.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Altre firme Metadata supportate per Java"
    content: |
        "Puoi anche firmare Gif con altri tipi di firma. Si prega di consultare l'elenco di seguito."
    format: 
       
       
back_to_top:
    enable: true
---