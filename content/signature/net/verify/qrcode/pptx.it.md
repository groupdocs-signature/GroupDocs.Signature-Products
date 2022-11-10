---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Verify
signaturetype: Qrcode
fileformat: Pptx
productName: .NET
lang: it
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Qrcode signature on Pptx for C#

############################# Head ############################
head_title: "Verifica delle firme Qrcode per i file Pptx tramite C#"
head_description: "Utilizza solo poche righe di codice .NET per verificare i documenti Pptx e le relative firme Qrcode."

############################# Header ############################
title: "Verifica delle firme Qrcode per i file Pptx"
description: "L'API per .NET offre l'opportunità di verificare le firme Qrcode nei documenti Pptx. La verifica delle firme elettroniche all'interno dei tuoi documenti Pptx potrebbe essere eseguita in modo rapido e semplice."
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
    title: "Scopri le nuove funzionalità dell'API GroupDocs.Signature for .NET"
    content: |
        L'API [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) offre un'ampia gamma di modi per elaborare numerosi formati di documenti utilizzando le firme elettroniche. Sono supportati molti tipi di firme digitali come testi, immagini, certificati digitali, codici a barre, codici QR, timbri o metadati. I clienti possono aggiungere, rimuovere, modificare, convalidare o cercare firme digitali in PDF, documenti MS Word, cartelle di lavoro MS Excel, presentazioni MS PowerPoint, file Adobe Photoshop e vari formati di immagine. È disponibile un numero sorprendente di funzioni e impostazioni aggiuntive.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Come convalidare le firme Qrcode nel tuo documento Pptx"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) include funzioni utili come la verifica delle firme Qrcode apposte in Pptx documenti. Usa questa opportunità senza implementare codice aggiuntivo.
        
        * In primo luogo, istanziare la classe Signature fornendo come parametro del costruttore il percorso di un documento che dovrebbe essere verificato.
        * In secondo luogo, crea un nuovo oggetto VerifyOptions e imposta tutte le proprietà richieste.
        * Infine, richiama il metodo Verify dell'oggetto di Signature passando l'istanza di VerifyOptions.
        * Quindi elaborare i risultati della verifica.

    title_right: "Requisiti di sistema"
    content_right: |
        GroupDocs.Signature for .NET sono supportati su tutte le principali piattaforme e sistemi operativi. Prima di eseguire il codice seguente, assicurati di avere i seguenti prerequisiti installati sul tuo sistema.

        * Sistemi operativi: Microsoft Windows, Linux, MacOS
        * Ambienti di sviluppo: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Scarica l'ultima versione di GroupDocs.Signature for .NET da [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Pptx file
        string filePath = "input.pptx";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                //Provide verification options
                QrCodeVerifyOptions options = new QrCodeVerifyOptions()
                {
                    // process only first page
                    PagesSetup = new PagesSetup() { FirstPage = true },
                    AllPages = false,
                    // set up text match type
                    MatchType = TextMatchType.StartsWith,
                    // specify text pattern to search
                    Text = "QrCode text",
                };

                // Verify document signatures
                VerificationResult result = signature.Verify(options);

                //process result
                if (result.IsValid)
                {
                    //..
                }
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Firma con Qrcode firme Demo live"
    content: |
       Aggiungi subito varie firme elettroniche al file Pptx visitando il sito Web [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Verifica altre firme Qrcode utilizzando C#"
    content: |
        "Verifica delle firme elettroniche apposte nei vari documenti. Controlla la qualità delle firme nei formati di file più diffusi come mostrato di seguito."
    format: 
       
       
back_to_top:
    enable: true
---