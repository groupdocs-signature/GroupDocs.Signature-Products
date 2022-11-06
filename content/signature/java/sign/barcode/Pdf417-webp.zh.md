---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Barcode
codetype: Pdf417
fileformat: Webp
productName: Java
lang: zh
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put  Barcode signature on Webp for Java

############################# Head ############################
head_title: "在 Java 中带有 Pdf417 条码的 eSign Webp 文档"
head_description: "创建 Pdf417 条码签名并使用几行代码将其放在带有 Java 的 Webp 文档中。使用 GroupDocs 文档签名 API 对各种文件格式进行签名。"

############################# Header ############################
title: "在 Java 中为 Webp 文档生成 Pdf417 条码签名"
description: "使用 Pdf417 条码对您的 Webp 业务文档进行电子签名。只需几行代码即可快速轻松地生成条形码签名以设置签名选项。"
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
    title_left: "在 Java 中使用 Barcode 签署 Webp 的步骤"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) 提供使用 Barcode 签名快速轻松地签署 Webp 文档的能力。
        
        * 创建 Signature 类的实例，提供 Webp 文件应该作为路径或内存流进行签名
        * 实例化 SignOptions 类并设置所有需要的数据。
        * 调用 Signature.Sign() 方法传递输出 Webp 文件或内存流

    title_right: " 系统要求"
    content_right: |
        所有主要平台和操作系统都支持 GroupDocs.Signature for Java。在执行以下代码之前，请确保您的系统上安装了以下先决条件。

        * 操作系统：Microsoft Windows、Linux、MacOS
        * 开发环境：NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * 从 [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature) 获取最新的 GroupDocs.Signature for Java
         
    code: |
        ```java    
                
        // Set up input Webp file
        String filePath = "input.webp";
        // Set up output file
        String outputFilePath = "output.webp";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // create barcode option with predefined barcode text
        BarcodeSignOptions options = new BarcodeSignOptions("John Smith");

        // setup Barcode encoding type
        options.setEncodeType(BarcodeTypes.Pdf417);

        // set signature position
        options.setLeft(50);
        options.setTop(50);
        options.setWidth(200);
        options.setHeight(50);

        // sign Webp document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "使用 Barcode 现场演示签署 Webp 文档"
    content: |
       访问 [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) 网站，立即使用各种签名为 Webp 文件签名。免费在线演示等着你。

        
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-barcode"
          title: "About Pdf417 Barcode"
          content: |
            PDF417 是一种堆叠线性条码格式，用于各种应用，例如运输、身份证和库存管理。
          characterset: |
             所有 256 个 ASCII 字符。
          textcapacity: |
             最多 800 个字符。
          image: |
             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n5CyNd2mE6YM3C103eeW7u1GcDbbfbpDbg48fhVus6H3LuXJRLf9hK77TGz77Q7qm05whu1ugne3grPZ7tMdcnPg8atwmw29dylPJrrtJ3TdZ2Lbb3dQ33SCM2x3E7y7FZzNdp/ukJsDj1+F22zovUt5MtFtP6HrPhPbfruD+qYTnGG7m+DdreBstvt0h9wcePwq3GZD713Kk4lu+wld95nY9tsd1Ded4Azb3QTvbgVns92nO+TmwONX4TYbeu9Snkx020/ous/Ett/uoL7pBGfY7iZ4dys4m+0+3SE3Bx6/CrfZ0HuX8mSi235C130mtv12B/VNJzjDdjfBu1vB2Wz36Q65OfD4VbjNZrvn7t735MR2750FZ1Pf1N2Ugbt735MT3ZuN4Gy2+3SH3Bx4/CrcZrPdc3fve3Jiu/fOgrOpb+puysDdve/Jie7NRnA22326Q24OPH4VbrPZ7rm79z05sd17Z8HZ1Dd1N2Xg7t735ET3ZiM4m+0+3SE3Bx6/CrfZbPfc3fuenNjuvbPgbOqbupsycHfve3Kie7MRnM12n+6QmwOPX4XbbLZ77u59T05s995ZcDb1Td1NGbi79z050b3ZCM5mu093yM2Bx6/CbTbbPXf3vicntnvvLDib+qbupgzc3fuenOjebARns92nO+TmwONX4Tab17013eYzkXbOE9s9O++nbOh/awfebwVns92nO+TmwONX4Tab17013eYzkXbOE9s9O++nbOh/awfebwVns92nO+TmwONX4Tab17013eYzkXbOE9s9O++nbOh/awfebwVns92nO+TmwONX4Tab17013eYzkXbOE9s9O++nbOh/awfebwVns92nO+TmwONX4Tab17013eYzkXbOE9s9O++nbOh/awfebwVns92nO+TmwONX4Tab17013eYzkXbOE9s9O++nbOh/awfebwVns92nO+TmwONX4TYbeu+coW6r4LylfqsKzqa++WkHaVe/UXtnqNtqYuqhfutGcDbbfbpDbg48fhVus6H3zhnqtgrOW+q3quBs6pufdpB29Ru1d4a6rSamHuq3bgRns92nO+TmwONX4TYbeu+coW6r4LylfqsKzqa++WkHaVe/UXtnqNtqYuqhfutGcDbbfbpDbg48fhVus6H3zhnqtgrOW+q3quBs6pufdpB29Ru1d4a6rSamHuq3bgRns92n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

          link: ""

############################# More Formats ############################
more_formats:
    enable: true
    title: "Java 的其他支持的 Barcode 签名"
    content: |
        "您还可以使用其他签名类型对 Webp 进行签名。请参阅下面的列表。"
    format: 
        
       
back_to_top:
    enable: true
---