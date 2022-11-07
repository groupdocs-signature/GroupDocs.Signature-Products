---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Search
signaturetype: Metadata
fileformat: Ott
productName: .NET
lang: ku
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Search Metadata signatures at Ott with C#

############################# Head ############################
head_title: "Li Metadata îmzeyan di pela Ott de di C# de bigerin"
head_description: ".NET ji bo lêgerîna îmzeyên Metadata di pelên Ott de bi karanîna çend rêzikên kodê bikar bînin."

############################# Header ############################
title: "Di pela Ott de li îmzeyên Metadata bigerin"
description: "API-ya xwecihî ya .NET destûrê dide ku meriv di pelên Ott yên jixwe îmzekirî de li îmzeyên Metadata bigere. Lêgerîna pêşkeftî ya e-îmzayê di nav belgeyên xwe yên Ott de bi karanîna çend rêzikên kodê pêk bînin."
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
    title_left: "Meriv çawa li îmzeyên Metadata di Ott de digere"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) ji pêşdebirên .NET re hêsantir dike ku bi pêkanîna çend gavên hêsan li Metadata di pelên Ott îmzeyan de ji sepanên xwe bigerin.
        
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
        
        // Set up input Ott file
        string filePath = "input.ott";

        // Instantiate Signature for input file
        using (var signature = new GroupDocs.Signature.Signature(filePath))
        {
                // search for Metadata signatures in Ott document
                List<WordProcessingMetadataSignature> signatures = signature.Search<WordProcessingMetadataSignature>(SignatureType.Metadata);

                // process signatures which were found 
                foreach (WordProcessingMetadataSignature item in signatures)
                {
                    //...
                }
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Li Metadata îmzeyên elektronîkî Demoya Zindî bigerin"
    content: |
       Niha bi serdana malpera [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) di belgeyê de ji bo îmzeyên elektronîkî yên cihêreng ên pelên Ott bigerin.

        
############################# More Formats ############################
more_formats:
    enable: true
    title: "Li îmzeyên din ên Metadata bi karanîna C# bigerin"
    content: |
        "Îmzeyên elektronîkî di belgeyên cihêreng de digerin. Wekî ku li jêr tê xuyang kirin, ji yek ji formatên pelê yên populer îmzeyan bibînin."
    format: 
           
       
back_to_top:
    enable: true
---