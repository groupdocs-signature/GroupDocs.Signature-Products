---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Verify
signaturetype: Qrcode
fileformat: Potm
productName: Java
lang: ku
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Qrcode signature on Potm for Java

############################# Head ############################
head_title: "Verastkirina îmzeyên Qrcode ji bo pelên Potm bi rêya Java"
head_description: "Tenê çend rêzên koda Java bikar bînin da ku belgeyên Potm û îmzeyên wan ên Qrcode rast bikin."

############################# Header ############################
title: "Verastkirina îmzeyan ji bo pelên Qrcode"
description: "API ji bo Java firsendê dide ku hûn îmzeyên Qrcode li ser belgeyên Potm verast bikin. Verastkirina e-îmzeyan di hundirê belgeyên we yên Potm de dibe ku zû û bi hêsanî were kirin."
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true

    left:
        img_alt: "GroupDocs.Signature for Java"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocs-signature-java.png"
        product: "GroupDocs.Signature"
        platform: "Java"



############################# About ############################
about:
    enable: true
    title: "Taybetmendiyên API-ê yên GroupDocs.Signature for Java yên nû keşif bikin"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) API rêgezên berfireh peyda dike ku meriv gelek formatên belgeyan bi karanîna îmzeyên elektronîkî veguhezîne. Gelek celeb îmzeyên dîjîtal ên wekî nivîs, wêne, sertîfîkayên dîjîtal, barkod, QR-kod, stamp an metadata têne piştgirî kirin. Xerîdar dikarin li PDF, belgeyên MS Word, pirtûkên xebatê yên MS Excel, pêşandanên MS PowerPoint, pelên Adobe Photoshop û cûrbecûr formatên wêneyê lê zêde bikin, jêbirin, biguherînin, rast bikin an bigerin. Hejmarek ecêb taybetmendî û mîhengên zêde hene.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Meriv çawa îmzeyên Qrcode di belgeya xweya Potm de rast bike"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) taybetmendîyên bikêrhatî yên wekî verastkirina îmzayên Qrcode yên ku li belgeyên Potm hatine danîn dihewîne. Vê derfetê bêyî pêkanîna kodek zêde bikar bînin.
        
        * Pêşîn, çîna Îmzeyê destnîşan bikin ku wekî rêgezek pîvana çêker ji belgeyek ku tê xwestin were verast kirin peyda dike.
        * Ya duyemîn, hêmanek nû ya VerifyOptions biafirînin û hemî taybetmendiyên pêwîst saz bikin.
        * Di dawiyê de, amûra Îmzeyê Verast bike ku mînaka VerifyOptions derbas dibe.
        * Piştre encamên verastkirinê pêvajoyê bikin.

    title_right: "Pêdiviyên Sîstemê"
    content_right: |
        GroupDocs.Signature for Java li ser hemî platform û pergalên xebitandinê yên sereke têne piştgirî kirin. Berî ku hûn koda jêrîn bicîh bikin, ji kerema xwe pê ewle bibin ku we şertên jêrîn li ser pergala we hatine saz kirin.

        * Pergalên xebitandinê: Microsoft Windows, Linux, MacOS
        * Jîngehên pêşkeftinê: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Guhertoya herî dawî ya GroupDocs.Signature for Java ji [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature) dakêşîne
         
    code: |
        ```java    
                
        // Set up input Potm file
        String filePath = "input.potm";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Provide verification options
        QrCodeVerifyOptions options = new QrCodeVerifyOptions();

        // process only first page
        options.setPagesSetup(new PagesSetup());
        options.setPageNumber(1);
        options.setAllPages(false);
        // specify text match type
        options.setMatchType(TextMatchType.StartsWith);
        // specify text pattern to search
        options.setText("QrCode text");
                            
        // Verify document signatures
        VerificationResult result = signature.verify(options);

        //process result
        if (result.isValid())
        {
            //..
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Îmzekirina bi Qrcode îmzeyan Demoya Zindî"
    content: |
       Bi serdana malpera [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) aniha gelek îmzeyên elektronîkî li pelê Potm zêde bikin.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Bi karanîna Java îmzeyên din ên Qrcode verast bikin"
    content: |
        "Verastkirina îmzeyên elektronîkî yên ku di belgeyên cihêreng de hatine bicîh kirin. Wekî ku li jêr têne xuyang kirin, kalîteya îmzeyan di formên pelên populer de kontrol bikin."
    format: 
       
       
back_to_top:
    enable: true
---