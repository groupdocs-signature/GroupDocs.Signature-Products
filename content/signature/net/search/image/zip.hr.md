---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Search
signaturetype: Image
fileformat: Zip
productName: .NET
lang: hr
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Search Image signatures at Zip with C#

############################# Head ############################
head_title: "Potražite Image potpise u datoteci Zip u C#"
head_description: "Upotrijebite .NET za traženje potpisa Image u datotekama Zip pomoću nekoliko redaka koda."

############################# Header ############################
title: "Potražite Image potpise u Zip datoteci"
description: "Izvorni API za .NET omogućuje pretraživanje potpisa Image u već potpisanim Zip datotekama. Izvršite napredno pretraživanje e-potpisa unutar svojih Zip dokumenata pomoću nekoliko redaka koda."
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
    title: "O GroupDocs.Signature for .NET API-ju"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) pruža .NET API za obradu dokumenata koji koriste različite vrste potpisa kao što su tekstovi, slike, digitalni certifikati, crtični kodovi, QR kodovi, pečati ili metapodaci. Korisnici mogu dodavati, brisati, ažurirati, verificirati ili pretraživati ​​elektroničke potpise unutar PDF-ova, MS Word dokumenata, MS Excel radnih knjiga, MS PowerPoint prezentacija, Adobe Photoshop datoteka i raznih formata slika, uz dodatnu podršku za prilagođavanje svojstava potpisa prema potrebi.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Kako tražiti Image potpise u Zip"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) programerima proizvoda .NET olakšava traženje potpisa Image u datotekama Zip iz njihovih aplikacija implementacijom nekoliko jednostavnih koraka.
        
        * Stvorite novu instancu klase Signature i proslijedite putanju izvornog dokumenta kao parametar konstruktora.
        * Instancirajte SearchOptions objekt prema svojim zahtjevima i odredite opcije pretraživanja.
        * Pozovite metodu Search instance klase Signature i proslijedite joj SearchOptions.
        * Obradite rezultate pretraživanja u skladu s vašim zahtjevima.

    title_right: "Zahtjevi sustava"
    content_right: |
        GroupDocs.Signature for .NET podržani su na svim glavnim platformama i operativnim sustavima. Prije izvršavanja koda u nastavku, provjerite imate li sljedeće preduvjete instalirane na vašem sustavu.

        * Operativni sustavi: Microsoft Windows, Linux, MacOS
        * Razvojna okruženja: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Preuzmite najnoviju verziju GroupDocs.Signature for .NET s [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Zip file
        string filePath = "input.zip";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                //Create search options
                ImageSearchOptions options = new ImageSearchOptions()
                {
                    // set minimum size if needed
                    MinContentSize = 100,
                    // set maximum image size if needed
                    MaxContentSize = 2000,                    
                    // return  Image images for processing
                    ReturnContent = true,
                    // set up type of returned  Image images
                    ReturnContentType = FileType.PNG                                 
                };

                // search for Image signatures in Zip document
                List<ImageSignature> signatures = signature.Search<ImageSignature>(options);

                // process signatures which were found                
                foreach (ImageSignature item in signatures)
                {
                    //...
                }
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Potražite Image elektroničke potpise Demo uživo"
    content: |
       Potražite u dokumentu različite elektroničke potpise za Zip datoteke upravo sada tako da posjetite [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) web mjesto.

        
############################# More Formats ############################
more_formats:
    enable: true
    title: "Potražite druge Image potpise koristeći C#"
    content: |
        "Pretraživanje elektroničkih potpisa u raznim dokumentima. Pronađite potpise jednog od popularnih formata datoteka kao što je prikazano u nastavku."
    format: 
           
       
back_to_top:
    enable: true
---