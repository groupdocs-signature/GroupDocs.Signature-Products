---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Metadata
fileformat: Ods
productName: .NET
lang: ro
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Metadata signature on Ods for C#

############################# Head ############################
head_title: "Adăugați semnături electronice metadate la documente Ods prin C#"
head_description: "Utilizați metadatele ca semnături electronice ascunse în documentele dvs. Ods folosind câteva rânduri de cod C#. Utilizați API-ul GroupDocs Document Signature pentru a vă semna electronic documentele și fișierele de afaceri cu informații despre metadate."

############################# Header ############################
title: "Semnăturile electronice cu metadate pentru documentul Ods prin .NET sunt simple și ușor de utilizat!"
description: "eSemnați documentele și contractele Ods cu intrări de metadate ascunse. Generați metadate pentru PDF-uri, documente MS Word, registre de lucru MS Excel, prezentări MS PowerPoint și diferite formate de imagine fără probleme și codare suplimentară."
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
    title: "Despre GroupDocs.Signature for .NET API-ul pentru semnături metadate"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) este un API popular pentru semnarea electronică a documentelor digitale. Sunt disponibile semnături precum texte, imagini, certificate digitale, coduri de bare, coduri QR, ștampile sau metadate. Semnăturile pot fi plasate pe fișiere PDF, documente MS Word, cărți de lucru MS Excel, prezentări MS PowerPoint, fișiere Adobe Photoshop și diferite formate de imagine. Clienții își pot semna documentul și își pot actualiza, căuta, verifica, șterge sau previzualiza semnăturile electronice care au fost puse pe acele documente. În plus, sunt oferite o mulțime de abilități pentru personalizarea semnăturilor.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Pași pentru a semna Ods cu Metadata în C#"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) oferă posibilitatea de a semna documente Ods cu semnături Metadata rapid și ușor.
        
        * Creați o instanță a clasei Signature care furnizează fișierul Ods care ar trebui să se semneze ca cale sau flux de memorie
        * Instanțiați clasa SignOptions și setați toate datele solicitate.
        * Invocați metoda Signature.Sign() pasând fișierul de ieșire Ods sau fluxul de memorie

    title_right: " Cerințe de sistem"
    content_right: |
        GroupDocs.Signature for .NET sunt acceptate pe toate platformele și sistemele de operare majore. Înainte de a executa codul de mai jos, vă rugăm să vă asigurați că aveți următoarele cerințe preliminare instalate pe sistemul dumneavoastră.

        * Sisteme de operare: Microsoft Windows, Linux, MacOS
        * Medii de dezvoltare: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Obțineți cel mai recent GroupDocs.Signature for .NET de la [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
        
        // Set up input Ods file
        string filePath = "input.ods";
        // Set up output file
        string outputFilePath = "output.ods";

        // Instantiate Signature for input file
        using (var signature = new GroupDocs.Signature.Signature(filePath))
        {
                // instantiate metadata signing options
                var options = new MetadataSignOptions();

                // setup Author property
                SpreadsheetMetadataSignature mdSign_Author = new SpreadsheetMetadataSignature("Author", "Mr.Scherlock Holmes");// String value
                options.Signatures.Add(mdSign_Author);
                // setup document data
                SpreadsheetMetadataSignature mdSign_DocData = new SpreadsheetMetadataSignature("CreatedOn", DateTime.Now);// Datetime value
                options.Signatures.Add(mdSign_DocData);
                // setup document id
                SpreadsheetMetadataSignature mdSign_DocId = new SpreadsheetMetadataSignature("DocumentId", 123456);// Integer value
                options.Signatures.Add(mdSign_DocId);
                
                // sign Ods document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Semnează documente Ods cu Metadata Live Demo"
    content: |
       Semnați fișierul Ods cu diferite semnături chiar acum, vizitând site-ul web [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Demo online gratuită vă așteaptă.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Alte semnături acceptate de Metadata pentru C#"
    content: |
        "De asemenea, puteți semna Ods cu alte tipuri de semnături. Vă rugăm să vedeți lista de mai jos."
    format: 
       
       
back_to_top:
    enable: true
---