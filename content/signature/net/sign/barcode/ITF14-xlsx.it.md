---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Barcode
codetype: I T F14
fileformat: Xlsx
productName: .NET
lang: it
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put  Barcode signature on Xlsx for C#

############################# Head ############################
head_title: "eSign Xlsx documento con codice a barre I T F14 in C#"
head_description: "Crea I T F14 Firma codice a barre e inseriscilo nel documento Xlsx con .NET utilizzando un paio di righe di codice. Utilizza l'API per la firma dei documenti di GroupDocs per firmare vari formati di file."

############################# Header ############################
title: "Genera I T F14 firma del codice a barre per il documento Xlsx in C#"
description: "Firma elettronicamente i tuoi documenti aziendali Xlsx con il codice a barre I T F14. Genera la firma del codice a barre in modo rapido e semplice con poche righe di codice per impostare le opzioni di firma."
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
    title: "Informazioni su GroupDocs.Signature for .NET API delle firme di codici a barre."
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) è un'API semplice e veloce per gestire la firma elettronica dei documenti digitali utilizzando tipi di codici a barre come UPCA, UPCE, EAN13, EAN14, Code39, Code39Extended, Code128, Codabar, Postnet, ISBN , ITF14 e molti altri. I clienti possono creare facilmente codici a barre fornendo il testo richiesto e inserirli in PDF, documenti Microsoft Office Words, cartelle di lavoro Microsoft Office Excel, presentazioni MS PowerPoint, file Adobe Photoshop e vari formati di immagine. I codici a barre inseriti nei documenti possono essere aggiornati, ricercati, verificati, eliminati o visualizzati in anteprima. Inoltre, è supportata la personalizzazione dei codici a barre.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Passaggi per firmare Xlsx con Barcode in C#"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) offre la possibilità di firmare documenti Xlsx con firme Barcode in modo rapido e semplice.
        
        * Crea un'istanza della classe Signature che fornisce il file Xlsx che dovrebbe firmare come percorso o flusso di memoria
        * Crea un'istanza della classe SignOptions e imposta tutti i dati richiesti.
        * Richiama il metodo Signature.Sign() passando il file di output Xlsx o il flusso di memoria

    title_right: " Requisiti di sistema"
    content_right: |
        GroupDocs.Signature for .NET sono supportati su tutte le principali piattaforme e sistemi operativi. Prima di eseguire il codice seguente, assicurati di avere i seguenti prerequisiti installati sul tuo sistema.

        * Sistemi operativi: Microsoft Windows, Linux, MacOS
        * Ambienti di sviluppo: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Ricevi l'ultimo GroupDocs.Signature for .NET da [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
        
        // Set up input Xlsx file
        string filePath = "input.xlsx";
        // Set up output file
        string outputFilePath = "output.xlsx";

        // Instantiate Signature for input file
        using (var signature = new GroupDocs.Signature.Signature(filePath))
        {
                // create barcode option with predefined barcode text
                var options = new BarcodeSignOptions("BC12345678")
                {
                    // setup Barcode encoding type
                    EncodeType = BarcodeTypes.I T F14,

                    // set signature position
                    Left = 50,
                    Top = 50,
                    Width = 200,
                    Height = 50                                        
                };
                
                // sign Xlsx document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Firma di documenti Xlsx con Barcode Demo live"
    content: |
       Firma subito il file Xlsx con varie firme visitando il sito web [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Demo online gratuita ti aspetta.

        
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-barcode"
          title: "About I T F14 Barcode"
          content: |
            ITF-14 è l'implementazione GS1 di un codice a barre Interleaved 2 of 5 (ITF) per codificare un numero di articolo commerciale globale.
          characterset: |
             Cifre numeriche (0-9).
          textcapacity: |
             13 cifre + 1 cifra di controllo.
          image: |
             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

          link: ""

############################# More Formats ############################
more_formats:
    enable: true
    title: "Altre firme Barcode supportate per C#"
    content: |
        "Puoi anche firmare Xlsx con altri tipi di firma. Si prega di consultare l'elenco di seguito."
    format: 
        
       
back_to_top:
    enable: true
---