---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Verify
signaturetype: Text
fileformat: Odp
productName: .NET
lang: ku
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Text signature on Odp for C#

############################# Head ############################
head_title: "Verastkirina îmzeyên Text ji bo pelên Odp bi rêya C#"
head_description: "Tenê çend rêzên koda .NET bikar bînin da ku belgeyên Odp û îmzeyên wan ên Text rast bikin."

############################# Header ############################
title: "Verastkirina îmzeyan ji bo pelên Text"
description: "API ji bo .NET firsendê dide ku hûn îmzeyên Text li ser belgeyên Odp verast bikin. Verastkirina e-îmzeyan di hundirê belgeyên we yên {{Pelformat}} de dibe ku zû û bi hêsanî were kirin."
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
    title: "Taybetmendiyên API-ê yên GroupDocs.Signature for .NET yên nû keşif bikin"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) API rêgezên berfireh peyda dike ku meriv gelek formatên belgeyan bi karanîna îmzeyên elektronîkî veguhezîne. Gelek celeb îmzeyên dîjîtal ên wekî nivîs, wêne, sertîfîkayên dîjîtal, barkod, QR-kod, stamp an metadata têne piştgirî kirin. Xerîdar dikarin li PDF, belgeyên MS Word, pirtûkên xebatê yên MS Excel, pêşandanên MS PowerPoint, pelên Adobe Photoshop û cûrbecûr formatên wêneyê lê zêde bikin, jêbirin, biguherînin, rast bikin an bigerin. Hejmarek ecêb taybetmendî û mîhengên zêde hene.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Meriv çawa îmzeyên Text di belgeya xweya Odp de rast bike"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) taybetmendîyên bikêrhatî yên wekî verastkirina îmzayên Text yên ku li belgeyên Odp hatine danîn dihewîne. Vê derfetê bêyî pêkanîna kodek zêde bikar bînin.
        
        * Pêşîn, çîna Îmzeyê destnîşan bikin ku wekî rêgezek pîvana çêker ji belgeyek ku tê xwestin were verast kirin peyda dike.
        * Ya duyemîn, hêmanek nû ya VerifyOptions biafirînin û hemî taybetmendiyên pêwîst saz bikin.
        * Di dawiyê de, amûra Îmzeyê Verast bike ku mînaka VerifyOptions derbas dibe.
        * Piştre encamên verastkirinê pêvajoyê bikin.

    title_right: "Pêdiviyên Sîstemê"
    content_right: |
        GroupDocs.Signature for .NET li ser hemî platform û pergalên xebitandinê yên sereke têne piştgirî kirin. Berî ku hûn koda jêrîn bicîh bikin, ji kerema xwe pê ewle bibin ku we şertên jêrîn li ser pergala we hatine saz kirin.

        * Pergalên xebitandinê: Microsoft Windows, Linux, MacOS
        * Jîngehên pêşkeftinê: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Guhertoya herî dawî ya GroupDocs.Signature for .NET ji [Nuget](https://www.nuget.org/packages/groupdocs.signature) dakêşîne
         
    code: |
        ```csharp    
                
        // Set up input Odp file
        string filePath = "input.odp";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                //Provide verification options
                TextVerifyOptions options = new TextVerifyOptions()
                {
                    // Process all pages 
                    AllPages = true,
                    // set up text match type
                    MatchType = TextMatchType.Exact,
                    // specify text pattern to search
                    Text = "Very important signature",
                };

                // Verify document signatures
                VerificationResult result = signature.Verify(options);

                //process result
                if (result.IsValid)
                {
                    //..
                }
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Îmzekirina bi Text îmzeyan Demoya Zindî"
    content: |
       Bi serdana malpera [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) aniha gelek îmzeyên elektronîkî li pelê Odp zêde bikin.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Bi karanîna C# îmzeyên din ên Text verast bikin"
    content: |
        "Verastkirina îmzeyên elektronîkî yên ku di belgeyên cihêreng de hatine bicîh kirin. Wekî ku li jêr têne xuyang kirin, kalîteya îmzeyan di formên pelên populer de kontrol bikin."
    format: 
       
       
back_to_top:
    enable: true
---