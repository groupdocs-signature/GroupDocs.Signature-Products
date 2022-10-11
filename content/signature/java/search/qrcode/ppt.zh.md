---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Search
signaturetype: Qrcode
fileformat: Ppt
productName: Java
lang: zh
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Search Qrcode signatures at Ppt with Java

############################# Head ############################
head_title: "在 Java 的 Ppt 文件中搜索 Qrcode 签名"
head_description: "使用 Java 通过几行代码在 Ppt 文件中搜索 Qrcode 签名。"

############################# Header ############################
title: "在 Ppt 文件中搜索 Qrcode 签名"
description: "Java 原生 API 允许在已签名的 Ppt 文件中搜索 Qrcode 签名。使用几行代码在您的 Ppt 文档中执行高级电子签名搜索。"
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
    title: "关于 GroupDocs.Signature for Java API"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) 提供 Java API 用于处理使用各种签名类型的文档，例如文本、图像、数字证书、条形码、QR 码、图章或元数据。用户可以在 PDF、MS Word 文档、MS Excel 工作簿、MS PowerPoint 演示文稿、Adobe Photoshop 文件和各种图像格式中添加、删除、更新、验证或搜索电子签名，并根据需要额外支持自定义签名属性。
    

############################# Steps ############################
steps:
    enable: true
    title_left: "如何在 Ppt 中搜索 Qrcode 签名"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) 让 Java 开发人员通过执行几个简单的步骤，可以更轻松地从他们的应用程序中搜索 Ppt 文件中的 Qrcode 签名。
        
        * 创建 Signature 类的新实例并将源文档路径作为构造函数参数传递。
        * 根据您的要求实例化 SearchOptions 对象并指定搜索选项。
        * 调用 Signature 类实例的 Search 方法并将 SearchOptions 传递给它。
        * 根据您的需求处理搜索结果。

    title_right: "系统要求"
    content_right: |
        所有主要平台和操作系统都支持 GroupDocs.Signature for Java。在执行以下代码之前，请确保您的系统上安装了以下先决条件。

        * 操作系统：Microsoft Windows、Linux、MacOS
        * 开发环境：NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * 从 [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature) 下载最新版本的 GroupDocs.Signature for Java
         
    code: |
        ```java    
                
        // Set up input Ppt file
        String filePath = "input.ppt";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Create search options
        QrCodeSearchOptions options = new QrCodeSearchOptions();

        // specify special pages to search on 
        options.setAllPages(false);
        // single page number
        options.setPageNumber(1);
        // specify text match type
        options.setMatchType(TextMatchType.Contains);
        // specify text pattern to search
        options.setText("Text signature");
        // return  Qrcode images for processing
        options.setReturnContent(true);
        // set up type of returned  Qrcode images
        options.setReturnContentType(FileType.PNG);
                            
        // search for Qrcode signatures in Ppt document
        List<QrCodeSignature> signatures = signature.search(QrCodeSignature.class, options);

        // process signatures which were found 
        signatures.forEach(item -> System.out.println(item.toString()));
        ```

############################# Demos ############################
demos:
    enable: true
    title: "搜索 Qrcode 电子签名 Live Demo"
    content: |
       立即访问 [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) 网站，在文档中搜索 Ppt 文件的各种电子签名。

        
############################# More Formats ############################
more_formats:
    enable: true
    title: "使用 Java 搜索其他 Qrcode 签名"
    content: |
        "在各种文档中搜索电子签名。从一种流行的文件格式中查找签名，如下所示。"
    format: 
           
       
back_to_top:
    enable: true
---