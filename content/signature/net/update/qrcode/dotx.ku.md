---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Update
signaturetype: Qrcode
fileformat: Dotx
productName: .NET
lang: ku
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Qrcode signature on Dotx for C#

############################# Head ############################
head_title: "Îmzeyên Qrcode li pelên Dotx bi C# hatine danîn nûve bikin"
head_description: "Ji bo têgihîştina koda .NET ji bo nûvekirina îmzeyan a Qrcode di belgeyên Dotx yên îmzekirî de hêsan û hêsan bikar bînin."

############################# Header ############################
title: "Îmzeyên ku li pelên Dotx hatine danîn biguherînin û nûve bikin"
description: "API ji bo .NET fonksîyonê ji bo îmzeyên Qrcode di belgeyên Dotx de nûve dike. E-îmzeyan di hundirê belgeyên xwe yên Dotx de bi çend rêzikên koda C# zû û bi hêsanî nûve bikin."
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
    title: "Li ser taybetmendiyên API-ê yên GroupDocs.Signature for .NET fêr bibin"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) Fonksiyonên API-ê hilbijarkek berfireh dihewîne da ku bi karanîna îmzeyên elektronîkî di formên belgeyên daxwazê ​​​​de were xebitandin. Berfirehiya e-îmzayên mîna nivîs, wêne, sertîfîkayên dîjîtal, barkod, QR-kod, stamp an metadata têne piştgirî kirin. Xerîdar dikarin li PDF, belgeyên MS Word, pirtûkên xebatê yên MS Excel, pêşandanên MS PowerPoint, pelên Adobe Photoshop û cûrbecûr formatên wêneyê lê zêde bikin, jêbirin, biguherînin, rast bikin an bigerin. Gelek taybetmendî û mîhengên kêrhatî hene.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Meriv çawa îmzeyên Qrcode di belgeya xweya Dotx de biguherîne"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) taybetmendiyên bikêrhatî yên mîna nûvekirina îmzeyên Qrcode yên ku li belgeyên Dotx hatine danîn, vedihewîne. Ew gengaz dike ku taybetmendiyên îmzeyan bêyî kodek zêde biguhezîne.
        
        * Ji bo destpêkê, tişta Îmzeyê biafirînin ku wekî rêgezek pîvana çêkerê ji belgeyek ku tê xwestin were nûve kirin derbas dibe.
        * Dûv re, tiştek nîşanek taybetî ya guncan destnîşan bikin û nasname û taybetmendiyên wê yên ku divê werin guheztin saz bikin.
        * Di dawiyê de, gazî rêbaza Nûvekirina Îmzeyê bikin ku tiştek nîşana taybetî derbas dike.
        * Pêvajoya nûvekirina encaman li gorî agahdariya we.

    title_right: "Pêdiviyên Sîstemê"
    content_right: |
        GroupDocs.Signature for .NET li ser hemî platform û pergalên xebitandinê yên sereke têne piştgirî kirin. Berî ku hûn koda jêrîn bicîh bikin, ji kerema xwe pê ewle bibin ku we şertên jêrîn li ser pergala we hatine saz kirin.

        * Pergalên xebitandinê: Microsoft Windows, Linux, MacOS
        * Jîngehên pêşkeftinê: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Guhertoya herî dawî ya GroupDocs.Signature for .NET ji [Nuget](https://www.nuget.org/packages/groupdocs.signature) dakêşîne
         
    code: |
        ```csharp    
                
        // Set up input Dotx file
        string filePath = "input.dotx";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                // Id of signature which is supposed to be updated
                // such Id might be got as a result of search operation
                string id = "eff64a14-dad9-47b0-88e5-2ee4e3604e71";

                // provide signature features to update
                // set up particular signature id
                QrCodeSignature signatureToUpdate = new QrCodeSignature(id)
                {
                    // specify signature width
                    Width = 200,
                    // specify signature height
                    Height = 200,
                    // set left position
                    Left = 120,
                    // set top position
                    Top = 160
                };

                // update signature
                bool updateResult = signature.Update(signatureToUpdate);

                // process updation result
                if (updateResult)
                {
                    Console.WriteLine("Signature was updated successfully!");
                }
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Nûvekirina îmzeyên Qrcode li ser rûpelên belgeyê - Demo Zindî"
    content: |
       Bi seredana malpera [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) aniha gelek îmzeyên elektronîkî yên belgeya Dotx biguherînin.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Bi rêya C# îmzeyên cihêreng ên Qrcode nûve bikin"
    content: |
        "Guhertina îmzeyên dîjîtal ên ku di formên belgeyên cihêreng de têne danîn. Daneyên îmzeyan bêyî kodek zêde nûve bikin."
    format: 
       
       
back_to_top:
    enable: true
---