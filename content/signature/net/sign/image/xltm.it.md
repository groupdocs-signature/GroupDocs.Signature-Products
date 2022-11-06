---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Image
fileformat: Xltm
productName: .NET
lang: it
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Image signature on Xltm for C#

############################# Head ############################
head_title: "Aggiunta di firme Image al file Xltm con C#"
head_description: "Inserisci Image Firma sul file Xltm per .NET utilizzando poche righe di codice. Usa l'API per la firma dei documenti di GroupDocs per firmare decine di formati di file."

############################# Header ############################
title: "Firma file Xltm con firme Image in C#"
description: "Come aggiungere la firma Image con poche righe di codice .NET"
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
    title: "Informazioni su GroupDocs.Signature for .NET API delle firme di immagini"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) è un'API popolare per la firma elettronica di documenti digitali. Sono disponibili firme come testi, immagini, certificati digitali, codici a barre, codici QR, timbri o metadati. Le firme possono essere posizionate su PDF, documenti MS Word, cartelle di lavoro MS Excel, presentazioni MS PowerPoint, file Adobe Photoshop e vari formati di immagine. I clienti possono firmare il proprio documento e aggiornare, cercare, verificare, eliminare o visualizzare in anteprima le firme elettroniche che sono state apposte su tali documenti. Inoltre, vengono fornite molte abilità per la personalizzazione delle firme.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Passaggi per firmare Xltm con Image in C#"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) offre la possibilità di firmare documenti Xltm con firme Image in modo rapido e semplice.
        
        * Crea un'istanza della classe Signature che fornisce il file Xltm che dovrebbe firmare come percorso o flusso di memoria
        * Crea un'istanza della classe SignOptions e imposta tutti i dati richiesti.
        * Richiama il metodo Signature.Sign() passando il file di output Xltm o il flusso di memoria

    title_right: " Requisiti di sistema"
    content_right: |
        GroupDocs.Signature for .NET sono supportati su tutte le principali piattaforme e sistemi operativi. Prima di eseguire il codice seguente, assicurati di avere i seguenti prerequisiti installati sul tuo sistema.

        * Sistemi operativi: Microsoft Windows, Linux, MacOS
        * Ambienti di sviluppo: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Ricevi l'ultimo GroupDocs.Signature for .NET da [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Xltm file
        string filePath = "input.xltm";
        // Set up output file
        string outputFilePath = "output.xltm";
        // Provide image file
        string imageFilePath = "image.png";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
            //Provide sign options
            ImageSignOptions options = new ImageSignOptions(imageFilePath)
            {
                // set signature position
                Left = 50,
                Top = 200
            };

            // sign Xltm document
            SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Firma di documenti Xltm con Image Demo live"
    content: |
       Firma subito il file Xltm con varie firme visitando il sito web [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Demo online gratuita ti aspetta.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Altre firme Image supportate per C#"
    content: |
        "Puoi anche firmare Xltm con altri tipi di firma. Si prega di consultare l'elenco di seguito."
    format: 
       
       
back_to_top:
    enable: true
---