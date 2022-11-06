---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Digital
fileformat: Xlsb
productName: .NET
lang: it
productCode: net
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Xlsb for C#

############################# Head ############################
head_title: "Aggiunta di firme elettroniche digitali al file Xlsb con C#"
head_description: "Inserisci la firma digitale sul file Xlsb per .NET utilizzando poche righe di codice. Usa l'API per la firma dei documenti di GroupDocs per firmare decine di formati di file."

############################# Header ############################
title: "eSign file Xlsb con firme Digital in C#"
description: "Come aggiungere la firma Digital con poche righe di codice .NET"
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
    title: "Informazioni su GroupDocs.Signature for .NET API delle firme digitali"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) è un'API popolare per la firma di documenti con firme elettroniche digitali, con certificati digitali. Per le firme digitali API utilizza i file di certificato PFX per firmare documenti con chiavi private e pubbliche protette da password. Le firme digitali possono essere utilizzate per certificare documenti aziendali con una pagina particolare PDF eSign, certificare interi documenti di Microsoft Office come Word, Excel, file Powerpoint e documenti Open Office. I clienti possono facilmente manipolare le firme come modificarle, rimuoverle o modificarle. L'API fornisce un modo per cercare e verificare le firme. Inoltre, vengono fornite molte abilità per la personalizzazione delle firme.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Passaggi per firmare Xlsb con Digital in C#"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) offre la possibilità di firmare documenti Xlsb con firme Digital in modo rapido e semplice.
        
        * Crea un'istanza della classe Signature che fornisce il file Xlsb che dovrebbe firmare come percorso o flusso di memoria
        * Crea un'istanza della classe SignOptions e imposta tutti i dati richiesti.
        * Richiama il metodo Signature.Sign() passando il file di output Xlsb o il flusso di memoria

    title_right: " Requisiti di sistema"
    content_right: |
        GroupDocs.Signature for .NET sono supportati su tutte le principali piattaforme e sistemi operativi. Prima di eseguire il codice seguente, assicurati di avere i seguenti prerequisiti installati sul tuo sistema.

        * Sistemi operativi: Microsoft Windows, Linux, MacOS
        * Ambienti di sviluppo: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Ricevi l'ultimo GroupDocs.Signature for .NET da [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Xlsb file
        string filePath = "input.xlsb";
        // Set up output file
        string outputFilePath = "output.xlsb";
        // Provide digital certificate
        string certificateFilePath = "certificate.pfx";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                //Provide sign options
                DigitalSignOptions options = new DigitalSignOptions(certificateFilePath)
                {
                    // set certificate password
                    Password = "1234567890",
                    // set signature position
                    Left = 50,
                    Top = 200,
                };

                // sign Xlsb document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Firma di documenti Xlsb con Digital Demo live"
    content: |
       Firma subito il file Xlsb con varie firme visitando il sito web [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Demo online gratuita ti aspetta.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Altre firme Digital supportate per C#"
    content: |
        "Puoi anche firmare Xlsb con altri tipi di firma. Si prega di consultare l'elenco di seguito."
    format: 
       
       
back_to_top:
    enable: true
---