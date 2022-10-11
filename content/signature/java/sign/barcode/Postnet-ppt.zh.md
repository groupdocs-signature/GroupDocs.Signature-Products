---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Barcode
codetype: Postnet
fileformat: Ppt
productName: Java
lang: zh
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put  Barcode signature on Ppt for Java

############################# Head ############################
head_title: "在 Java 中带有 Postnet 条码的 eSign Ppt 文档"
head_description: "创建 Postnet 条码签名并使用几行代码将其放在带有 Java 的 Ppt 文档中。使用 GroupDocs 文档签名 API 对各种文件格式进行签名。"

############################# Header ############################
title: "在 Java 中为 Ppt 文档生成 Postnet 条码签名"
description: "使用 Postnet 条码对您的 Ppt 业务文档进行电子签名。只需几行代码即可快速轻松地生成条形码签名以设置签名选项。"
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
    title: "关于 GroupDocs.Signature for Java 条码签名 API。"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) 是一个快速简便的 API，用于使用 UPCA、UPCE、EAN13、EAN14、Code39、Code39Extended、Code128、Codabar、Postnet、ISBN 等条码类型管理数字文档电子签名, ITF14 和许多其他的。客户可以轻松创建提供所需文本的条码，并将它们放在 PDF、Microsoft Office Words 文档、Microsoft Office Excel 工作簿、MS PowerPoint 演示文稿、Adobe Photoshop 文件和各种图像格式中。可以更新、搜索、验证、删除或预览放置在文档中的条形码。此外，还支持条码定制。
    

############################# Steps ############################
steps:
    enable: true
    title_left: "在 Java 中使用 Barcode 签署 Ppt 的步骤"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) 提供使用 Barcode 签名快速轻松地签署 Ppt 文档的能力。
        
        * 创建 Signature 类的实例，提供 Ppt 文件应该作为路径或内存流进行签名
        * 实例化 SignOptions 类并设置所有需要的数据。
        * 调用 Signature.Sign() 方法传递输出 Ppt 文件或内存流

    title_right: " 系统要求"
    content_right: |
        所有主要平台和操作系统都支持 GroupDocs.Signature for Java。在执行以下代码之前，请确保您的系统上安装了以下先决条件。

        * 操作系统：Microsoft Windows、Linux、MacOS
        * 开发环境：NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * 从 [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature) 获取最新的 GroupDocs.Signature for Java
         
    code: |
        ```java    
                
        // Set up input Ppt file
        String filePath = "input.ppt";
        // Set up output file
        String outputFilePath = "output.ppt";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // create barcode option with predefined barcode text
        BarcodeSignOptions options = new BarcodeSignOptions("John Smith");

        // setup Barcode encoding type
        options.setEncodeType(BarcodeTypes.Postnet);

        // set signature position
        options.setLeft(50);
        options.setTop(50);
        options.setWidth(200);
        options.setHeight(50);

        // sign Ppt document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "使用 Barcode 现场演示签署 Ppt 文档"
    content: |
       访问 [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) 网站，立即使用各种签名为 Ppt 文件签名。免费在线演示等着你。

        
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-barcode"
          title: "About Postnet Barcode"
          content: |
            POSTNET（邮政数字编码技术）是美国邮政服务用来协助引导邮件的条形码符号。
          characterset: |
             数字 (0-9)。
          textcapacity: |
             最多 11 个字符。
          image: |
             iVBORw0KGgoAAAANSUhEUgAAACcAAAAjCAYAAAAXMhMjAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsMAAA7DAcdvqGQAAACeSURBVFhH7c7BCkMxEELR/P9Pp1LoRrCXpi4Cbw5kIRKZtS82x52a407Ncae+HrfWer8Pyr+i/3NcQv/nuIT+z3EJ/X/Ocf9mlxuhsXZ2uREaa2eXG6Gxdna5ERprZ5cbobF2drkRGmtnlxuhsXZ2uREaa2eXG6Gxdna5ERprZ5cbobF2drkRGmtnlxuhsXZ2ubnAHHdqjjt18XF7vwDevzbHqsQWPwAAAABJRU5ErkJggg==

          link: ""

############################# More Formats ############################
more_formats:
    enable: true
    title: "Java 的其他支持的 Barcode 签名"
    content: |
        "您还可以使用其他签名类型对 Ppt 进行签名。请参阅下面的列表。"
    format: 
        
       
back_to_top:
    enable: true
---