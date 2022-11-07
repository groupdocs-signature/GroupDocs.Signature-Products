---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Delete
signaturetype: Text
fileformat: Xlsm
productName: .NET
lang: ku
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Text signature on Xlsm for C#

############################# Head ############################
head_title: "Bi rêya C# îmzeyên Text ji pelên Xlsm jêbirin"
head_description: "Jêbirina îmzayên taybetî yên Text ji belgeyên îmzekirî yên Xlsm dibe ku bi koda kurt a .NET bi hêsanî were kirin."

############################# Header ############################
title: "Nîşanên Text yên ku di pelên Xlsm de cih digirin rakin"
description: "Ji belgeyên Xlsm îmzeyên cihêreng ên Text jêbirin. Ji rakirina îmzeyên Text koda C# ya sade hewce dike."
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
    title: "Li ser taybetmendiyên API-ê yên GroupDocs.Signature for .NET agahdarî bistînin"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) API gelek awayan peyda dike ku hûn belgeyên we bi karanîna îmzeyên elektronîkî bi kar bînin. Îmzeyên dîjîtal ên wekî nivîs, wêne, sertîfîkayên dîjîtal, barkod, QR-kod, stamp an metadata hene. Xerîdar xwedî îmkan in ku li PDF, belgeyên MS Word, pirtûkên xebatê yên MS Excel, pêşandanên MS PowerPoint, pelên Adobe Photoshop û cûrbecûr formatên wêneyê lê zêde bikin, jêbikin, nûve bikin, verast bikin an li îmzeyên dîjîtal bigerin. Gelek taybetmendiyên kêrhatî û mîhengan têne peyda kirin.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Meriv çawa îmzayên Text ji belgeya xweya Xlsm rabike"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) ji bo paqijkirina Xlsm belgeyên Text bi çend rêzikên kodê taybetmendiyek bikêr peyda dike.
        
        * Pêşîn, tişta Îmzeyê ya ku ji belgeya we re wekî parametreyek çêker derbas dibe destnîşan bikin.
        * Dûv re, tiştek îmzeya guncan biafirînin û nasnameya wê ya yekta saz bikin.
        * Piştî wê, rêbaza Jêbirinê vekêşin ku tiştê îmzeyê derbas dike ku divê were jêbirin.
        * Di dawiyê de, encamên operasyonê.

    title_right: "Pêdiviyên Sîstemê"
    content_right: |
        GroupDocs.Signature for .NET li ser hemî platform û pergalên xebitandinê yên sereke têne piştgirî kirin. Berî ku hûn koda jêrîn bicîh bikin, ji kerema xwe pê ewle bibin ku we şertên jêrîn li ser pergala we hatine saz kirin.

        * Pergalên xebitandinê: Microsoft Windows, Linux, MacOS
        * Jîngehên pêşkeftinê: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Guhertoya herî dawî ya GroupDocs.Signature for .NET ji [Nuget](https://www.nuget.org/packages/groupdocs.signature) dakêşîne
         
    code: |
        ```csharp    
                
        // Set up input Xlsm file
        string filePath = "input.xlsm";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                // Id of signature which is supposed to be deleted
                // such Id may be obtained as result of search operation
                string id = "ff988ab1-7403-4c8d-8db7-f2a56b9f8530";

                // provide signature features to delete
                // set up particular signature id
                TextSignature signatureToDelete = new TextSignature(id);

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
    title: "Îmzekirina bi Text îmzeyan Demoya Zindî"
    content: |
       Bi serdana malpera [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) aniha gelek îmzeyên elektronîkî li pelê Xlsm zêde bikin.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Bi C# îmzeyên xwe yên Text jêbikin"
    content: |
        "Jêbirina e-îmzayên ku li cûrbecûr formatên belgeyê hatine zêdekirin. Bêyî kodek zêde îmzeyan bi lez rakin."
    format: 
       
       
back_to_top:
    enable: true
---