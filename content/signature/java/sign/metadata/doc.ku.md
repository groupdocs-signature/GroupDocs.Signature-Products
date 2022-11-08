---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Metadata
fileformat: Doc
productName: Java
lang: ku
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Metadata signature on Doc for Java

############################# Head ############################
head_title: "Bi rêya Java îmzeyên elektronîkî yên Metadata li belgeyên Doc bişînin"
head_description: "Metadata wekî îmzeyên elektronîkî yên veşartî di hundurê belgeyên xwe yên Doc de bi karanîna çend rêzikên koda Java bikar bînin. API-ya Îmzekirina Belgeya GroupDocs bikar bînin da ku belge û pelên karsaziya xwe bi agahdariya Metadata e-îmza bikin."

############################# Header ############################
title: "Îmzeyên elektronîkî yên metadata ji bo belgeya Doc bi rêya Java ji bo karanîna hêsan û hêsan in!"
description: "Belge û peymanên xwe yên Doc bi navnîşên Metadata veşartî re îmze bikin. Ji bo PDF, belgeyên MS Word, pirtûkên xebatê MS Excel, pêşandanên MS PowerPoint û cûrbecûr formatên wêneyê bêyî pirsgirêk û kodkirina zêde Metadata biafirînin."
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
    title: "Der barê GroupDocs.Signature for Java API-ya îmzeyên metadata"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) API-ya navdar e ji bo e-îmzakirina belgeyên dîjîtal. Îmzeyên wekî nivîs, wêne, sertîfîkayên dîjîtal, barkod, QR-kod, stamp an metadata hene. Dibe ku îmze li ser PDF, belgeyên MS Word, pirtûkên xebatê yên MS Excel, pêşandanên MS PowerPoint, pelên Adobe Photoshop û cûrbecûr formên wêneyan werin danîn. Xerîdar dikarin belgeya xwe îmze bikin û e-îmzayên ku li ser wan belgeyan hatine danîn nûve bikin, bigerin, verast bikin, jêbikin an pêşdîtin bikin. Digel vê yekê, ji bo xwerûkirina îmzeyan gelek jêhatî têne peyda kirin.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Gavên îmzekirina Doc bi Metadata di Java de"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) îmzakirina belgeyên Doc bi îmzeyên Metadata zû û bi hêsanî peyda dike.
        
        * Nimûneyek ji çîna îmzayê biafirîne ku pelê Doc pêşkêş dike ku divê wekî rêyek an herikîna bîranînê were îmzekirin
        * Dersa SignOptions destnîşan bikin û hemî daneyên daxwazkirî bicîh bikin.
        * Rêbaza Signature.Sign() vexwend ku derana pelê Doc an jî herikîna bîrê derbas dike

    title_right: " Pêdiviyên Sîstemê"
    content_right: |
        GroupDocs.Signature for Java li ser hemî platform û pergalên xebitandinê yên sereke têne piştgirî kirin. Berî ku hûn koda jêrîn bicîh bikin, ji kerema xwe pê ewle bibin ku we şertên jêrîn li ser pergala we hatine saz kirin.

        * Pergalên xebitandinê: Microsoft Windows, Linux, MacOS
        * Jîngehên pêşkeftinê: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Nûtirîn GroupDocs.Signature for Java ji [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature) bistînin
         
    code: |
        ```java    
                
        // Set up input Doc file
        String filePath = "input.doc";
        // Set up output file
        String outputFilePath = "output.doc";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // instantiate metadata signing options
        MetadataSignOptions options = new MetadataSignOptions();

        // setup Author property
        WordProcessingMetadataSignature mdSign_Author = new WordProcessingMetadataSignature("Author", "Mr.Scherlock Holmes");// String value
        options.getSignatures().add(mdSign_Author);
        // setup document data
        WordProcessingMetadataSignature mdSign_DocData = new WordProcessingMetadataSignature("CreatedOn", new Date());// Datetime value
        options.getSignatures().add(mdSign_DocData);
        // setup document id
        WordProcessingMetadataSignature mdSign_DocId = new WordProcessingMetadataSignature("DocumentId", 123456);// Integer value
        options.getSignatures().add(mdSign_DocId);

        // sign Doc document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Îmzekirina belgeyên Doc bi Metadata Demoya Zindî"
    content: |
       Naha bi serdana malpera [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) pelê Doc bi îmzeyên cihêreng îmze bikin. Demoya serhêl a belaş li benda we ye.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Îmzeyên din ên piştgirî yên Metadata ji bo Java"
    content: |
        "Her weha hûn dikarin Doc bi celebên din ên îmzayê re îmze bikin. Ji kerema xwe lîsteya jêrîn bibînin."
    format: 
       
       
back_to_top:
    enable: true
---