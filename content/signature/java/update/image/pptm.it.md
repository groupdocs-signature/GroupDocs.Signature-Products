---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Update
signaturetype: Image
fileformat: Pptm
productName: Java
lang: it
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Image signature on Pptm for Java

############################# Head ############################
head_title: "Aggiorna le firme Image inserite nei file Pptm con Java"
head_description: "Utilizza il codice Java semplice e facile per l'aggiornamento delle firme Image nei documenti Pptm firmati."

############################# Header ############################
title: "Modifica e aggiorna le firme Image inserite nei file Pptm"
description: "L'API per Java fornisce funzionalità per l'aggiornamento delle firme Image nei documenti Pptm. Aggiorna le firme elettroniche all'interno dei tuoi documenti Pptm con un paio di righe di codice Java in modo rapido e semplice."
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
    title: "Ulteriori informazioni sulle funzionalità dell'API GroupDocs.Signature for Java"
    content: |
        La funzionalità dell'API [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) contiene un'ampia selezione di mezzi per elaborare i formati di documenti richiesti utilizzando le firme elettroniche. È supportato un ampio spettro di firme elettroniche come testi, immagini, certificati digitali, codici a barre, codici QR, timbri o metadati. I clienti possono aggiungere, rimuovere, modificare, convalidare o cercare firme digitali in PDF, documenti MS Word, cartelle di lavoro MS Excel, presentazioni MS PowerPoint, file Adobe Photoshop e vari formati di immagine. Sono disponibili numerose funzioni e impostazioni utili.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Come modificare le firme Image nel tuo documento Pptm"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) include funzioni utili come l'aggiornamento di firme Image apposte in documenti Pptm. Consente di modificare le caratteristiche delle firme senza codice aggiuntivo.
        
        * Per cominciare, crea l'oggetto Signature passando come percorso del parametro del costruttore a un documento che dovrebbe essere aggiornato.
        * Quindi, crea un'istanza di un particolare oggetto di firma appropriato e imposta il suo identificatore e le proprietà che devono essere modificate.
        * Infine, chiama il metodo di aggiornamento della firma passando un particolare oggetto di firma.
        * Elabora i risultati dell'aggiornamento a tuo avviso.

    title_right: "Requisiti di sistema"
    content_right: |
        GroupDocs.Signature for Java sono supportati su tutte le principali piattaforme e sistemi operativi. Prima di eseguire il codice seguente, assicurati di avere i seguenti prerequisiti installati sul tuo sistema.

        * Sistemi operativi: Microsoft Windows, Linux, MacOS
        * Ambienti di sviluppo: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Scarica l'ultima versione di GroupDocs.Signature for Java da [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Pptm file
        String filePath = "input.pptm";
        // Set up output file
        String outputFilePath = "output.pptm";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // Id of signature which is supposed to be updated
        // such Id might be got as a result of search operation
        String id = "ff988ab1-7403-4c8d-8db7-f2a56b9f8530";

        // provide signature features to update
        // set up particular signature id
        ImageSignature signatureToUpdate = new ImageSignature(id);

        // specify signature width
        signatureToUpdate.setWidth(170);
        // specify signature height
        signatureToUpdate.setHeight(250);
        // set left position
        signatureToUpdate.setLeft(10);
        // set top position
        signatureToUpdate.setTop(10);

        // update signature
        Boolean updateResult = signature.update(outputFilePath, signatureToUpdate);

        // process updation result
        if (updateResult)
        {
                System.out.println("Signature was updated successfully!");
        }
        ```

############################# Demos ############################
demos:
    enable: true
    title: "Aggiornamento delle firme Image nelle pagine del documento - Demo dal vivo"
    content: |
       Modifica subito diverse firme elettroniche del documento Pptm visitando il sito Web [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Aggiorna varie firme Image tramite Java"
    content: |
        "Modifica delle firme digitali che vengono inserite in vari formati di documenti. Aggiorna i dati delle firme senza codice aggiuntivo."
    format: 
       
       
back_to_top:
    enable: true
---