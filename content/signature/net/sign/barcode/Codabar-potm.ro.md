---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Barcode
codetype: Codabar
fileformat: Potm
productName: .NET
lang: ro
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put  Barcode signature on Potm for C#

############################# Head ############################
head_title: "eSign Potm document cu Codabar cod de bare în C#"
head_description: "Creați semnătura codului de bare Codabar și puneți-o pe documentul Potm cu .NET folosind câteva rânduri de cod. Utilizați API-ul GroupDocs Document Signature pentru a semna diferite formate de fișiere."

############################# Header ############################
title: "Generați semnătura de cod de bare Codabar pentru documentul Potm în C#"
description: "eSemnați documentele dvs. comerciale Potm cu codul de bare Codabar. Generați semnătura cod de bare rapid și ușor cu câteva linii de cod pentru a configura opțiunile de semnare."
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
    title: "Despre GroupDocs.Signature for .NET API-ul pentru semnături coduri de bare."
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) este un API rapid și ușor pentru a gestiona semnarea electronică a documentelor digitale folosind tipuri de coduri de bare precum UPCA, UPCE, EAN13, EAN14, Code39, Code39Extended, Code128, Codabar, Postnet, ISBN , ITF14 și multe altele. Clienții pot crea cu ușurință coduri de bare care oferă textul necesar și le pot pune pe PDF, documente Microsoft Office Words, cărți de lucru Microsoft Office Excel, prezentări MS PowerPoint, fișiere Adobe Photoshop și diferite formate de imagine. Codurile de bare plasate în documente pot fi actualizate, căutate, verificate, șterse sau previzualizate. În plus, personalizarea codurilor de bare este acceptată.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Pași pentru a semna Potm cu Barcode în C#"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) oferă posibilitatea de a semna documente Potm cu semnături Barcode rapid și ușor.
        
        * Creați o instanță a clasei Signature care furnizează fișierul Potm care ar trebui să se semneze ca cale sau flux de memorie
        * Instanțiați clasa SignOptions și setați toate datele solicitate.
        * Invocați metoda Signature.Sign() pasând fișierul de ieșire Potm sau fluxul de memorie

    title_right: " Cerințe de sistem"
    content_right: |
        GroupDocs.Signature for .NET sunt acceptate pe toate platformele și sistemele de operare majore. Înainte de a executa codul de mai jos, vă rugăm să vă asigurați că aveți următoarele cerințe preliminare instalate pe sistemul dumneavoastră.

        * Sisteme de operare: Microsoft Windows, Linux, MacOS
        * Medii de dezvoltare: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Obțineți cel mai recent GroupDocs.Signature for .NET de la [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
        
        // Set up input Potm file
        string filePath = "input.potm";
        // Set up output file
        string outputFilePath = "output.potm";

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
                
                // sign Potm document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Semnează documente Potm cu Barcode Live Demo"
    content: |
       Semnați fișierul Potm cu diferite semnături chiar acum, vizitând site-ul web [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Demo online gratuită vă așteaptă.

        
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-barcode"
          title: "About Codabar Barcode"
          content: |
            Codabar este un cod de bare liniar care a fost conceput pentru a fi citit cu acuratețe chiar și atunci când este imprimat pe imprimante cu matrice de puncte pentru formulare cu mai multe părți, cum ar fi biletele de avion FedEx și formularul de bancă de sânge.
          characterset: |
             Cifre numerice (0-9) și caractere speciale $/-:+.
          textcapacity: |
             Fără restricții specifice.
          image: |
             iVBORw0KGgoAAAANSUhEUgAAAD0AAABGCAYAAAB/h5zrAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsMAAA7DAcdvqGQAAAK2SURBVHhe7c9BagQBDAPB/f+nNxDQpUCOfc1MQx8khMGf7wN5n34K79NP4X36KYxPfz6fX0OyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2svfi3/I+/RTeJ9+Cg98+vv9AViQgD/8yuhqAAAAAElFTkSuQmCC

          link: ""

############################# More Formats ############################
more_formats:
    enable: true
    title: "Alte semnături acceptate de Barcode pentru C#"
    content: |
        "De asemenea, puteți semna Potm cu alte tipuri de semnături. Vă rugăm să vedeți lista de mai jos."
    format: 
        
       
back_to_top:
    enable: true
---