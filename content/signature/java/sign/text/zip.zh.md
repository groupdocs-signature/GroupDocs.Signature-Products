---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Text
fileformat: Zip
productName: Java
lang: zh
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Text signature on Zip for Java

############################# Head ############################
head_title: "使用 Java 为 Zip 文件创建文本电子签名"
head_description: "使用几行代码将 Text 电子签名放在 Java 的 Zip 文件中。使用 GroupDocs 文档签名 API 对数十种文件格式进行签名。"

############################# Header ############################
title: "在 Java 中使用 Text 签名对 Zip 文件进行签名"
description: "如何用几行 Java 代码添加 Text 签名"
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
    title: "关于 GroupDocs.Signature for Java API"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) 是用于数字文档电子签名的流行 API。可以使用文本、图像、数字证书、条形码、二维码、印章或元数据等签名。签名可以放在 PDF、MS Word 文档、MS Excel 工作簿、MS PowerPoint 演示文稿、Adobe Photoshop 文件和各种图像格式上。客户可以签署他们的文件并更新、搜索、验证、删除或预览放在这些文件上的电子签名。此外，还提供了许多签名定制的能力。
    

############################# Steps ############################
steps:
    enable: true
    title_left: "在 Java 中使用 Text 签署 Zip 的步骤"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) 提供使用 Text 签名快速轻松地签署 Zip 文档的能力。
        
        * 创建 Signature 类的实例，提供 Zip 文件应该作为路径或内存流进行签名
        * 实例化 SignOptions 类并设置所有需要的数据。
        * 调用 Signature.Sign() 方法传递输出 Zip 文件或内存流

    title_right: " 系统要求"
    content_right: |
        所有主要平台和操作系统都支持 GroupDocs.Signature for Java。在执行以下代码之前，请确保您的系统上安装了以下先决条件。

        * 操作系统：Microsoft Windows、Linux、MacOS
        * 开发环境：NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * 从 [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature) 获取最新的 GroupDocs.Signature for Java
         
    code: |
        ```java    
                
        // Set up input Zip file
        String filePath = "input.zip";
        // Set up output file
        String outputFilePath = "output.zip";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Provide sign options
        TextSignOptions options = new TextSignOptions("John Smith");

        // set signature position
        options.setLeft(50);
        options.setTop(200);

        // sign Zip document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "使用 Text 现场演示签署 Zip 文档"
    content: |
       访问 [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) 网站，立即使用各种签名为 Zip 文件签名。免费在线演示等着你。          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Java 的其他支持的 Text 签名"
    content: |
        "您还可以使用其他签名类型对 Zip 进行签名。请参阅下面的列表。"
    format: 
       
       
back_to_top:
    enable: true
---