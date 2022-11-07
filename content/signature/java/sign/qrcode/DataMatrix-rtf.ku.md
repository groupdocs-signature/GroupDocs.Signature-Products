---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Qrcode
codetype: Data Matrix
fileformat: Rtf
productName: Java
lang: ku
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put  Qrcode signature on Rtf for Java

############################# Head ############################
head_title: "Belgeya eSign {{Pelformat}} bi Data Matrix Koda QR di Java"
head_description: "Koda QR-a Data Matrix biafirînin û bi koda Java bi koda Java li pelê Rtf bixin. API-ya Îmzekirina Belgeya GroupDocs bikar bînin da ku belge û pelên karsaziya xwe bi QR Code e-îmza bikin."

############################# Header ############################
title: "Di Java de ji bo belgeya Data Matrix îmzeya Koda QR çêbike"
description: "Belge û peymanên xwe yên {{Pelformat}} bi koda QR-a Data Matrix îmze bikin. Zû û bi hêsanî îmzeya QR Code biafirînin."
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
    title: "Der barê GroupDocs.Signature for Java API-ya îmzeyên QR Code"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) API-ya gihîştî ye ku ji bo belgeyan îmzeyên QR Code çêbike û çêbike. Bikarhêner dikarin îmzeyên QR Code peyda bikin ku nivîsê dakêşin an li ser medyaya civakî wekî wêneyê parve bikin. Belgeya îmzekirî dikare bi API-ê an jî bi tenê li ser kameraya mobîl were skankirin! Peymanên karsaziya xwe û belgeyên fermî bi elektronîkî bi zêdekirina îmzeya QR Code îmze bikin û wê manîpule bikin. Her îmzeya QR Code dê agahdariya xwerû ya yekta hebe da ku îmzekerê nas bike an destûr bide belgeyê. Digel vê yekê, naveroka QR Code dikare bi bişkojkên kesane bi bernameyê were şîfrekirin û şîfrekirin. Ew gelek jêhatîbûnê vedike da ku daneyên hesas di hundurê belgeyên giştî de parve bike. Piştî ku bikarhênerê îmzakirî dikare nûve bike, verast bike, jêbibe, pêşdîtin bike an li Kodên QR di nav PDF, belgeyên MS Word, pirtûkên xebatê yên MS Excel, pêşandanên MS PowerPoint, pelên Adobe Photoshop û cûrbecûr formên wêneyan de nûve bike, verast bike, jê bibe, pêşdîtin an bigere. Kodên QR dikarin ji hêla din ve bêne xweş kirin.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Gavên îmzekirina Rtf bi Qrcode di Java de"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) îmzakirina belgeyên Rtf bi îmzeyên Qrcode zû û bi hêsanî peyda dike.
        
        * Nimûneyek ji çîna îmzayê biafirîne ku pelê {{Pelformat}} pêşkêş dike ku divê wekî rêyek an herikîna bîranînê were îmzekirin
        * Dersa SignOptions destnîşan bikin û hemî daneyên daxwazkirî bicîh bikin.
        * Rêbaza Signature.Sign() vexwend ku derana pelê {{Pelformat}} an jî herikîna bîrê derbas dike

    title_right: " Pêdiviyên Sîstemê"
    content_right: |
        GroupDocs.Signature for Java li ser hemî platform û pergalên xebitandinê yên sereke têne piştgirî kirin. Berî ku hûn koda jêrîn bicîh bikin, ji kerema xwe pê ewle bibin ku we şertên jêrîn li ser pergala we hatine saz kirin.

        * Pergalên xebitandinê: Microsoft Windows, Linux, MacOS
        * Jîngehên pêşkeftinê: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Nûtirîn GroupDocs.Signature for Java ji [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature) bistînin
         
    code: |
        ```java    
                
        // Set up input Rtf file
        String filePath = "input.rtf";
        // Set up output file
        String outputFilePath = "output.rtf";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // create barcode option with predefined barcode text
        BarcodeSignOptions options = new BarcodeSignOptions("John Smith");

        // setup Barcode encoding type
        options.setEncodeType(QrCodeTypes.Data Matrix);

        // set signature position
        options.setLeft(50);
        options.setTop(50);
        options.setWidth(200);
        options.setHeight(50);

        // sign Rtf document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Îmzekirina belgeyên {{Pelformat}} bi Qrcode Demoya Zindî"
    content: |
       Naha bi serdana malpera [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) pelê Rtf bi îmzeyên cihêreng îmze bikin. Demoya serhêl a belaş li benda we ye.

              
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-barcode"
          title: "About Data Matrix QrCode"
          content: |
            Data Matrix kodek du-alî ye ku ji 'hucreyên' reş û spî an jî xalên ku bi rengek çargoşe an çargoşe hatine rêz kirin, ku wekî matrix jî tê zanîn, pêk tê. Agahdariya ku were kod kirin dikare daneyên nivîsê an hejmarî be.
          characterset: |
             Hemî 256 tîpên ASCII, hemî karakterên ISO, û hemî tîpên Koda Veguhastina Dehanî ya Kodkirî ya Berfirehkirî (EBCDIC) piştgirî dike.
          textcapacity: |
             Heya 3116 reqemên hejmarî, an jî 2335 tîpên hejmarî yên alfa, an jî 1556 tîpên binaryê.
          image: |
             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

          link: ""

############################# More Formats ############################
more_formats:
    enable: true
    title: "Îmzeyên din ên piştgirî yên Qrcode ji bo Java"
    content: |
        "Her weha hûn dikarin {{Pelformat}} bi celebên din ên îmzayê re îmze bikin. Ji kerema xwe lîsteya jêrîn bibînin."
    format: 
        
       
back_to_top:
    enable: true
---