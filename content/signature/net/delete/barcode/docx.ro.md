---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Delete
signaturetype: Barcode
fileformat: Docx
productName: .NET
lang: ro
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Barcode signature on Docx for C#

############################# Head ############################
head_title: "Ștergeți semnăturile Barcode din fișierele Docx prin C#"
head_description: "Ștergerea anumitor semnături Barcode din documentele Docx semnate poate fi efectuată cu ușurință cu ajutorul unui cod scurt .NET."

############################# Header ############################
title: "Eliminați semnăturile Barcode care sunt plasate în fișiere Docx"
description: "Ștergeți diferite semnături Barcode din documentele Docx. Eliminarea semnăturilor Barcode necesită un cod simplu C#."
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
    title: "Obțineți informații despre funcțiile API-ului GroupDocs.Signature for .NET"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) API oferă multe modalități de a vă procesa documentele folosind semnături electronice. Sunt disponibile semnături digitale precum texte, imagini, certificate digitale, coduri de bare, coduri QR, ștampile sau metadate. Clienții au posibilitatea de a adăuga, șterge, actualiza, verifica sau căuta semnături digitale în PDF-uri, documente MS Word, registre de lucru MS Excel, prezentări MS PowerPoint, fișiere Adobe Photoshop și diferite formate de imagine. Sunt oferite un număr mare de funcții și setări utile.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Cum să eliminați semnăturile Barcode din documentul dvs. Docx"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) oferă o funcție utilă pentru ștergerea documentelor Docx de semnăturile Barcode cu câteva linii de cod.
        
        * În primul rând, instanțiază obiectul Signature care trece calea către documentul tău ca parametru de constructor.
        * Apoi, creați un obiect de semnătură adecvat și configurați identificatorul unic al acestuia.
        * {steps.content_left.step_3}
        * {steps.content_left.step_4}

    title_right: "Cerințe de sistem"
    content_right: |
        GroupDocs.Signature for .NET sunt acceptate pe toate platformele și sistemele de operare majore. Înainte de a executa codul de mai jos, vă rugăm să vă asigurați că aveți următoarele cerințe preliminare instalate pe sistemul dumneavoastră.

        * Sisteme de operare: Microsoft Windows, Linux, MacOS
        * Medii de dezvoltare: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Descărcați cea mai recentă versiune a GroupDocs.Signature for .NET de la [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Docx file
        string filePath = "input.docx";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                // Id of signature which is supposed to be deleted
                // such Id may be obtained as result of search operation
                string id = "07f83369-318b-41ad-a843-732417b912c2";

                // provide signature features to delete
                // set up particular signature id
                BarcodeSignature signatureToDelete = new BarcodeSignature(id);

                // delete signature
                bool deleteResult = signature.Delete(signatureToDelete);

                // process deletion result
                if (deleteResult)
                {
                    Console.WriteLine("Signature was deleted successfully!");
                }
        }
        ```

############################# Demos ############################
demos:
    enable: true
    title: "Semnează cu Barcode semnături Demo live"
    content: |
       Adăugați diverse semnături electronice în fișierul Docx chiar acum, vizitând site-ul web [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Ștergeți-vă semnăturile Barcode cu C#"
    content: |
        "Ștergerea semnăturilor electronice care au fost adăugate la diferite formate de documente. Eliminați rapid semnăturile fără cod suplimentar."
    format: 
       
       
back_to_top:
    enable: true
---