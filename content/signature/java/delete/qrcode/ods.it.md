---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Delete
signaturetype: Qrcode
fileformat: Ods
productName: Java
lang: it
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Qrcode signature on Ods for Java

############################# Head ############################
head_title: "Elimina le firme Qrcode dai file Ods tramite Java"
head_description: "L'eliminazione di firme Qrcode specifiche da documenti Ods firmati può essere eseguita facilmente con il codice Java breve."

############################# Header ############################
title: "Rimuovi le firme Qrcode che sono inserite nei file Ods"
description: "Elimina varie firme Qrcode da documenti Ods. La rimozione delle firme Qrcode richiede un semplice codice Java."
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
    title: "Ottieni informazioni sulle funzionalità dell'API GroupDocs.Signature for Java"
    content: |
        L'API [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) fornisce molti modi per elaborare i tuoi documenti utilizzando le firme elettroniche. Sono disponibili firme digitali come testi, immagini, certificati digitali, codici a barre, codici QR, timbri o metadati. I clienti hanno la possibilità di aggiungere, eliminare, aggiornare, verificare o cercare firme digitali su PDF, documenti MS Word, cartelle di lavoro MS Excel, presentazioni MS PowerPoint, file Adobe Photoshop e vari formati di immagine. Viene fornito un gran numero di funzioni e impostazioni utili.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Come rimuovere le firme Qrcode dal tuo documento Ods"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) fornisce una funzione utile per cancellare documenti Ods di firme Qrcode con poche righe di codice.
        
        * In primo luogo, istanziare l'oggetto Signature passando il percorso al documento come parametro del costruttore.
        * Quindi, crea un oggetto firma appropriato e imposta il suo identificatore univoco.
        * Dopodiché, invoca il metodo Delete passando l'oggetto della firma che deve essere eliminato.
        * Infine, i risultati dell'operazione di processo.

    title_right: "Requisiti di sistema"
    content_right: |
        GroupDocs.Signature for Java sono supportati su tutte le principali piattaforme e sistemi operativi. Prima di eseguire il codice seguente, assicurati di avere i seguenti prerequisiti installati sul tuo sistema.

        * Sistemi operativi: Microsoft Windows, Linux, MacOS
        * Ambienti di sviluppo: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Scarica l'ultima versione di GroupDocs.Signature for Java da [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Ods file
        String filePath = "input.ods";
        // Set up output file
        String outputFilePath = "output.ods";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // Id of signature which is supposed to be deleted
        // such Id may be obtained as result of search operation
        String id = "eff64a14-dad9-47b0-88e5-2ee4e3604e71";

        // provide signature features to delete
        QrCodeSignature signatureToDelete = new QrCodeSignature(id);

        // delete signature
        Boolean deleteResult = signature.delete(outputFilePath, signatureToDelete);

        // process deletion result
        if (deleteResult)
        {
                System.out.println("Signature was deleted successfully!");
        }
        ```

############################# Demos ############################
demos:
    enable: true
    title: "Firma con Qrcode firme Demo live"
    content: |
       Aggiungi subito varie firme elettroniche al file Ods visitando il sito Web [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Elimina le tue firme Qrcode con Java"
    content: |
        "Cancellazione delle firme elettroniche che sono state aggiunte a vari formati di documenti. Rimuovi rapidamente le firme senza codice aggiuntivo."
    format: 
       
       
back_to_top:
    enable: true
---