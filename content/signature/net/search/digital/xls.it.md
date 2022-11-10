---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Search
signaturetype: Digital
fileformat: Xls
productName: .NET
lang: it
productCode: net
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Search Digital signatures at Xls with C#

############################# Head ############################
head_title: "Cerca le firme Digital nel file Xls in C#"
head_description: "Usa .NET per cercare le firme Digital nei file Xls utilizzando poche righe di codice."

############################# Header ############################
title: "Cerca le firme Digital nel file Xls"
description: "L'API nativa .NET consente di cercare firme Digital in file Xls già firmati. Esegui una ricerca avanzata di firme elettroniche all'interno dei tuoi documenti Xls utilizzando poche righe di codice."
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
    title_left: "Come cercare le firme Digital in Xls"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) consente agli sviluppatori di .NET di cercare più facilmente le firme Digital nei file Xls dalle loro applicazioni implementando alcuni semplici passaggi.
        
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
                
        // Set up input Xls file
        string filePath = "input.xls";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                //Create search options
                DigitalSearchOptions options = new DigitalSearchOptions()
                {
                    // specify special search criteria
                    Comments = "Approved",
                    // specify date range period of signature
                    SignDateTimeFrom = new DateTime(year: 2020, month: 01, day: 01),
                    SignDateTimeTo = new DateTime(year: 2020, month: 12, day: 31)
                };

                // search for Digital signatures in Xls document
                List<DigitalSignature> signatures = signature.Search<DigitalSignature>(options);

                // process signatures which were found                
                foreach (DigitalSignature item in signatures)
                {
                    //...
                }
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Cerca Digital firme elettroniche Demo live"
    content: |
       Cerca subito nel documento varie firme elettroniche nei file Xls visitando il sito Web [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).

        
############################# More Formats ############################
more_formats:
    enable: true
    title: "Cerca altre firme Digital utilizzando C#"
    content: |
        "Le firme elettroniche ricercano in vari documenti. Trova le firme da uno dei formati di file più diffusi come mostrato di seguito."
    format: 
           
       
back_to_top:
    enable: true
---