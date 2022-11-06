---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Barcode
codetype: Pharmacode
fileformat: Dotx
productName: .NET
lang: it
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put  Barcode signature on Dotx for C#

############################# Head ############################
head_title: "eSign Dotx documento con codice a barre Pharmacode in C#"
head_description: "Crea Pharmacode Firma codice a barre e inseriscilo nel documento Dotx con .NET utilizzando un paio di righe di codice. Utilizza l'API per la firma dei documenti di GroupDocs per firmare vari formati di file."

############################# Header ############################
title: "Genera Pharmacode firma del codice a barre per il documento Dotx in C#"
description: "Firma elettronicamente i tuoi documenti aziendali Dotx con il codice a barre Pharmacode. Genera la firma del codice a barre in modo rapido e semplice con poche righe di codice per impostare le opzioni di firma."
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
    title_left: "Passaggi per firmare Dotx con Barcode in C#"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) offre la possibilità di firmare documenti Dotx con firme Barcode in modo rapido e semplice.
        
        * Crea un'istanza della classe Signature che fornisce il file Dotx che dovrebbe firmare come percorso o flusso di memoria
        * Crea un'istanza della classe SignOptions e imposta tutti i dati richiesti.
        * Richiama il metodo Signature.Sign() passando il file di output Dotx o il flusso di memoria

    title_right: " Requisiti di sistema"
    content_right: |
        GroupDocs.Signature for .NET sono supportati su tutte le principali piattaforme e sistemi operativi. Prima di eseguire il codice seguente, assicurati di avere i seguenti prerequisiti installati sul tuo sistema.

        * Sistemi operativi: Microsoft Windows, Linux, MacOS
        * Ambienti di sviluppo: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Ricevi l'ultimo GroupDocs.Signature for .NET da [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
        
        // Set up input Dotx file
        string filePath = "input.dotx";
        // Set up output file
        string outputFilePath = "output.dotx";

        // Instantiate Signature for input file
        using (var signature = new GroupDocs.Signature.Signature(filePath))
        {
                // create barcode option with predefined barcode text
                var options = new BarcodeSignOptions("BC12345678")
                {
                    // setup Barcode encoding type
                    EncodeType = BarcodeTypes.Pharmacode,

                    // set signature position
                    Left = 50,
                    Top = 50,
                    Width = 200,
                    Height = 50                                        
                };
                
                // sign Dotx document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Firma di documenti Dotx con Barcode Demo live"
    content: |
       Firma subito il file Dotx con varie firme visitando il sito web [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Demo online gratuita ti aspetta.

        
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-barcode"
          title: "About Pharmacode Barcode"
          content: |
            Pharmacode, noto anche come Pharmaceutical Binary Code, è uno standard di codici a barre, utilizzato nell'industria farmaceutica come sistema di controllo dell'imballaggio.
          characterset: |
             Cifre numeriche (0-9).
          textcapacity: |
             Rappresenta un solo numero intero compreso tra 3 e 131070.
          image: |
             iVBORw0KGgoAAAANSUhEUgAAAIEAAAAkCAYAAACucVkNAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsMAAA7DAcdvqGQAAAIQSURBVHhe7dIxigQxEATB/f+n91RuUH2GEMhYBaRTasaaz/f5ee8neN5P8Lyf4FneT/C8n+B5P8Gz/PsTfD6fmtpNUrtJOr2bdnfT7d0m88vSPpTUbpLaTdLp3bS7m27vNplflvahpHaT1G6STu+m3d10e7fJ/LK0DyW1m6R2k3R6N+3uptu7TeaXpX0oqd0ktZuk07tpdzfd3m0yvyztQ0ntJqndJJ3eTbu76fZuk/llaR9KajdJ7Sbp9G7a3U23d5vML0v7UFK7SWo3Sad30+5uur3bZH5Z2oeS2k1Su0k6vZt2d9Pt3Sbzy9I+lNRuktpN0undtLubbu82mV+W9qGkdpPUbpJO76bd3XR7t8n8srQPJbWbpHaTdHo37e6m27tN5pelfSip3SS1m6TTu2l3N93ebTK/LO1DSe0mqd0knd5Nu7vp9m6T+WVpH0pqN0ntJun0btrdTbd3m8wvS/tQUrtJajdJp3fT7m66vdtkflnah5LaTVK7STq9m3Z30+3dJvPL0j6U1G6S2k3S6d20u5tu7zaZX5b2oaR2k9Rukk7vpt3ddHu3yfyytA8ltZukdpN0ejft7qbbu03ml6V9KKndJLWbpNO7aXc33d5tMr8s7UNJ7Sap3SSd3k27u+n2bpP5ZWkfSmo3Se0m6fRu2t1Nt3ebzC/Pz3g/wfN+guf9BM/yfoLn/QTP9/sHDRdB4BliyZUAAAAASUVORK5CYII=

          link: ""

############################# More Formats ############################
more_formats:
    enable: true
    title: "Altre firme Barcode supportate per C#"
    content: |
        "Puoi anche firmare Dotx con altri tipi di firma. Si prega di consultare l'elenco di seguito."
    format: 
        
       
back_to_top:
    enable: true
---