---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Digital
fileformat: Pdf
productName: .NET
lang: ro
productCode: net
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Pdf for C#

############################# Head ############################
head_title: "Adăugarea semnăturilor electronice digitale la fișierul Pdf cu C#"
head_description: "Puneți semnătura digitală pe fișierul Pdf pentru .NET folosind câteva rânduri de cod. Utilizați API-ul GroupDocs Document Signature pentru a semna zeci de formate de fișiere."

############################# Header ############################
title: "eSign fișiere Pdf cu semnături Digital în C#"
description: "Cum să adăugați semnătura Digital cu câteva rânduri de cod .NET"
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
    title: "Despre GroupDocs.Signature for .NET API-ul pentru semnături digitale"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) este un API popular pentru a semna documente cu semnături electronice digitale, cu certificate digitale. Pentru semnăturile digitale, API-ul utilizează fișiere de certificat PFX pentru a emite documentul cu chei publice și private protejate cu parolă. Semnăturile digitale pot fi folosite pentru a certifica documente de afaceri cu o anumită pagină eSign PDF, pentru a certifica documente întregi Microsoft Office, cum ar fi Words, Excel, fișiere Powerpoint și documente Open Office. Clienții pot manipula cu ușurință semnăturile, cum ar fi editarea, eliminarea sau ajustarea acestora. API-ul oferă o modalitate de a căuta și verifica semnăturile. În plus, sunt oferite o mulțime de abilități pentru personalizarea semnăturilor.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Pași pentru a semna Pdf cu Digital în C#"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) oferă posibilitatea de a semna documente Pdf cu semnături Digital rapid și ușor.
        
        * Creați o instanță a clasei Signature care furnizează fișierul Pdf care ar trebui să se semneze ca cale sau flux de memorie
        * Instanțiați clasa SignOptions și setați toate datele solicitate.
        * Invocați metoda Signature.Sign() pasând fișierul de ieșire Pdf sau fluxul de memorie

    title_right: " Cerințe de sistem"
    content_right: |
        GroupDocs.Signature for .NET sunt acceptate pe toate platformele și sistemele de operare majore. Înainte de a executa codul de mai jos, vă rugăm să vă asigurați că aveți următoarele cerințe preliminare instalate pe sistemul dumneavoastră.

        * Sisteme de operare: Microsoft Windows, Linux, MacOS
        * Medii de dezvoltare: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Obțineți cel mai recent GroupDocs.Signature for .NET de la [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Pdf file
        string filePath = "input.pdf";
        // Set up output file
        string outputFilePath = "output.pdf";
        // Provide digital certificate
        string certificateFilePath = "certificate.pfx";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                //Provide sign options
                DigitalSignOptions options = new DigitalSignOptions(certificateFilePath)
                {
                    // set certificate password
                    Password = "1234567890",
                    // set signature position
                    Left = 50,
                    Top = 200,
                };

                // sign Pdf document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Semnează documente Pdf cu Digital Live Demo"
    content: |
       Semnați fișierul Pdf cu diferite semnături chiar acum, vizitând site-ul web [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Demo online gratuită vă așteaptă.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Alte semnături acceptate de Digital pentru C#"
    content: |
        "De asemenea, puteți semna Pdf cu alte tipuri de semnături. Vă rugăm să vedeți lista de mai jos."
    format: 
       
       
back_to_top:
    enable: true
---