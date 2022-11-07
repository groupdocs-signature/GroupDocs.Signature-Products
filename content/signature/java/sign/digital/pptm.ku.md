---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Digital
fileformat: Pptm
productName: Java
lang: ku
productCode: java
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Pptm for Java

############################# Head ############################
head_title: "Zêdekirina îmzeyên elektronîkî yên dîjîtal li pelê Pptm bi Java"
head_description: "Ji bo Java bi çend rêzikên kodê Îmzeya Dîjîtal bixin ser pelê {{Pelformat}}. API-ya Îmzekirina Belgeya GroupDocs bikar bînin da ku bi dehan formatên pelan îmze bikin."

############################# Header ############################
title: "eSign Pptm pelên bi Digital di Java de"
description: "Meriv çawa bi çend rêzikên koda Java nîşana Digital zêde bike"
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
    title: "Derbarê GroupDocs.Signature for Java API-ya îmzeyên dîjîtal"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) API-ya populer e ku bi îmzeyên elektronîkî yên dîjîtal, bi sertîfîkayên dîjîtal ve, belgeyan çêdike. Ji bo îmzeyên dîjîtal API pelên sertîfîkayên PFX bikar tîne da ku belgeyê bi bişkojkên taybet û giştî yên parastî bi şîfreyê veqetîne. Dibe ku îmzeyên dîjîtal ji bo pejirandina belgeyên karsaziyê bi rûpela taybetî ya eSign PDF-ê re, pejirandina tevahî belgeyên Microsoft Office yên mîna Words, Excel, pelên Powerpoint, û belgeyên Open Office-ê werin bikar anîn. Xerîdar dikarin bi hêsanî îmzeyan wekî sererastkirina wan, rakirin an sererastkirina wan manîpule bikin. API ji bo lêgerîn û verastkirina îmzeyan rêyek peyda dike. Digel vê yekê, ji bo xwerûkirina îmzeyan gelek jêhatî têne peyda kirin.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Gavên îmzekirina Pptm bi Digital di Java de"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) îmzakirina belgeyên Pptm bi îmzeyên Digital zû û bi hêsanî peyda dike.
        
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
                
        // Set up input Pptm file
        String filePath = "input.pptm";
        // Set up output file
        String outputFilePath = "output.pptm";
        // Provide digital certificate
        String certificateFilePath = "certificate.pfx";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Provide sign options
        DigitalSignOptions options = new DigitalSignOptions(certificateFilePath);

        // set certificate password
        options.setPassword("1234567890");

        // set signature position
        options.setLeft(50);
        options.setTop(200);

        // sign Pptm document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Îmzekirina belgeyên {{Pelformat}} bi Digital Demoya Zindî"
    content: |
       Naha bi serdana malpera [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) pelê Pptm bi îmzeyên cihêreng îmze bikin. Demoya serhêl a belaş li benda we ye.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Îmzeyên din ên piştgirî yên Digital ji bo Java"
    content: |
        "Her weha hûn dikarin {{Pelformat}} bi celebên din ên îmzayê re îmze bikin. Ji kerema xwe lîsteya jêrîn bibînin."
    format: 
       
       
back_to_top:
    enable: true
---