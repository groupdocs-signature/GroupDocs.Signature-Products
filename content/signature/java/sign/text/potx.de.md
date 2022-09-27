---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Text
fileformat: Potx
productName: Java
lang: de
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Text signature on Potx for Java

############################# Head ############################
head_title: "{text-content.meta_title}"
head_description: "{text-content.meta_description}"

############################# Header ############################
title: "{text-content.h1}"
description: "{text-content.h2}"
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
    title: "{text-about.title}"
    content: |
        {text-about.content}
    

############################# Steps ############################
steps:
    enable: true
    title_left: "{text-steps.title}"
    content_left: |
        {text-steps.content.description}
        
        * {text-steps.content.step_1}
        * {text-steps.content.step_2}
        * {text-steps.content.step_3}

    title_right: " {system-requirements.title}"
    content_right: |
        {system-requirements.content.description}

        * {system-requirements.content.step_1}
        * {system-requirements.content.step_2}
        * Java runtime: J2SE 6.0 and above
        * {system-requirements.content.step_3}
         
    code: |
        ```java    
                
        // Set up input Potx file
        String filePath = "input.potx";
        // Set up output file
        String outputFilePath = "output.potx";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Provide sign options
        TextSignOptions options = new TextSignOptions("John Smith");

        // set signature position
        options.setLeft(50);
        options.setTop(200);

        // sign Potx document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Signieren von Potx-Dokumenten mit Text Live-Demo"
    content: |
       Signieren Sie die Datei Potx jetzt mit verschiedenen Signaturen, indem Sie die Website [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) besuchen. Kostenlose Online-Demo wartet auf Sie.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Andere unterstützte Text-Signaturen für Java"
    content: |
        "Sie können Potx auch mit anderen Signaturtypen signieren. Bitte sehen Sie sich die Liste unten an."
    format: 
       
       
back_to_top:
    enable: true
---