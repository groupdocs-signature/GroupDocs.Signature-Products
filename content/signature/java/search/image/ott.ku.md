---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Search
signaturetype: Image
fileformat: Ott
productName: Java
lang: ku
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Search Image signatures at Ott with Java

############################# Head ############################
head_title: "Li Image îmzeyan di pela Ott de di Java de bigerin"
head_description: "Java ji bo lêgerîna îmzeyên Image di pelên Ott de bi karanîna çend rêzikên kodê bikar bînin."

############################# Header ############################
title: "Di pela Ott de li îmzeyên Image bigerin"
description: "API-ya xwecihî ya Java destûrê dide ku meriv di pelên Ott yên jixwe îmzekirî de li îmzeyên Image bigere. Lêgerîna pêşkeftî ya e-îmzayê di nav belgeyên xwe yên Ott de bi karanîna çend rêzikên kodê pêk bînin."
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true

    left:
        img_alt: "GroupDocs.Signature for Java"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocsature-java.png"
        product: "GroupDocs.Signature"
        platform: "Java"



############################# About ############################
about:
    enable: true
    title: "Derbarê GroupDocs.Signature for Java API"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) API-ya Java peyda dike ji bo ku belgeyan bi kar anîna cûrbecûr cûrbecûr îmzeyan wekî nivîs, wêne, sertîfîkayên dîjîtal, barkod, QR-kod, mor an metadata bi kar tîne. Bikarhêner dikarin di nav PDF, belgeyên MS Word, pirtûkên xebatê yên MS Excel, pêşandanên MS PowerPoint, pelên Adobe Photoshop û cûrbecûr formên wêneyan de, bi piştgirîyek zêde ji bo xweşkirina taybetmendiyên îmzeyan li gorî hewcedariyê zêde bikin, jêbikin, nûve bikin, verast bikin an bigerin.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Meriv çawa li îmzeyên Image di Ott de digere"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) ji pêşdebirên Java re hêsantir dike ku bi pêkanîna çend gavên hêsan li Image di pelên Ott îmzeyan de ji sepanên xwe bigerin.
        
        * Nimûneyek nû ya çîna Îmzeyê biafirînin û riya belgeya çavkaniyê wekî parametreyek çêker derbas bikin.
        * Tişta Vebijêrkên Lêgerînê li gorî daxwazên xwe destnîşan bikin û vebijarkên lêgerînê diyar bikin.
        * Rêbaza Lêgerînê ya mînaka pola Îmzeyê bang bikin û Vebijarkên Lêgerînê jê re derbas bikin.
        * Encamên lêgerînê li gorî daxwazên xwe pêvajoyê bikin.

    title_right: "Pêdiviyên Sîstemê"
    content_right: |
        GroupDocs.Signature for Java li ser hemî platform û pergalên xebitandinê yên sereke têne piştgirî kirin. Berî ku hûn koda jêrîn bicîh bikin, ji kerema xwe pê ewle bibin ku we şertên jêrîn li ser pergala we hatine saz kirin.

        * Pergalên xebitandinê: Microsoft Windows, Linux, MacOS
        * Jîngehên pêşkeftinê: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Guhertoya herî dawî ya GroupDocs.Signature for Java ji [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature) dakêşîne
         
    code: |
        ```java    
                
        // Set up input Ott file
        String filePath = "input.ott";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Create search options
        ImageSearchOptions options = new ImageSearchOptions();

        // set minimum size if needed 
        options.setMinContentSize(100);
        // set maximum image size if needed
        options.setMaxContentSize(2000);
        // return images for processing
        options.setReturnContent(true);
        // set up type of returned images
        options.setReturnContentType(FileType.PNG);

        // search for Image signatures in Ott document
        List<ImageSignature> signatures = signature.search(ImageSignature.class, options);

        // process signatures which were found 
        signatures.forEach(item -> System.out.println(item.toString()));

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Li Image îmzeyên elektronîkî Demoya Zindî bigerin"
    content: |
       Niha bi serdana malpera [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) di belgeyê de ji bo îmzeyên elektronîkî yên cihêreng ên pelên Ott bigerin.

        
############################# More Formats ############################
more_formats:
    enable: true
    title: "Li îmzeyên din ên Image bi karanîna Java bigerin"
    content: |
        "Îmzeyên elektronîkî di belgeyên cihêreng de digerin. Wekî ku li jêr tê xuyang kirin, ji yek ji formatên pelê yên populer îmzeyan bibînin."
    format: 
           
       
back_to_top:
    enable: true
---