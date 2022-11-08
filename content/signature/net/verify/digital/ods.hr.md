---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Verify
signaturetype: Digital
fileformat: Ods
productName: .NET
lang: hr
productCode: net
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Ods for C#

############################# Head ############################
head_title: "Provjera Digital potpisa za Ods datoteke putem C#"
head_description: "Upotrijebite samo nekoliko redaka .NET koda za provjeru Ods dokumenata i njihovih Digital potpisa."

############################# Header ############################
title: "Provjera potpisa Digital za Ods datoteke"
description: "API za .NET pruža priliku za provjeru potpisa Digital u dokumentima Ods. Provjera e-potpisa unutar vaših Ods dokumenata može se izvršiti brzo i jednostavno."
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
    title: "Otkrijte nove GroupDocs.Signature for .NET API značajke"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) API pruža širok raspon načina za obradu brojnih formata dokumenata korištenjem elektroničkih potpisa. Podržane su mnoge vrste digitalnih potpisa kao što su tekstovi, slike, digitalni certifikati, crtični kodovi, QR kodovi, pečati ili metapodaci. Korisnici mogu dodavati, uklanjati, uređivati, potvrđivati ​​ili pretraživati ​​digitalne potpise u PDF-ovima, MS Word dokumentima, MS Excel radnim knjigama, MS PowerPoint prezentacijama, Adobe Photoshop datotekama i raznim formatima slika. Dostupan je nevjerojatan broj dodatnih značajki i postavki.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Kako provjeriti valjanost potpisa Digital u vašem Ods dokumentu"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) uključuje korisne značajke kao što je provjera potpisa Digital postavljenih na dokumente Ods. Iskoristite ovu priliku bez implementacije dodatnog koda.
        
        * Prvo, instancirajte klasu potpisa koja kao parametar konstruktora daje put do dokumenta koji bi trebao biti verificiran.
        * Drugo, stvorite novi objekt VerifyOptions i postavite sva potrebna svojstva.
        * Na kraju, pozovite metodu Verify objekta Signature prolazeći instancu VerifyOptions.
        * Zatim obradite rezultate provjere.

    title_right: "Zahtjevi sustava"
    content_right: |
        GroupDocs.Signature for .NET podržani su na svim glavnim platformama i operativnim sustavima. Prije izvršavanja koda u nastavku, provjerite imate li sljedeće preduvjete instalirane na vašem sustavu.

        * Operativni sustavi: Microsoft Windows, Linux, MacOS
        * Razvojna okruženja: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Preuzmite najnoviju verziju GroupDocs.Signature for .NET s [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Ods file
        string filePath = "input.ods";

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
    title: "Potpisivanje s Digital potpisima Demo uživo"
    content: |
       Odmah dodajte različite elektroničke potpise u datoteku Ods tako da posjetite [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) web mjesto.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Provjerite druge Digital potpise koristeći C#"
    content: |
        "Provjera elektroničkih potpisa postavljenih u različite dokumente. Provjerite kvalitetu potpisa u popularnim formatima datoteka kao što je otkriveno u nastavku."
    format: 
       
       
back_to_top:
    enable: true
---