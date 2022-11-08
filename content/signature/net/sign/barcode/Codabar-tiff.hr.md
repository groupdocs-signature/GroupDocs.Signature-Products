---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Barcode
codetype: Codabar
fileformat: Tiff
productName: .NET
lang: hr
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put  Barcode signature on Tiff for C#

############################# Head ############################
head_title: "eSign Tiff dokument s Codabar crtičnim kodom u C#"
head_description: "Stvorite Codabar potpis crtičnog koda i stavite ga na Tiff dokument s .NET pomoću nekoliko redaka koda. Koristite GroupDocs Document Signature API za potpisivanje različitih formata datoteka."

############################# Header ############################
title: "Generirajte Codabar potpis crtičnog koda za Tiff dokument u C#"
description: "ePotpišite svoje Tiff poslovne dokumente pomoću Codabar crtičnog koda. Brzo i jednostavno generirajte potpis crtičnog koda s nekoliko redaka koda za postavljanje opcija potpisivanja."
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
    title: "O API-ju za potpise crtičnog koda GroupDocs.Signature for .NET."
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) je brz i jednostavan API za upravljanje e-potpisivanjem digitalnih dokumenata pomoću vrsta crtičnog koda kao što su UPCA, UPCE, EAN13, EAN14, Code39, Code39Extended, Code128, Codabar, Postnet, ISBN , ITF14 i mnogi drugi. Kupci mogu jednostavno kreirati crtične kodove sa potrebnim tekstom i staviti ih u PDF, Microsoft Office Words dokumente, Microsoft Office Excel radne knjige, MS PowerPoint prezentacije, Adobe Photoshop datoteke i razne formate slika. Crtični kodovi postavljeni u dokumente mogu se ažurirati, pretraživati, verificirati, brisati ili pregledavati. Štoviše, podržana je prilagodba crtičnih kodova.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Koraci za potpisivanje Tiff s Barcode u C#"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) pruža mogućnost brzog i jednostavnog potpisivanja Tiff dokumenata s Barcode potpisima.
        
        * Stvorite instancu klase potpisa koja daje Tiff datoteku koja bi se trebala potpisati kao put ili memorijski tok
        * Instancirajte klasu SignOptions i postavite sve tražene podatke.
        * Pozovite metodu Signature.Sign() prosljeđujući izlaznu datoteku Tiff ili memorijski tok

    title_right: " Zahtjevi sustava"
    content_right: |
        GroupDocs.Signature for .NET podržani su na svim glavnim platformama i operativnim sustavima. Prije izvršavanja koda u nastavku, provjerite imate li sljedeće preduvjete instalirane na vašem sustavu.

        * Operativni sustavi: Microsoft Windows, Linux, MacOS
        * Razvojna okruženja: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Preuzmite najnoviji GroupDocs.Signature for .NET od [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
        
        // Set up input Tiff file
        string filePath = "input.tiff";
        // Set up output file
        string outputFilePath = "output.tiff";

        // Instantiate Signature for input file
        using (var signature = new GroupDocs.Signature.Signature(filePath))
        {
                // create barcode option with predefined barcode text
                var options = new BarcodeSignOptions("BC12345678")
                {
                    // setup Barcode encoding type
                    EncodeType = BarcodeTypes.Codabar,

                    // set signature position
                    Left = 50,
                    Top = 50,
                    Width = 200,
                    Height = 50                                        
                };
                
                // sign Tiff document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Potpisivanje Tiff dokumenata s Barcode Live Demo"
    content: |
       Potpišite datoteku Tiff raznim potpisima upravo sada tako da posjetite [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) web mjesto. Besplatan online demo čeka na vas.

        
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-barcode"
          title: "About Codabar Barcode"
          content: |
            Codabar je simbologija linearnog crtičnog koda koja je dizajnirana za točno čitanje čak i kada se ispisuje na matričnim pisačima za višedijelne obrasce kao što su FedEx zračni računi i obrasci banke krvi.
          characterset: |
             Brojčane znamenke (0-9) i posebni znakovi $/-:+.
          textcapacity: |
             Nema posebnih ograničenja.
          image: |
             iVBORw0KGgoAAAANSUhEUgAAAD0AAABGCAYAAAB/h5zrAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsMAAA7DAcdvqGQAAAK2SURBVHhe7c9BagQBDAPB/f+nNxDQpUCOfc1MQx8khMGf7wN5n34K79NP4X36KYxPfz6fX0OyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2svfi3/I+/RTeJ9+Cg98+vv9AViQgD/8yuhqAAAAAElFTkSuQmCC

          link: ""

############################# More Formats ############################
more_formats:
    enable: true
    title: "Drugi podržani potpisi Barcode za C#"
    content: |
        "Također možete potpisati Tiff drugim vrstama potpisa. Pogledajte popis u nastavku."
    format: 
        
       
back_to_top:
    enable: true
---