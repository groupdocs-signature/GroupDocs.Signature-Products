---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Verify
signaturetype: Digital
fileformat: Docm
productName: Java
lang: ku
productCode: java
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Docm for Java

############################# Head ############################
head_title: "Verastkirina îmzeyên Digital ji bo pelên Docm bi rêya Java"
head_description: "Tenê çend rêzên koda Java bikar bînin da ku belgeyên Docm û îmzeyên wan ên Digital rast bikin."

############################# Header ############################
title: "Verastkirina îmzeyan ji bo pelên Digital"
description: "API ji bo Java firsendê dide ku hûn îmzeyên Digital li ser belgeyên Docm verast bikin. Verastkirina e-îmzeyan di hundirê belgeyên we yên Docm de dibe ku zû û bi hêsanî were kirin."
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
    title_left: "Meriv çawa îmzeyên Digital di belgeya xweya Docm de rast bike"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) taybetmendîyên bikêrhatî yên wekî verastkirina îmzayên Digital yên ku li belgeyên Docm hatine danîn dihewîne. Vê derfetê bêyî pêkanîna kodek zêde bikar bînin.
        
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
                
        // Set up input Docm file
        String filePath = "input.docm";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Provide verification options
        DigitalVerifyOptions options = new DigitalVerifyOptions();

        // Digital signature comment
        options.setComments("Approved");

        // specify period of signatures
        options.setSignDateTimeFrom(new Date(2020, 12, 12));
        options.setSignDateTimeTo(new Date(2022, 12, 12));
                            
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
    title: "Îmzekirina bi Digital îmzeyan Demoya Zindî"
    content: |
       Bi serdana malpera [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) aniha gelek îmzeyên elektronîkî li pelê Docm zêde bikin.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Bi karanîna Java îmzeyên din ên Digital verast bikin"
    content: |
        "Verastkirina îmzeyên elektronîkî yên ku di belgeyên cihêreng de hatine bicîh kirin. Wekî ku li jêr têne xuyang kirin, kalîteya îmzeyan di formên pelên populer de kontrol bikin."
    format: 
       
       
back_to_top:
    enable: true
---