---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Delete
signaturetype: Digital
fileformat: Dotx
productName: Java
lang: ku
productCode: java
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Dotx for Java

############################# Head ############################
head_title: "Bi rêya Java îmzeyên Digital ji pelên Dotx jêbirin"
head_description: "Jêbirina îmzayên taybetî yên Digital ji belgeyên îmzekirî yên Dotx dibe ku bi koda kurt a Java bi hêsanî were kirin."

############################# Header ############################
title: "Nîşanên Digital yên ku di pelên Dotx de cih digirin rakin"
description: "Ji belgeyên Dotx îmzeyên cihêreng ên Digital jêbirin. Ji rakirina îmzeyên Digital koda Java ya sade hewce dike."
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
    title_left: "Meriv çawa îmzayên Digital ji belgeya xweya Dotx rabike"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) ji bo paqijkirina Dotx belgeyên Digital bi çend rêzikên kodê taybetmendiyek bikêr peyda dike.
        
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
                
        // Set up input Dotx file
        String filePath = "input.dotx";
        // Set up output file
        String outputFilePath = "output.dotx";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // Id of signature which is supposed to be deleted
        // such Id may be obtained as result of search operation
        String id = "a01e1940-997a-444b-89af-9309a2d559a5";

        // provide signature item to delete
        DigitalSignature signatureToDelete = new DigitalSignature(id);

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
    title: "Îmzekirina bi Digital îmzeyan Demoya Zindî"
    content: |
       Bi serdana malpera [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) aniha gelek îmzeyên elektronîkî li pelê Dotx zêde bikin.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Bi Java îmzeyên xwe yên Digital jêbikin"
    content: |
        "Jêbirina e-îmzayên ku li cûrbecûr formatên belgeyê hatine zêdekirin. Bêyî kodek zêde îmzeyan bi lez rakin."
    format: 
       
       
back_to_top:
    enable: true
---