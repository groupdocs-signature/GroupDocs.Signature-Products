---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Search
signaturetype: Digital
fileformat: Pptm
productName: .NET
lang: ro
productCode: net
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Search Digital signatures at Pptm with C#

############################# Head ############################
head_title: "Căutați semnături Digital în fișierul Pptm în C#"
head_description: "Utilizați .NET pentru a căuta semnături Digital în fișiere Pptm folosind câteva rânduri de cod."

############################# Header ############################
title: "Căutați semnături Digital în fișierul Pptm"
description: "API-ul nativ .NET permite căutarea semnăturilor Digital în fișierele Pptm deja semnate. Efectuați o căutare avansată de semnătură electronică în documentele dvs. Pptm folosind câteva rânduri de cod."
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
    title_left: "Cum să căutați semnături Digital în Pptm"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) facilitează pentru dezvoltatorii .NET să caute semnături Digital în fișierele Pptm din aplicațiile lor prin implementarea câțiva pași simpli.
        
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
                
        // Set up input Pptm file
        string filePath = "input.pptm";

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

                // search for Digital signatures in Pptm document
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
    title: "Căutați Digital semnături electronice Live Demo"
    content: |
       Căutați în document diferite semnături electronice în fișiere Pptm chiar acum, vizitând site-ul web [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).

        
############################# More Formats ############################
more_formats:
    enable: true
    title: "Căutați alte semnături Digital folosind C#"
    content: |
        "Căutare de semnături electronice în diverse documente. Găsiți semnături din unul dintre formatele de fișiere populare, așa cum se arată mai jos."
    format: 
           
       
back_to_top:
    enable: true
---