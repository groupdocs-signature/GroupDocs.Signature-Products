---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Digital
fileformat: Docm
productName: Java
lang: ko
productCode: java
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Docm for Java

############################# Head ############################
head_title: "{digital-content.meta_title}"
head_description: "{digital-content.meta_description}"

############################# Header ############################
title: "{digital-content.h1}"
description: "{digital-content.h2}"
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
    title: "{digital-about.title}"
    content: |
        {digital-about.content}
    

############################# Steps ############################
steps:
    enable: true
    title_left: "{digital-steps.title}"
    content_left: |
        {digital-steps.content.description}
        
        * {digital-steps.content.step_1}
        * {digital-steps.content.step_2}
        * {digital-steps.content.step_3}

    title_right: " {system-requirements.title}"
    content_right: |
        {system-requirements.content.description}

        * {system-requirements.content.step_1}
        * {system-requirements.content.step_2}
        * Java runtime: J2SE 6.0 and above
        * {system-requirements.content.step_3}
         
    code: |
        ```java    
                
        // Set up input Docm file
        String filePath = "input.docm";
        // Set up output file
        String outputFilePath = "output.docm";
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

        // sign Docm document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Digital 라이브 데모로 Docm 문서 서명"
    content: |
       지금 바로 [GroupDocs.Signature 앱](https://products.groupdocs.app/signature/family) 웹사이트에서 다양한 서명으로 Docm 파일에 서명하세요. 무료 온라인 데모가 여러분을 기다리고 있습니다.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Java에 대해 지원되는 기타 Digital 서명"
    content: |
        "다른 서명 유형으로 Docm에 서명할 수도 있습니다. 아래 목록을 참조하십시오."
    format: 
       
       
back_to_top:
    enable: true
---