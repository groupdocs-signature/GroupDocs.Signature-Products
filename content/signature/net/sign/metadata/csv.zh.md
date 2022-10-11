---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Metadata
fileformat: Csv
productName: .NET
lang: zh
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Metadata signature on Csv for C#

############################# Head ############################
head_title: "通过 C# 将元数据电子签名附加到 Csv 文档"
head_description: "使用几行 C# 代码将元数据用作 Csv 文档中的隐藏电子签名。使用 GroupDocs 文档签名 API 使用元数据信息对您的业务文档和文件进行电子签名。"

############################# Header ############################
title: "通过 .NET 的 Csv 文档的元数据电子签名简单易用！"
description: "使用隐藏的元数据条目对您的 Csv 文档和合同进行电子签名。为 PDF、MS Word 文档、MS Excel 工作簿、MS PowerPoint 演示文稿和各种图像格式生成元数据，没有问题和额外的编码。"
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true

    left:
        img_alt: "GroupDocs.Signature for .NET"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocs-signature-net.png"
        product: "GroupDocs.Signature"
        platform: ".NET"



############################# About ############################
about:
    enable: true
    title: "关于 GroupDocs.Signature for .NET 元数据签名 API"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) 是用于数字文档电子签名的流行 API。可以使用文本、图像、数字证书、条形码、二维码、印章或元数据等签名。签名可以放在 PDF、MS Word 文档、MS Excel 工作簿、MS PowerPoint 演示文稿、Adobe Photoshop 文件和各种图像格式上。客户可以签署他们的文件并更新、搜索、验证、删除或预览放在这些文件上的电子签名。此外，还提供了许多签名定制的能力。
    

############################# Steps ############################
steps:
    enable: true
    title_left: "在 C# 中使用 Metadata 签署 Csv 的步骤"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) 提供使用 Metadata 签名快速轻松地签署 Csv 文档的能力。
        
        * 创建 Signature 类的实例，提供 Csv 文件应该作为路径或内存流进行签名
        * 实例化 SignOptions 类并设置所有需要的数据。
        * 调用 Signature.Sign() 方法传递输出 Csv 文件或内存流

    title_right: " 系统要求"
    content_right: |
        所有主要平台和操作系统都支持 GroupDocs.Signature for .NET。在执行以下代码之前，请确保您的系统上安装了以下先决条件。

        * 操作系统：Microsoft Windows、Linux、MacOS
        * 开发环境：Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * 从 [Nuget](https://www.nuget.org/packages/groupdocs.signature) 获取最新的 GroupDocs.Signature for .NET
         
    code: |
        ```csharp    
        
        // Set up input Csv file
        string filePath = "input.csv";
        // Set up output file
        string outputFilePath = "output.csv";

        // Instantiate Signature for input file
        using (var signature = new GroupDocs.Signature.Signature(filePath))
        {
                // instantiate metadata signing options
                var options = new MetadataSignOptions();

                // setup Author property
                SpreadsheetMetadataSignature mdSign_Author = new SpreadsheetMetadataSignature("Author", "Mr.Scherlock Holmes");// String value
                options.Signatures.Add(mdSign_Author);
                // setup document data
                SpreadsheetMetadataSignature mdSign_DocData = new SpreadsheetMetadataSignature("CreatedOn", DateTime.Now);// Datetime value
                options.Signatures.Add(mdSign_DocData);
                // setup document id
                SpreadsheetMetadataSignature mdSign_DocId = new SpreadsheetMetadataSignature("DocumentId", 123456);// Integer value
                options.Signatures.Add(mdSign_DocId);
                
                // sign Csv document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "使用 Metadata 现场演示签署 Csv 文档"
    content: |
       访问 [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) 网站，立即使用各种签名为 Csv 文件签名。免费在线演示等着你。          

############################# More Formats ############################
more_formats:
    enable: true
    title: "C# 的其他支持的 Metadata 签名"
    content: |
        "您还可以使用其他签名类型对 Csv 进行签名。请参阅下面的列表。"
    format: 
       
       
back_to_top:
    enable: true
---