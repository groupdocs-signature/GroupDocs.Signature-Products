---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Digital
fileformat: Xls
productName: Java
lang: zh
productCode: java
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Xls for Java

############################# Head ############################
head_title: "使用 Java 将数字电子签名添加到 Xls 文件"
head_description: "使用几行代码为 Java 的 Xls 文件添加数字签名。使用 GroupDocs 文档签名 API 对数十种文件格式进行签名。"

############################# Header ############################
title: "在 Java 中使用 Digital 签名的 eSign Xls 文件"
description: "如何用几行 Java 代码添加 Digital 签名"
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
    title: "关于 GroupDocs.Signature for Java 数字签名 API"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) 是一种流行的 API，用于使用数字电子签名和数字证书对文档进行签名。对于数字签名 API，使用 PFX 证书文件来设计带有密码保护的私钥和公钥的文档。数字签名可用于验证具有 eSign PDF 特定页面的商业文档，验证整个 Microsoft Office 文档，如 Words、Excel、Powerpoint 文件和 Open Office 文档。客户可以轻松地操作签名，例如编辑、删除或调整签名。 API 提供了一种搜索和验证签名的方法。此外，还提供了许多签名定制的能力。
    

############################# Steps ############################
steps:
    enable: true
    title_left: "在 Java 中使用 Digital 签署 Xls 的步骤"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) 提供使用 Digital 签名快速轻松地签署 Xls 文档的能力。
        
        * 创建 Signature 类的实例，提供 Xls 文件应该作为路径或内存流进行签名
        * 实例化 SignOptions 类并设置所有需要的数据。
        * 调用 Signature.Sign() 方法传递输出 Xls 文件或内存流

    title_right: " 系统要求"
    content_right: |
        所有主要平台和操作系统都支持 GroupDocs.Signature for Java。在执行以下代码之前，请确保您的系统上安装了以下先决条件。

        * 操作系统：Microsoft Windows、Linux、MacOS
        * 开发环境：NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * 从 [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature) 获取最新的 GroupDocs.Signature for Java
         
    code: |
        ```java    
                
        // Set up input Xls file
        String filePath = "input.xls";
        // Set up output file
        String outputFilePath = "output.xls";
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

        // sign Xls document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "使用 Digital 现场演示签署 Xls 文档"
    content: |
       访问 [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) 网站，立即使用各种签名为 Xls 文件签名。免费在线演示等着你。          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Java 的其他支持的 Digital 签名"
    content: |
        "您还可以使用其他签名类型对 Xls 进行签名。请参阅下面的列表。"
    format: 
       
       
back_to_top:
    enable: true
---