---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Metadata
fileformat: Pps
productName: .NET
lang: it
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Metadata signature on Pps for C#

############################# Head ############################
head_title: "Aggiungi firme elettroniche di metadati a documenti Pps tramite C#"
head_description: "Usa i metadati come firme elettroniche nascoste all'interno dei tuoi documenti Pps utilizzando un paio di righe di codice C#. Usa l'API per la firma dei documenti di GroupDocs per firmare elettronicamente i tuoi documenti e file aziendali con informazioni sui metadati."

############################# Header ############################
title: "Le firme elettroniche dei metadati per il documento Pps tramite .NET sono semplici e facili da usare!"
description: "Firma elettronicamente i tuoi documenti e contratti Pps con voci di metadati nascoste. Genera metadati per PDF, documenti MS Word, cartelle di lavoro MS Excel, presentazioni MS PowerPoint e vari formati di immagine senza problemi e codifica aggiuntiva."
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
    title: "Informazioni su GroupDocs.Signature for .NET API delle firme dei metadati"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) è un'API popolare per la firma elettronica di documenti digitali. Sono disponibili firme come testi, immagini, certificati digitali, codici a barre, codici QR, timbri o metadati. Le firme possono essere posizionate su PDF, documenti MS Word, cartelle di lavoro MS Excel, presentazioni MS PowerPoint, file Adobe Photoshop e vari formati di immagine. I clienti possono firmare il proprio documento e aggiornare, cercare, verificare, eliminare o visualizzare in anteprima le firme elettroniche che sono state apposte su tali documenti. Inoltre, vengono fornite molte abilità per la personalizzazione delle firme.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Passaggi per firmare Pps con Metadata in C#"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) offre la possibilità di firmare documenti Pps con firme Metadata in modo rapido e semplice.
        
        * Crea un'istanza della classe Signature che fornisce il file Pps che dovrebbe firmare come percorso o flusso di memoria
        * Crea un'istanza della classe SignOptions e imposta tutti i dati richiesti.
        * Richiama il metodo Signature.Sign() passando il file di output Pps o il flusso di memoria

    title_right: " Requisiti di sistema"
    content_right: |
        GroupDocs.Signature for .NET sono supportati su tutte le principali piattaforme e sistemi operativi. Prima di eseguire il codice seguente, assicurati di avere i seguenti prerequisiti installati sul tuo sistema.

        * Sistemi operativi: Microsoft Windows, Linux, MacOS
        * Ambienti di sviluppo: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Ricevi l'ultimo GroupDocs.Signature for .NET da [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
        
        // Set up input Pps file
        string filePath = "input.pps";
        // Set up output file
        string outputFilePath = "output.pps";

        // Instantiate Signature for input file
        using (var signature = new GroupDocs.Signature.Signature(filePath))
        {
                // instantiate metadata signing options
                var options = new MetadataSignOptions();

                // setup Author property
                PresentationMetadataSignature mdSign_Author = new PresentationMetadataSignature("Author", "Mr.Scherlock Holmes");// String value
                options.Signatures.Add(mdSign_Author);
                // setup document data
                PresentationMetadataSignature mdSign_DocData = new PresentationMetadataSignature("CreatedOn", DateTime.Now);// Datetime value
                options.Signatures.Add(mdSign_DocData);
                // setup document id
                PresentationMetadataSignature mdSign_DocId = new PresentationMetadataSignature("DocumentId", 123456);// Integer value
                options.Signatures.Add(mdSign_DocId);
                
                // sign Pps document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Firma di documenti Pps con Metadata Demo live"
    content: |
       Firma subito il file Pps con varie firme visitando il sito web [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Demo online gratuita ti aspetta.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Altre firme Metadata supportate per C#"
    content: |
        "Puoi anche firmare Pps con altri tipi di firma. Si prega di consultare l'elenco di seguito."
    format: 
       
       
back_to_top:
    enable: true
---