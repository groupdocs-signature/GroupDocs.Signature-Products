---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Search
signaturetype: Qrcode
fileformat: Csv
productName: .NET
lang: ku
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Search Qrcode signatures at Csv with C#

############################# Head ############################
head_title: "Li Qrcode îmzeyan di pela Csv de di C# de bigerin"
head_description: ".NET ji bo lêgerîna îmzeyên Qrcode di pelên Csv de bi karanîna çend rêzikên kodê bikar bînin."

############################# Header ############################
title: "Di pela Csv de li îmzeyên Qrcode bigerin"
description: "API-ya xwecihî ya .NET destûrê dide ku meriv di pelên Csv yên jixwe îmzekirî de li îmzeyên Qrcode bigere. Lêgerîna pêşkeftî ya e-îmzayê di nav belgeyên xwe yên Csv de bi karanîna çend rêzikên kodê pêk bînin."
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true

    left:
        img_alt: "GroupDocs.Signature for .NET"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocsature-net.png"
        product: "GroupDocs.Signature"
        platform: ".NET"



############################# About ############################
about:
    enable: true
    title: "Derbarê GroupDocs.Signature for .NET API"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) API-ya .NET peyda dike ji bo ku belgeyan bi kar anîna cûrbecûr cûrbecûr îmzeyan wekî nivîs, wêne, sertîfîkayên dîjîtal, barkod, QR-kod, mor an metadata bi kar tîne. Bikarhêner dikarin di nav PDF, belgeyên MS Word, pirtûkên xebatê yên MS Excel, pêşandanên MS PowerPoint, pelên Adobe Photoshop û cûrbecûr formên wêneyan de, bi piştgirîyek zêde ji bo xweşkirina taybetmendiyên îmzeyan li gorî hewcedariyê zêde bikin, jêbikin, nûve bikin, verast bikin an bigerin.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Meriv çawa li îmzeyên Qrcode di Csv de digere"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) ji pêşdebirên .NET re hêsantir dike ku bi pêkanîna çend gavên hêsan li Qrcode di pelên Csv îmzeyan de ji sepanên xwe bigerin.
        
        * Nimûneyek nû ya çîna Îmzeyê biafirînin û riya belgeya çavkaniyê wekî parametreyek çêker derbas bikin.
        * Tişta Vebijêrkên Lêgerînê li gorî daxwazên xwe destnîşan bikin û vebijarkên lêgerînê diyar bikin.
        * Rêbaza Lêgerînê ya mînaka pola Îmzeyê bang bikin û Vebijarkên Lêgerînê jê re derbas bikin.
        * Encamên lêgerînê li gorî daxwazên xwe pêvajoyê bikin.

    title_right: "Pêdiviyên Sîstemê"
    content_right: |
        GroupDocs.Signature for .NET li ser hemî platform û pergalên xebitandinê yên sereke têne piştgirî kirin. Berî ku hûn koda jêrîn bicîh bikin, ji kerema xwe pê ewle bibin ku we şertên jêrîn li ser pergala we hatine saz kirin.

        * Pergalên xebitandinê: Microsoft Windows, Linux, MacOS
        * Jîngehên pêşkeftinê: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Guhertoya herî dawî ya GroupDocs.Signature for .NET ji [Nuget](https://www.nuget.org/packages/groupdocs.signature) dakêşîne
         
    code: |
        ```csharp    
                
        // Set up input Csv file
        string filePath = "input.csv";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                //Create search options
                QrCodeSearchOptions options = new QrCodeSearchOptions()
                {
                    // specify special pages to search on 
                    AllPages = false,
                    // single page number
                    PageNumber = 1,
                    // set up text match type
                    MatchType = TextMatchType.Contains,
                    // specify text pattern to search
                    Text = "Text signature",
                    // return  Qrcode images for processing
                    ReturnContent = true,
                    // set up type of returned  Qrcode images
                    ReturnContentType = FileType.PNG
                };

                // search for Qrcode signatures in Csv document
                List<QrCodeSignature> signatures = signature.Search<QrCodeSignature>(options);

                // process signatures which were found                
                foreach (QrCodeSignature item in signatures)
                {
                    //...
                }
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Li Qrcode îmzeyên elektronîkî Demoya Zindî bigerin"
    content: |
       Niha bi serdana malpera [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) di belgeyê de ji bo îmzeyên elektronîkî yên cihêreng ên pelên Csv bigerin.

        
############################# More Formats ############################
more_formats:
    enable: true
    title: "Li îmzeyên din ên Qrcode bi karanîna C# bigerin"
    content: |
        "Îmzeyên elektronîkî di belgeyên cihêreng de digerin. Wekî ku li jêr tê xuyang kirin, ji yek ji formatên pelê yên populer îmzeyan bibînin."
    format: 
           
       
back_to_top:
    enable: true
---