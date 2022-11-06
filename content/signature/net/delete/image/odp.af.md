---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Delete
signaturetype: Image
fileformat: Odp
productName: .NET
lang: af
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Image signature on Odp for C#

############################# Head ############################
head_title: "Vee Image handtekeninge van Odp lêers uit via C#"
head_description: "Die uitvee van spesifieke Image handtekeninge van getekende {{Lêerformaat}} dokumente kan maklik uitgevoer word met kort .NET kode."

############################# Header ############################
title: "Verwyder Image handtekeninge wat in {{Lêerformaat}} lêers geplaas is"
description: "Vee verskeie Image handtekeninge uit {{Lêerformaat}} dokumente uit. Die verwydering van Image handtekeninge vereis eenvoudige C# kode."
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
    title: "Kry inligting oor GroupDocs.Signature for .NET API-kenmerke"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) API bied baie maniere om jou dokumente te verwerk deur elektroniese handtekeninge te gebruik. Digitale handtekeninge soos tekste, beelde, digitale sertifikate, strepieskodes, QR-kodes, seëls of metadata is beskikbaar. Kliënte het die moontlikheid om digitale handtekeninge by PDF's, MS Word-dokumente, MS Excel-werkboeke, MS PowerPoint-aanbiedings, Adobe Photoshop-lêers en verskeie beeldformate by te voeg, uit te vee, op te dateer, te verifieer of te soek. 'n Groot aantal nuttige kenmerke en instellings word verskaf.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Hoe om Image-handtekeninge uit jou {{Lêerformaat}}-dokument te verwyder"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) bied nuttige kenmerk vir die skoonmaak van {{Lêerformaat}} dokumente van Image handtekeninge met 'n paar reëls kode.
        
        * Eerstens, instansieer Handtekening-objek wat deurgaanpad na jou dokument as 'n konstruktor parameter.
        * Skep dan 'n toepaslike handtekeningvoorwerp en stel sy unieke identifiseerder op.
        * Daarna, roep Verwyder metode deur handtekeningvoorwerp wat uitgevee moet word.
        * Laastens, die resultate van die proses.

    title_right: "Stelselvereistes"
    content_right: |
        GroupDocs.Signature for .NET word op alle groot platforms en bedryfstelsels ondersteun. Voordat u die kode hieronder uitvoer, maak asseblief seker dat u die volgende voorvereistes op u stelsel geïnstalleer het.

        * Bedryfstelsels: Microsoft Windows, Linux, MacOS
        * Ontwikkelingsomgewings: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Laai die nuutste weergawe van GroupDocs.Signature for .NET af vanaf [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Odp file
        string filePath = "input.odp";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                // Id of signature which is supposed to be deleted
                // such Id may be obtained as result of search operation
                string id = "e3ad0ec7-9abf-426d-b9aa-b3328f3f1470";

                // provide signature features to delete
                // set up particular signature id
                ImageSignature signatureToDelete = new ImageSignature(id);

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
    title: "Ondertekening met Image handtekeninge Live Demo"
    content: |
       Voeg nou verskeie elektroniese handtekeninge by die Odp-lêer deur die [GroupDocs.Signature-toepassing](https://products.groupdocs.app/signature/family) webwerf te besoek.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Vee jou Image handtekeninge uit met C#"
    content: |
        "Skraping van e-handtekeninge wat by verskeie dokumentformate gevoeg is. Verwyder handtekeninge vinnig sonder ekstra kode."
    format: 
       
       
back_to_top:
    enable: true
---