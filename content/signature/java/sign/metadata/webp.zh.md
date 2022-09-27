---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Metadata
fileformat: Webp
productName: Java
lang: zh
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Metadata signature on Webp for Java

############################# Head ############################
head_title: "通过 Java 将元数据电子签名附加到 Webp 文档"
head_description: "使用几行 Java 代码将元数据用作 Webp 文档中的隐藏电子签名。使用 GroupDocs 文档签名 API 使用元数据信息对您的业务文档和文件进行电子签名。"

############################# Header ############################
title: "通过 Java 的 Webp 文档的元数据电子签名简单易用！"
description: "使用隐藏的元数据条目对您的 Webp 文档和合同进行电子签名。为 PDF、MS Word 文档、MS Excel 工作簿、MS PowerPoint 演示文稿和各种图像格式生成元数据，没有问题和额外的编码。"
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
    title: "{metadata-about.title}"
    content: |
        {metadata-about.content}
    

############################# Steps ############################
steps:
    enable: true
    title_left: "{metadata-steps.title}"
    content_left: |
        {metadata-steps.content.description}
        
        * {metadata-steps.content.step_1}
        * {metadata-steps.content.step_2}
        * {metadata-steps.content.step_3}

    title_right: " {system-requirements.title}"
    content_right: |
        {system-requirements.content.description}

        * {system-requirements.content.step_1}
        * {system-requirements.content.step_2}
        * Java runtime: J2SE 6.0 and above
        * {system-requirements.content.step_3}
         
    code: |
        ```java    
                
        // Set up input Webp file
        String filePath = "input.webp";
        // Set up output file
        String outputFilePath = "output.webp";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // instantiate metadata signing options
        MetadataSignOptions options = new MetadataSignOptions();

        // Specify different Metadata Signatures and add them to options signature collection
        // set start id
        int imgsMetadataId = 41996;
        // setup int value
        ImageMetadataSignature mdSign_DocId = new ImageMetadataSignature(imgsMetadataId++, 123456); // int
        options.getSignatures().add(mdSign_DocId);
        // setup Author property
        ImageMetadataSignature mdSign_Author = new ImageMetadataSignature(imgsMetadataId++, "Mr.Scherlock Holmes"); // string
        options.getSignatures().add(mdSign_Author);
        // setup data of sign date
        ImageMetadataSignature mdSign_Date = new ImageMetadataSignature(imgsMetadataId++, new Date()); // DateTime
        options.getSignatures().add(mdSign_Date);
        // setup double
        ImageMetadataSignature mdSign_Amnt = new ImageMetadataSignature(imgsMetadataId++, 123.456); //decimal value
        options.getSignatures().add(mdSign_Amnt);

        // sign Webp document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "使用 Metadata 现场演示签署 Webp 文档"
    content: |
       访问 [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) 网站，立即使用各种签名为 Webp 文件签名。免费在线演示等着你。          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Java 的其他支持的 Metadata 签名"
    content: |
        "您还可以使用其他签名类型对 Webp 进行签名。请参阅下面的列表。"
    format: 
       
       
back_to_top:
    enable: true
---