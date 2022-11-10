---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Delete
signaturetype: Qrcode
fileformat: Odt
productName: Java
lang: ku
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Qrcode signature on Odt for Java

############################# Head ############################
head_title: "Bi rêya Java îmzeyên Qrcode ji pelên Odt jêbirin"
head_description: "Jêbirina îmzayên taybetî yên Qrcode ji belgeyên îmzekirî yên Odt dibe ku bi koda kurt a Java bi hêsanî were kirin."

############################# Header ############################
title: "Nîşanên Qrcode yên ku di pelên Odt de cih digirin rakin"
description: "Ji belgeyên Odt îmzeyên cihêreng ên Qrcode jêbirin. Ji rakirina îmzeyên Qrcode koda Java ya sade hewce dike."
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
    title: "Li ser taybetmendiyên API-ê yên GroupDocs.Signature for Java agahdarî bistînin"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) API gelek awayan peyda dike ku hûn belgeyên we bi karanîna îmzeyên elektronîkî bi kar bînin. Îmzeyên dîjîtal ên wekî nivîs, wêne, sertîfîkayên dîjîtal, barkod, QR-kod, stamp an metadata hene. Xerîdar xwedî îmkan in ku li PDF, belgeyên MS Word, pirtûkên xebatê yên MS Excel, pêşandanên MS PowerPoint, pelên Adobe Photoshop û cûrbecûr formatên wêneyê lê zêde bikin, jêbikin, nûve bikin, verast bikin an li îmzeyên dîjîtal bigerin. Gelek taybetmendiyên kêrhatî û mîhengan têne peyda kirin.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Meriv çawa îmzayên Qrcode ji belgeya xweya Odt rabike"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) ji bo paqijkirina Odt belgeyên Qrcode bi çend rêzikên kodê taybetmendiyek bikêr peyda dike.
        
        * Pêşîn, tişta Îmzeyê ya ku ji belgeya we re wekî parametreyek çêker derbas dibe destnîşan bikin.
        * Dûv re, tiştek îmzeya guncan biafirînin û nasnameya wê ya yekta saz bikin.
        * Piştî wê, rêbaza Jêbirinê vekêşin ku tiştê îmzeyê derbas dike ku divê were jêbirin.
        * Di dawiyê de, encamên operasyonê.

    title_right: "Pêdiviyên Sîstemê"
    content_right: |
        GroupDocs.Signature for Java li ser hemî platform û pergalên xebitandinê yên sereke têne piştgirî kirin. Berî ku hûn koda jêrîn bicîh bikin, ji kerema xwe pê ewle bibin ku we şertên jêrîn li ser pergala we hatine saz kirin.

        * Pergalên xebitandinê: Microsoft Windows, Linux, MacOS
        * Jîngehên pêşkeftinê: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Guhertoya herî dawî ya GroupDocs.Signature for Java ji [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature) dakêşîne
         
    code: |
        ```java    
                
        // Set up input Odt file
        String filePath = "input.odt";
        // Set up output file
        String outputFilePath = "output.odt";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // Id of signature which is supposed to be deleted
        // such Id may be obtained as result of search operation
        String id = "eff64a14-dad9-47b0-88e5-2ee4e3604e71";

        // provide signature features to delete
        QrCodeSignature signatureToDelete = new QrCodeSignature(id);

        // delete signature
        Boolean deleteResult = signature.delete(outputFilePath, signatureToDelete);

        // process deletion result
        if (deleteResult)
        {
                System.out.println("Signature was deleted successfully!");
        }
        ```

############################# Demos ############################
demos:
    enable: true
    title: "Îmzekirina bi Qrcode îmzeyan Demoya Zindî"
    content: |
       Bi serdana malpera [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) aniha gelek îmzeyên elektronîkî li pelê Odt zêde bikin.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Bi Java îmzeyên xwe yên Qrcode jêbikin"
    content: |
        "Jêbirina e-îmzayên ku li cûrbecûr formatên belgeyê hatine zêdekirin. Bêyî kodek zêde îmzeyan bi lez rakin."
    format: 
       
       
back_to_top:
    enable: true
---