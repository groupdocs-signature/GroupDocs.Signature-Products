---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Barcode
codetype: Interleaved2of5
fileformat: Gif
productName: Java
lang: zh
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put  Barcode signature on Gif for Java

############################# Head ############################
head_title: "在 Java 中带有 Interleaved2of5 条码的 eSign Gif 文档"
head_description: "创建 Interleaved2of5 条码签名并使用几行代码将其放在带有 Java 的 Gif 文档中。使用 GroupDocs 文档签名 API 对各种文件格式进行签名。"

############################# Header ############################
title: "在 Java 中为 Gif 文档生成 Interleaved2of5 条码签名"
description: "使用 Interleaved2of5 条码对您的 Gif 业务文档进行电子签名。只需几行代码即可快速轻松地生成条形码签名以设置签名选项。"
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
    title_left: "在 Java 中使用 Barcode 签署 Gif 的步骤"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) 提供使用 Barcode 签名快速轻松地签署 Gif 文档的能力。
        
        * 创建 Signature 类的实例，提供 Gif 文件应该作为路径或内存流进行签名
        * 实例化 SignOptions 类并设置所有需要的数据。
        * 调用 Signature.Sign() 方法传递输出 Gif 文件或内存流

    title_right: " 系统要求"
    content_right: |
        所有主要平台和操作系统都支持 GroupDocs.Signature for Java。在执行以下代码之前，请确保您的系统上安装了以下先决条件。

        * 操作系统：Microsoft Windows、Linux、MacOS
        * 开发环境：NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * 从 [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature) 获取最新的 GroupDocs.Signature for Java
         
    code: |
        ```java    
                
        // Set up input Gif file
        String filePath = "input.gif";
        // Set up output file
        String outputFilePath = "output.gif";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // create barcode option with predefined barcode text
        BarcodeSignOptions options = new BarcodeSignOptions("John Smith");

        // setup Barcode encoding type
        options.setEncodeType(BarcodeTypes.Interleaved2of5);

        // set signature position
        options.setLeft(50);
        options.setTop(50);
        options.setWidth(200);
        options.setHeight(50);

        // sign Gif document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "使用 Barcode 现场演示签署 Gif 文档"
    content: |
       访问 [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) 网站，立即使用各种签名为 Gif 文件签名。免费在线演示等着你。

        
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-barcode"
          title: "About Interleaved2of5 Barcode"
          content: |
            Interleaved 2 of 5 (ITF) 是连续的两宽条码符号编码数字。它在商业上用于 135 胶片、ITF-14 条码和一些产品的纸箱上，而里面的产品标有 UPC 或 EAN。
          characterset: |
             数字 (0-9)。
          textcapacity: |
             可变长度。
          image: |
             iVBORw0KGgoAAAANSUhEUgAAAB8AAACGCAYAAAAlx1GyAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsMAAA7DAcdvqGQAAAFdSURBVHhe7Y0xCkJRAMPe/S/9BSFLqHaSN9hAhyzNeS6y+BUWv8LX+DnnPfjkHtjN4pF2hntgN4tH2hnugd0sHmlnuAd2s3ikneEe2M3ikXaGe2A3i0faGe6B3SweaWe4B3azeKSd4R7YzeKRdoZ7YDeLR9oZ7oHdLB5pZ7gHdrN4pJ3hHtjN4pF2hntgN4tH2hnugd0sHmlnuAd2s3ikneEe2M3ikXaGe2A3i0faGe6B3SweaWe4B3azeKSd4R7YzeKRdoZ7YDeLR9oZ7oHdLB5pZ7gHdrN4pJ3hHtjN4pF2hntgN4tH2hnugd0sHmlnuAd2s3ikneEe2M3ikXaGe2A3i0faGe6B3SweaWe4B3azeKSd4R7YzeKRdoZ7YDeLR9oZ7oHdLB5pZ7gHdrN4pJ3hHtjN4pF2hntgN4tH2hnugd0sHmlnuAd2s3ikneEe2M3X+K9Z/Ar/Gn+eF5E2tt5Q4JATAAAAAElFTkSuQmCC

          link: ""

############################# More Formats ############################
more_formats:
    enable: true
    title: "Java 的其他支持的 Barcode 签名"
    content: |
        "您还可以使用其他签名类型对 Gif 进行签名。请参阅下面的列表。"
    format: 
        
       
back_to_top:
    enable: true
---