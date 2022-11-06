---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Verify
signaturetype: Digital
fileformat: Xlsb
productName: .NET
lang: it
productCode: net
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Xlsb for C#

############################# Head ############################
head_title: "Verifica delle firme Digital per i file Xlsb tramite C#"
head_description: "Utilizza solo poche righe di codice .NET per verificare i documenti Xlsb e le relative firme Digital."

############################# Header ############################
title: "Verifica delle firme Digital per i file Xlsb"
description: "L'API per .NET offre l'opportunità di verificare le firme Digital nei documenti Xlsb. La verifica delle firme elettroniche all'interno dei tuoi documenti Xlsb potrebbe essere eseguita in modo rapido e semplice."
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
    title_left: "Come convalidare le firme Digital nel tuo documento Xlsb"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) include funzioni utili come la verifica delle firme Digital apposte in Xlsb documenti. Usa questa opportunità senza implementare codice aggiuntivo.
        
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
                
        // Set up input Xlsb file
        string filePath = "input.xlsb";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                //Provide verification options
                DigitalVerifyOptions options = new DigitalVerifyOptions()
                {
                    // Digital signature comment
                    Comments = "Approved by co-owner",
                    // specify period of signatures
                    SignDateTimeFrom = new DateTime(year: 2021, month: 01, day: 01),
                    SignDateTimeTo = new DateTime(year: 2022, month: 12, day: 31)
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
    title: "Firma con Digital firme Demo live"
    content: |
       Aggiungi subito varie firme elettroniche al file Xlsb visitando il sito Web [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Verifica altre firme Digital utilizzando C#"
    content: |
        "Verifica delle firme elettroniche apposte nei vari documenti. Controlla la qualità delle firme nei formati di file più diffusi come mostrato di seguito."
    format: 
       
       
back_to_top:
    enable: true
---