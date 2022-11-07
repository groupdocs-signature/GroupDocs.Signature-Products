---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Delete
signaturetype: Digital
fileformat: Xlsx
productName: .NET
lang: lv
productCode: net
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Xlsx for C#

############################# Head ############################
head_title: "Dzēst Digital parakstus no Xlsx failiem, izmantojot C#"
head_description: "Konkrētu Digital parakstu dzēšanu no parakstītiem Xlsx dokumentiem var viegli veikt, izmantojot īsu .NET kodu."

############################# Header ############################
title: "Noņemiet Digital parakstus, kas ir ievietoti Xlsx failos"
description: "Izdzēsiet dažādus Digital parakstus no Xlsx dokumentiem. Lai noņemtu Digital parakstus, ir nepieciešams vienkāršs C# kods."
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
    title: "Iegūstiet informāciju par GroupDocs.Signature for .NET API funkcijām"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) API nodrošina daudzus veidus, kā apstrādāt dokumentus, izmantojot elektroniskos parakstus. Ir pieejami digitālie paraksti, piemēram, teksti, attēli, digitālie sertifikāti, svītrkodi, QR kodi, zīmogi vai metadati. Klientiem ir iespēja pievienot, dzēst, atjaunināt, pārbaudīt vai meklēt ciparparakstus PDF, MS Word dokumentos, MS Excel darbgrāmatās, MS PowerPoint prezentācijās, Adobe Photoshop failos un dažādos attēlu formātos. Tiek nodrošināts liels skaits noderīgu funkciju un iestatījumu.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Kā noņemt Digital parakstus no sava Xlsx dokumenta"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) nodrošina noderīgu līdzekli, lai no Xlsx dokumentiem notīrītu Digital parakstus, izmantojot dažas koda rindiņas.
        
        * Pirmkārt, kā konstruktora parametru izveidojiet Signature objektu, kas nodod ceļu uz jūsu dokumentu.
        * Pēc tam izveidojiet atbilstošu paraksta objektu un iestatiet tā unikālo identifikatoru.
        * Pēc tam izsauciet Delete metodi, kas nodod paraksta objektu, kas ir jāizdzēš.
        * Visbeidzot, procesa darbības rezultāti.

    title_right: "Sistēmas prasības"
    content_right: |
        GroupDocs.Signature for .NET tiek atbalstīti visās lielākajās platformās un operētājsistēmās. Pirms tālāk norādītā koda izpildes, lūdzu, pārliecinieties, vai jūsu sistēmā ir instalēti šādi priekšnosacījumi.

        * Operētājsistēmas: Microsoft Windows, Linux, MacOS
        * Izstrādes vides: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Lejupielādējiet jaunāko GroupDocs.Signature for .NET versiju no [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Xlsx file
        string filePath = "input.xlsx";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                // Id of signature which is supposed to be deleted
                // such Id may be obtained as result of search operation
                string id = "a01e1940-997a-444b-89af-9309a2d559a5";

                // provide signature features to delete
                // set up particular signature id
                DigitalSignature signatureToDelete = new DigitalSignature(id);

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
    title: "Parakstīšana ar Digital parakstiem tiešraidē"
    content: |
       Pievienojiet dažādus elektroniskos parakstus failam Xlsx tūlīt, apmeklējot vietni [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Izdzēsiet savus Digital parakstus, izmantojot C#"
    content: |
        "Dažādiem dokumentu formātiem pievienoto e-parakstu dzēšana. Ātri noņemiet parakstus bez papildu koda."
    format: 
       
       
back_to_top:
    enable: true
---