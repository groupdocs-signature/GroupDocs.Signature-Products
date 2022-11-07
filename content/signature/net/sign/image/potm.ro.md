---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Image
fileformat: Potm
productName: .NET
lang: ro
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Image signature on Potm for C#

############################# Head ############################
head_title: "Adăugarea de semnături Image la fișierul Potm cu C#"
head_description: "Puneți Image Semnătura pe fișierul Potm pentru .NET folosind câteva rânduri de cod. Utilizați API-ul GroupDocs Document Signature pentru a semna zeci de formate de fișiere."

############################# Header ############################
title: "Semnează fișiere Potm cu semnături Image în C#"
description: "Cum să adăugați semnătura Image cu câteva rânduri de cod .NET"
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
    title: "Despre GroupDocs.Signature for .NET API-ul pentru semnături imagine"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) este un API popular pentru semnarea electronică a documentelor digitale. Sunt disponibile semnături precum texte, imagini, certificate digitale, coduri de bare, coduri QR, ștampile sau metadate. Semnăturile pot fi plasate pe fișiere PDF, documente MS Word, cărți de lucru MS Excel, prezentări MS PowerPoint, fișiere Adobe Photoshop și diferite formate de imagine. Clienții își pot semna documentul și își pot actualiza, căuta, verifica, șterge sau previzualiza semnăturile electronice care au fost puse pe acele documente. În plus, sunt oferite o mulțime de abilități pentru personalizarea semnăturilor.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Pași pentru a semna Potm cu Image în C#"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) oferă posibilitatea de a semna documente Potm cu semnături Image rapid și ușor.
        
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
        // Provide image file
        string imageFilePath = "image.png";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
            //Provide sign options
            ImageSignOptions options = new ImageSignOptions(imageFilePath)
            {
                // set signature position
                Left = 50,
                Top = 200
            };

            // sign Potm document
            SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Semnează documente Potm cu Image Live Demo"
    content: |
       Semnați fișierul Potm cu diferite semnături chiar acum, vizitând site-ul web [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Demo online gratuită vă așteaptă.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Alte semnături acceptate de Image pentru C#"
    content: |
        "De asemenea, puteți semna Potm cu alte tipuri de semnături. Vă rugăm să vedeți lista de mai jos."
    format: 
       
       
back_to_top:
    enable: true
---