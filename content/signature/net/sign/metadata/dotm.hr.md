---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Metadata
fileformat: Dotm
productName: .NET
lang: hr
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Metadata signature on Dotm for C#

############################# Head ############################
head_title: "Dodajte elektroničke potpise metapodataka Dotm dokumentima putem C#"
head_description: "Koristite metapodatke kao skrivene elektroničke potpise unutar svojih Dotm dokumenata pomoću nekoliko redaka C# koda. Upotrijebite GroupDocs Document Signature API za e-potpisivanje vaših poslovnih dokumenata i datoteka s informacijama o metapodacima."

############################# Header ############################
title: "Elektronički potpisi metapodataka za Dotm dokument putem .NET jednostavni su i laki za korištenje!"
description: "ePotpišite svoje Dotm dokumente i ugovore sa skrivenim unosima metapodataka. Generirajte metapodatke za PDF-ove, MS Word dokumente, MS Excel radne knjige, MS PowerPoint prezentacije i razne formate slika bez problema i dodatnog kodiranja."
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
    title: "O API-ju za potpise metapodataka GroupDocs.Signature for .NET"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) je popularan API za e-potpisivanje digitalnih dokumenata. Dostupni su potpisi kao što su tekstovi, slike, digitalni certifikati, crtični kodovi, QR kodovi, pečati ili metapodaci. Potpisi se mogu staviti na PDF-ove, MS Word dokumente, MS Excel radne knjige, MS PowerPoint prezentacije, Adobe Photoshop datoteke i razne formate slika. Korisnici mogu potpisati svoj dokument i ažurirati, pretraživati, verificirati, brisati ili pregledavati e-potpise koji su stavljeni na te dokumente. Štoviše, pruža se mnogo mogućnosti za prilagodbu potpisa.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Koraci za potpisivanje Dotm s Metadata u C#"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) pruža mogućnost brzog i jednostavnog potpisivanja Dotm dokumenata s Metadata potpisima.
        
        * Stvorite instancu klase potpisa koja daje Dotm datoteku koja bi se trebala potpisati kao put ili memorijski tok
        * Instancirajte klasu SignOptions i postavite sve tražene podatke.
        * Pozovite metodu Signature.Sign() prosljeđujući izlaznu datoteku Dotm ili memorijski tok

    title_right: " Zahtjevi sustava"
    content_right: |
        GroupDocs.Signature for .NET podržani su na svim glavnim platformama i operativnim sustavima. Prije izvršavanja koda u nastavku, provjerite imate li sljedeće preduvjete instalirane na vašem sustavu.

        * Operativni sustavi: Microsoft Windows, Linux, MacOS
        * Razvojna okruženja: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Preuzmite najnoviji GroupDocs.Signature for .NET od [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
        
        // Set up input Dotm file
        string filePath = "input.dotm";
        // Set up output file
        string outputFilePath = "output.dotm";

        // Instantiate Signature for input file
        using (var signature = new GroupDocs.Signature.Signature(filePath))
        {
                // instantiate metadata signing options
                var options = new MetadataSignOptions();

                // setup Author property
                WordProcessingMetadataSignature mdSign_Author = new WordProcessingMetadataSignature("Author", "Mr.Scherlock Holmes");// String value
                options.Signatures.Add(mdSign_Author);
                // setup document data
                WordProcessingMetadataSignature mdSign_DocData = new WordProcessingMetadataSignature("CreatedOn", DateTime.Now);// Datetime value
                options.Signatures.Add(mdSign_DocData);
                // setup document id
                WordProcessingMetadataSignature mdSign_DocId = new WordProcessingMetadataSignature("DocumentId", 123456);// Integer value
                options.Signatures.Add(mdSign_DocId);
                
                // sign Dotm document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Potpisivanje Dotm dokumenata s Metadata Live Demo"
    content: |
       Potpišite datoteku Dotm raznim potpisima upravo sada tako da posjetite [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) web mjesto. Besplatan online demo čeka na vas.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Drugi podržani potpisi Metadata za C#"
    content: |
        "Također možete potpisati Dotm drugim vrstama potpisa. Pogledajte popis u nastavku."
    format: 
       
       
back_to_top:
    enable: true
---