---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Search
signaturetype: Qrcode
fileformat: Doc
productName: .NET
lang: it
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Search Qrcode signatures at Doc with C#

############################# Head ############################
head_title: "Cerca le firme Qrcode nel file Doc in C#"
head_description: "Usa .NET per cercare le firme Qrcode nei file Doc utilizzando poche righe di codice."

############################# Header ############################
title: "Cerca le firme Qrcode nel file Doc"
description: "L'API nativa .NET consente di cercare firme Qrcode in file Doc già firmati. Esegui una ricerca avanzata di firme elettroniche all'interno dei tuoi documenti Doc utilizzando poche righe di codice."
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true

    left:
        img_alt: "GroupDocs.Signature for .NET"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocsature-net.png"
        product: "GroupDocs.Signature"
        platform: ".NET"



############################# About ############################
about:
    enable: true
    title: "Informazioni sull'API GroupDocs.Signature for .NET"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) fornisce l'API .NET per l'elaborazione di documenti utilizzando vari tipi di firma come testi, immagini, certificati digitali, codici a barre, codici QR, timbri o metadati. Gli utenti possono aggiungere, eliminare, aggiornare, verificare o cercare firme elettroniche all'interno di PDF, documenti MS Word, cartelle di lavoro MS Excel, presentazioni MS PowerPoint, file Adobe Photoshop e vari formati di immagine, con supporto aggiuntivo per la personalizzazione delle proprietà delle firme secondo necessità.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Come cercare le firme Qrcode in Doc"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) consente agli sviluppatori di .NET di cercare più facilmente le firme Qrcode nei file Doc dalle loro applicazioni implementando alcuni semplici passaggi.
        
        * Crea una nuova istanza della classe Signature e passa il percorso del documento di origine come parametro del costruttore.
        * Crea un'istanza dell'oggetto SearchOptions in base alle tue esigenze e specifica le opzioni di ricerca.
        * Chiama il metodo di ricerca dell'istanza della classe Signature e passa ad esso SearchOptions.
        * Elabora i risultati della ricerca in base alle tue richieste.

    title_right: "Requisiti di sistema"
    content_right: |
        GroupDocs.Signature for .NET sono supportati su tutte le principali piattaforme e sistemi operativi. Prima di eseguire il codice seguente, assicurati di avere i seguenti prerequisiti installati sul tuo sistema.

        * Sistemi operativi: Microsoft Windows, Linux, MacOS
        * Ambienti di sviluppo: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Scarica l'ultima versione di GroupDocs.Signature for .NET da [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Doc file
        string filePath = "input.doc";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                //Create search options
                QrCodeSearchOptions options = new QrCodeSearchOptions()
                {
                    // specify special pages to search on 
                    AllPages = false,
                    // single page number
                    PageNumber = 1,
                    // set up text match type
                    MatchType = TextMatchType.Contains,
                    // specify text pattern to search
                    Text = "Text signature",
                    // return  Qrcode images for processing
                    ReturnContent = true,
                    // set up type of returned  Qrcode images
                    ReturnContentType = FileType.PNG
                };

                // search for Qrcode signatures in Doc document
                List<QrCodeSignature> signatures = signature.Search<QrCodeSignature>(options);

                // process signatures which were found                
                foreach (QrCodeSignature item in signatures)
                {
                    //...
                }
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Cerca Qrcode firme elettroniche Demo live"
    content: |
       Cerca subito nel documento varie firme elettroniche nei file Doc visitando il sito Web [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).

        
############################# More Formats ############################
more_formats:
    enable: true
    title: "Cerca altre firme Qrcode utilizzando C#"
    content: |
        "Le firme elettroniche ricercano in vari documenti. Trova le firme da uno dei formati di file più diffusi come mostrato di seguito."
    format: 
           
       
back_to_top:
    enable: true
---