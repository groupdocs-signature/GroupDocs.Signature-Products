---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Search
signaturetype: Barcode
fileformat: Tar
productName: .NET
lang: ro
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Search Barcode signatures at Tar with C#

############################# Head ############################
head_title: "Căutați semnături Barcode în fișierul Tar în C#"
head_description: "Utilizați .NET pentru a căuta semnături Barcode în fișiere Tar folosind câteva rânduri de cod."

############################# Header ############################
title: "Căutați semnături Barcode în fișierul Tar"
description: "API-ul nativ .NET permite căutarea semnăturilor Barcode în fișierele Tar deja semnate. Efectuați o căutare avansată de semnătură electronică în documentele dvs. Tar folosind câteva rânduri de cod."
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
    title: "Despre GroupDocs.Signature for .NET API"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) oferă .NET API pentru procesarea documentelor folosind diferite tipuri de semnături, cum ar fi texte, imagini, certificate digitale, coduri de bare, coduri QR, ștampile sau metadate. Utilizatorii pot adăuga, șterge, actualiza, verifica sau căuta semnături electronice în PDF-uri, documente MS Word, registre de lucru MS Excel, prezentări MS PowerPoint, fișiere Adobe Photoshop și diferite formate de imagine, cu suport suplimentar pentru personalizarea proprietăților semnăturilor după cum este necesar.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Cum să căutați semnături Barcode în Tar"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) facilitează pentru dezvoltatorii .NET să caute semnături Barcode în fișierele Tar din aplicațiile lor prin implementarea câțiva pași simpli.
        
        * Creați o nouă instanță a clasei Signature și treceți calea documentului sursă ca parametru de constructor.
        * Instanciați obiectul SearchOptions în funcție de cerințele dvs. și specificați opțiunile de căutare.
        * Apelați metoda Search a instanței clasei Signature și transmiteți-i SearchOptions.
        * Procesați rezultatele căutării în funcție de cerințele dvs.

    title_right: "Cerințe de sistem"
    content_right: |
        GroupDocs.Signature for .NET sunt acceptate pe toate platformele și sistemele de operare majore. Înainte de a executa codul de mai jos, vă rugăm să vă asigurați că aveți următoarele cerințe preliminare instalate pe sistemul dumneavoastră.

        * Sisteme de operare: Microsoft Windows, Linux, MacOS
        * Medii de dezvoltare: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Descărcați cea mai recentă versiune a GroupDocs.Signature for .NET de la [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
        
        // Set up input Tar file
        string filePath = "input.tar";

        // Instantiate Signature for input file
        using (var signature = new GroupDocs.Signature.Signature(filePath))
        {
                //Create search options
                BarcodeSearchOptions options = new BarcodeSearchOptions()
                {
                    // specify special pages to search on 
                    AllPages = false,
                    // single page number
                    PageNumber = 1,
                    // set up text match type
                    MatchType = TextMatchType.Contains,
                    // specify text pattern to search
                    Text = "Text signature",
                    // return  Barcode images for processing
                    ReturnContent = true,
                    // set up type of returned  Barcode images
                    ReturnContentType = FileType.PNG
                };

                // search for Barcode signatures in Tar document
                List<BarcodeSignature> signatures = signature.Search<BarcodeSignature>(options);

                // process signatures which were found                
                foreach (BarcodeSignature item in signatures)
                {
                    //...
                }
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Căutați Barcode semnături electronice Live Demo"
    content: |
       Căutați în document diferite semnături electronice în fișiere Tar chiar acum, vizitând site-ul web [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).

        
############################# More Formats ############################
more_formats:
    enable: true
    title: "Căutați alte semnături Barcode folosind C#"
    content: |
        "Căutare de semnături electronice în diverse documente. Găsiți semnături din unul dintre formatele de fișiere populare, așa cum se arată mai jos."
    format: 
           
       
back_to_top:
    enable: true
---