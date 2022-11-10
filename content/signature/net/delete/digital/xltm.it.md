---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Delete
signaturetype: Digital
fileformat: Xltm
productName: .NET
lang: it
productCode: net
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Xltm for C#

############################# Head ############################
head_title: "Elimina le firme Digital dai file Xltm tramite C#"
head_description: "L'eliminazione di firme Digital specifiche da documenti Xltm firmati può essere eseguita facilmente con il codice .NET breve."

############################# Header ############################
title: "Rimuovi le firme Digital che sono inserite nei file Xltm"
description: "Elimina varie firme Digital da documenti Xltm. La rimozione delle firme Digital richiede un semplice codice C#."
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true

    left:
        img_alt: "GroupDocs.Signature for .NET"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocs-signature-net.png"
        product: "GroupDocs.Signature"
        platform: ".NET"



############################# About ############################
about:
    enable: true
    title: "Ottieni informazioni sulle funzionalità dell'API GroupDocs.Signature for .NET"
    content: |
        L'API [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) fornisce molti modi per elaborare i tuoi documenti utilizzando le firme elettroniche. Sono disponibili firme digitali come testi, immagini, certificati digitali, codici a barre, codici QR, timbri o metadati. I clienti hanno la possibilità di aggiungere, eliminare, aggiornare, verificare o cercare firme digitali su PDF, documenti MS Word, cartelle di lavoro MS Excel, presentazioni MS PowerPoint, file Adobe Photoshop e vari formati di immagine. Viene fornito un gran numero di funzioni e impostazioni utili.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Come rimuovere le firme Digital dal tuo documento Xltm"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) fornisce una funzione utile per cancellare documenti Xltm di firme Digital con poche righe di codice.
        
        * In primo luogo, istanziare l'oggetto Signature passando il percorso al documento come parametro del costruttore.
        * Quindi, crea un oggetto firma appropriato e imposta il suo identificatore univoco.
        * Dopodiché, invoca il metodo Delete passando l'oggetto della firma che deve essere eliminato.
        * Infine, i risultati dell'operazione di processo.

    title_right: "Requisiti di sistema"
    content_right: |
        GroupDocs.Signature for .NET sono supportati su tutte le principali piattaforme e sistemi operativi. Prima di eseguire il codice seguente, assicurati di avere i seguenti prerequisiti installati sul tuo sistema.

        * Sistemi operativi: Microsoft Windows, Linux, MacOS
        * Ambienti di sviluppo: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Scarica l'ultima versione di GroupDocs.Signature for .NET da [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Xltm file
        string filePath = "input.xltm";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                // Id of signature which is supposed to be deleted
                // such Id may be obtained as result of search operation
                string id = "a01e1940-997a-444b-89af-9309a2d559a5";

                // provide signature features to delete
                // set up particular signature id
                DigitalSignature signatureToDelete = new DigitalSignature(id);

                // delete signature
                bool deleteResult = signature.Delete(signatureToDelete);

                // process deletion result
                if (deleteResult)
                {
                    Console.WriteLine("Signature was deleted successfully!");
                }
        }
        ```

############################# Demos ############################
demos:
    enable: true
    title: "Firma con Digital firme Demo live"
    content: |
       Aggiungi subito varie firme elettroniche al file Xltm visitando il sito Web [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Elimina le tue firme Digital con C#"
    content: |
        "Cancellazione delle firme elettroniche che sono state aggiunte a vari formati di documenti. Rimuovi rapidamente le firme senza codice aggiuntivo."
    format: 
       
       
back_to_top:
    enable: true
---