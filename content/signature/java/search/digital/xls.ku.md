---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Search
signaturetype: Digital
fileformat: Xls
productName: Java
lang: ku
productCode: java
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Search Digital signatures at Xls with Java

############################# Head ############################
head_title: "Li Digital îmzeyan di pela Xls de di Java de bigerin"
head_description: "Java ji bo lêgerîna îmzeyên Digital di pelên Xls de bi karanîna çend rêzikên kodê bikar bînin."

############################# Header ############################
title: "Di pela Xls de li îmzeyên Digital bigerin"
description: "API-ya xwecihî ya Java destûrê dide ku meriv di pelên Xls yên jixwe îmzekirî de li îmzeyên Digital bigere. Lêgerîna pêşkeftî ya e-îmzayê di nav belgeyên xwe yên Xls de bi karanîna çend rêzikên kodê pêk bînin."
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
    title_left: "Meriv çawa li îmzeyên Digital di Xls de digere"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) ji pêşdebirên Java re hêsantir dike ku bi pêkanîna çend gavên hêsan li Digital di pelên Xls îmzeyan de ji sepanên xwe bigerin.
        
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
                
        // Set up input Xls file
        String filePath = "input.xls";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Create search options
        DigitalSearchOptions options = new DigitalSearchOptions();

        // specify special search criteria
        options.setComments("Approved");
        // specify period of signatures
        options.setSignDateTimeFrom(new Date(2021, 3, 5));
        options.setSignDateTimeTo(new Date(2022, 7, 16));
        
        // search for Digital signatures in Xls document
        List<DigitalSignature> signatures = signature.search(DigitalSignature.class, options);

        // process signatures which were found 
        signatures.forEach(item -> System.out.println(item.toString()));

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Li Digital îmzeyên elektronîkî Demoya Zindî bigerin"
    content: |
       Niha bi serdana malpera [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) di belgeyê de ji bo îmzeyên elektronîkî yên cihêreng ên pelên Xls bigerin.

        
############################# More Formats ############################
more_formats:
    enable: true
    title: "Li îmzeyên din ên Digital bi karanîna Java bigerin"
    content: |
        "Îmzeyên elektronîkî di belgeyên cihêreng de digerin. Wekî ku li jêr tê xuyang kirin, ji yek ji formatên pelê yên populer îmzeyan bibînin."
    format: 
           
       
back_to_top:
    enable: true
---