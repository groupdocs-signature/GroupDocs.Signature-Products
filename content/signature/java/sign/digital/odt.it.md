---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Digital
fileformat: Odt
productName: Java
lang: it
productCode: java
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Odt for Java

############################# Head ############################
head_title: "Aggiunta di firme elettroniche digitali al file Odt con Java"
head_description: "Inserisci la firma digitale sul file Odt per Java utilizzando poche righe di codice. Usa l'API per la firma dei documenti di GroupDocs per firmare decine di formati di file."

############################# Header ############################
title: "eSign file Odt con firme Digital in Java"
description: "Come aggiungere la firma Digital con poche righe di codice Java"
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
    title: "Informazioni su GroupDocs.Signature for Java API delle firme digitali"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) è un'API popolare per la firma di documenti con firme elettroniche digitali, con certificati digitali. Per le firme digitali API utilizza i file di certificato PFX per firmare documenti con chiavi private e pubbliche protette da password. Le firme digitali possono essere utilizzate per certificare documenti aziendali con una pagina particolare PDF eSign, certificare interi documenti di Microsoft Office come Word, Excel, file Powerpoint e documenti Open Office. I clienti possono facilmente manipolare le firme come modificarle, rimuoverle o modificarle. L'API fornisce un modo per cercare e verificare le firme. Inoltre, vengono fornite molte abilità per la personalizzazione delle firme.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Passaggi per firmare Odt con Digital in Java"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) offre la possibilità di firmare documenti Odt con firme Digital in modo rapido e semplice.
        
        * Crea un'istanza della classe Signature che fornisce il file Odt che dovrebbe firmare come percorso o flusso di memoria
        * Crea un'istanza della classe SignOptions e imposta tutti i dati richiesti.
        * Richiama il metodo Signature.Sign() passando il file di output Odt o il flusso di memoria

    title_right: " Requisiti di sistema"
    content_right: |
        GroupDocs.Signature for Java sono supportati su tutte le principali piattaforme e sistemi operativi. Prima di eseguire il codice seguente, assicurati di avere i seguenti prerequisiti installati sul tuo sistema.

        * Sistemi operativi: Microsoft Windows, Linux, MacOS
        * Ambienti di sviluppo: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Ricevi l'ultimo GroupDocs.Signature for Java da [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Odt file
        String filePath = "input.odt";
        // Set up output file
        String outputFilePath = "output.odt";
        // Provide digital certificate
        String certificateFilePath = "certificate.pfx";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Provide sign options
        DigitalSignOptions options = new DigitalSignOptions(certificateFilePath);

        // set certificate password
        options.setPassword("1234567890");

        // set signature position
        options.setLeft(50);
        options.setTop(200);

        // sign Odt document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Firma di documenti Odt con Digital Demo live"
    content: |
       Firma subito il file Odt con varie firme visitando il sito web [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Demo online gratuita ti aspetta.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Altre firme Digital supportate per Java"
    content: |
        "Puoi anche firmare Odt con altri tipi di firma. Si prega di consultare l'elenco di seguito."
    format: 
       
       
back_to_top:
    enable: true
---