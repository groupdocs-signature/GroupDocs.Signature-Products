---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Update
signaturetype: Image
fileformat: Pps
productName: Java
lang: ku
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Image signature on Pps for Java

############################# Head ############################
head_title: "Îmzeyên Image li pelên Pps bi Java hatine danîn nûve bikin"
head_description: "Ji bo têgihîştina koda Java ji bo nûvekirina îmzeyan a Image di belgeyên Pps yên îmzekirî de hêsan û hêsan bikar bînin."

############################# Header ############################
title: "Îmzeyên ku li pelên Pps hatine danîn biguherînin û nûve bikin"
description: "API ji bo Java fonksîyonê ji bo îmzeyên Image di belgeyên Pps de nûve dike. E-îmzeyan di hundirê belgeyên xwe yên Pps de bi çend rêzikên koda Java zû û bi hêsanî nûve bikin."
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
    title: "Li ser taybetmendiyên API-ê yên GroupDocs.Signature for Java fêr bibin"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) Fonksiyonên API-ê hilbijarkek berfireh dihewîne da ku bi karanîna îmzeyên elektronîkî di formên belgeyên daxwazê ​​​​de were xebitandin. Berfirehiya e-îmzayên mîna nivîs, wêne, sertîfîkayên dîjîtal, barkod, QR-kod, stamp an metadata têne piştgirî kirin. Xerîdar dikarin li PDF, belgeyên MS Word, pirtûkên xebatê yên MS Excel, pêşandanên MS PowerPoint, pelên Adobe Photoshop û cûrbecûr formatên wêneyê lê zêde bikin, jêbirin, biguherînin, rast bikin an bigerin. Gelek taybetmendî û mîhengên kêrhatî hene.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Meriv çawa îmzeyên Image di belgeya xweya Pps de biguherîne"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) taybetmendiyên bikêrhatî yên mîna nûvekirina îmzeyên Image yên ku li belgeyên Pps hatine danîn, vedihewîne. Ew gengaz dike ku taybetmendiyên îmzeyan bêyî kodek zêde biguhezîne.
        
        * Ji bo destpêkê, tişta Îmzeyê biafirînin ku wekî rêgezek pîvana çêkerê ji belgeyek ku tê xwestin were nûve kirin derbas dibe.
        * Dûv re, tiştek nîşanek taybetî ya guncan destnîşan bikin û nasname û taybetmendiyên wê yên ku divê werin guheztin saz bikin.
        * Di dawiyê de, gazî rêbaza Nûvekirina Îmzeyê bikin ku tiştek nîşana taybetî derbas dike.
        * Pêvajoya nûvekirina encaman li gorî agahdariya we.

    title_right: "Pêdiviyên Sîstemê"
    content_right: |
        GroupDocs.Signature for Java li ser hemî platform û pergalên xebitandinê yên sereke têne piştgirî kirin. Berî ku hûn koda jêrîn bicîh bikin, ji kerema xwe pê ewle bibin ku we şertên jêrîn li ser pergala we hatine saz kirin.

        * Pergalên xebitandinê: Microsoft Windows, Linux, MacOS
        * Jîngehên pêşkeftinê: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Guhertoya herî dawî ya GroupDocs.Signature for Java ji [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature) dakêşîne
         
    code: |
        ```java    
                
        // Set up input Pps file
        String filePath = "input.pps";
        // Set up output file
        String outputFilePath = "output.pps";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // Id of signature which is supposed to be updated
        // such Id might be got as a result of search operation
        String id = "ff988ab1-7403-4c8d-8db7-f2a56b9f8530";

        // provide signature features to update
        // set up particular signature id
        ImageSignature signatureToUpdate = new ImageSignature(id);

        // specify signature width
        signatureToUpdate.setWidth(170);
        // specify signature height
        signatureToUpdate.setHeight(250);
        // set left position
        signatureToUpdate.setLeft(10);
        // set top position
        signatureToUpdate.setTop(10);

        // update signature
        Boolean updateResult = signature.update(outputFilePath, signatureToUpdate);

        // process updation result
        if (updateResult)
        {
                System.out.println("Signature was updated successfully!");
        }
        ```

############################# Demos ############################
demos:
    enable: true
    title: "Nûvekirina îmzeyên Image li ser rûpelên belgeyê - Demo Zindî"
    content: |
       Bi seredana malpera [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) aniha gelek îmzeyên elektronîkî yên belgeya {{Pelformat}} biguherînin.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Bi rêya Java îmzeyên cihêreng ên Image nûve bikin"
    content: |
        "Guhertina îmzeyên dîjîtal ên ku di formên belgeyên cihêreng de têne danîn. Daneyên îmzeyan bêyî kodek zêde nûve bikin."
    format: 
       
       
back_to_top:
    enable: true
---