---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Update
signaturetype: Text
fileformat: Ods
productName: .NET
lang: it
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Text signature on Ods for C#

############################# Head ############################
head_title: "Aggiorna le firme Text inserite nei file Ods con C#"
head_description: "Utilizza il codice .NET semplice e facile per l'aggiornamento delle firme Text nei documenti Ods firmati."

############################# Header ############################
title: "Modifica e aggiorna le firme Text inserite nei file Ods"
description: "L'API per .NET fornisce funzionalità per l'aggiornamento delle firme Text nei documenti Ods. Aggiorna le firme elettroniche all'interno dei tuoi documenti Ods con un paio di righe di codice C# in modo rapido e semplice."
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
    title: "Ulteriori informazioni sulle funzionalità dell'API GroupDocs.Signature for .NET"
    content: |
        La funzionalità dell'API [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) contiene un'ampia selezione di mezzi per elaborare i formati di documenti richiesti utilizzando le firme elettroniche. È supportato un ampio spettro di firme elettroniche come testi, immagini, certificati digitali, codici a barre, codici QR, timbri o metadati. I clienti possono aggiungere, rimuovere, modificare, convalidare o cercare firme digitali in PDF, documenti MS Word, cartelle di lavoro MS Excel, presentazioni MS PowerPoint, file Adobe Photoshop e vari formati di immagine. Sono disponibili numerose funzioni e impostazioni utili.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Come modificare le firme Text nel tuo documento Ods"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) include funzioni utili come l'aggiornamento di firme Text apposte in documenti Ods. Consente di modificare le caratteristiche delle firme senza codice aggiuntivo.
        
        * Per cominciare, crea l'oggetto Signature passando come percorso del parametro del costruttore a un documento che dovrebbe essere aggiornato.
        * Quindi, crea un'istanza di un particolare oggetto di firma appropriato e imposta il suo identificatore e le proprietà che devono essere modificate.
        * Infine, chiama il metodo di aggiornamento della firma passando un particolare oggetto di firma.
        * Elabora i risultati dell'aggiornamento a tuo avviso.

    title_right: "Requisiti di sistema"
    content_right: |
        GroupDocs.Signature for .NET sono supportati su tutte le principali piattaforme e sistemi operativi. Prima di eseguire il codice seguente, assicurati di avere i seguenti prerequisiti installati sul tuo sistema.

        * Sistemi operativi: Microsoft Windows, Linux, MacOS
        * Ambienti di sviluppo: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Scarica l'ultima versione di GroupDocs.Signature for .NET da [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Ods file
        string filePath = "input.ods";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                // Id of signature which is supposed to be updated
                // such Id might be got as a result of search operation
                string id = "ff988ab1-7403-4c8d-8db7-f2a56b9f8530";

                // provide signature features to update
                // set up particular signature id
                TextSignature signatureToUpdate = new TextSignature(id)
                {
                    // specify signature width
                    Width = 130,
                    // specify signature height
                    Height = 20,
                    // set left position
                    Left = 40,
                    // set top position
                    Top = 50,
                    // set up new text
                    Text = "Mr. John Smith"
                };

                // update signature
                bool updateResult = signature.Update(signatureToUpdate);

                // process updation result
                if (updateResult)
                {
                    Console.WriteLine("Signature was updated successfully!");
                }
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Aggiornamento delle firme Text nelle pagine del documento - Demo dal vivo"
    content: |
       Modifica subito diverse firme elettroniche del documento Ods visitando il sito Web [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Aggiorna varie firme Text tramite C#"
    content: |
        "Modifica delle firme digitali che vengono inserite in vari formati di documenti. Aggiorna i dati delle firme senza codice aggiuntivo."
    format: 
       
       
back_to_top:
    enable: true
---