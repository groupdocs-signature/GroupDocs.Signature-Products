---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Metadata
fileformat: Wmf
productName: .NET
lang: zh
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Metadata signature on Wmf for C#

############################# Head ############################
head_title: "通过 C# 将元数据电子签名附加到 Wmf 文档"
head_description: "使用几行 C# 代码将元数据用作 Wmf 文档中的隐藏电子签名。使用 GroupDocs 文档签名 API 使用元数据信息对您的业务文档和文件进行电子签名。"

############################# Header ############################
title: "通过 .NET 的 Wmf 文档的元数据电子签名简单易用！"
description: "使用隐藏的元数据条目对您的 Wmf 文档和合同进行电子签名。为 PDF、MS Word 文档、MS Excel 工作簿、MS PowerPoint 演示文稿和各种图像格式生成元数据，没有问题和额外的编码。"
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
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * {system-requirements.content.step_3}
         
    code: |
        ```csharp    
        
        // Set up input Wmf file
        string filePath = "input.wmf";
        // Set up output file
        string outputFilePath = "output.wmf";

        // Instantiate Signature for input file
        using (var signature = new GroupDocs.Signature.Signature(filePath))
        {
                // instantiate metadata signing options
                MetadataSignOptions options = new MetadataSignOptions();

                // Specify different Metadata Signatures and add them to options signature collection
                // set start id
                ushort imgsMetadataId = 41996;
                // setup int value
                ImageMetadataSignature mdSign_DocId = new ImageMetadataSignature(imgsMetadataId++, 123456); // int
                options.Signatures.Add(mdSign_DocId);
                // setup Author property
                ImageMetadataSignature mdSign_Author = new ImageMetadataSignature(imgsMetadataId++, "Mr.Scherlock Holmes"); // string
                options.Signatures.Add(mdSign_Author);
                // setup data of sign date
                ImageMetadataSignature mdSign_Date = new ImageMetadataSignature(imgsMetadataId++, DateTime.Now); // DateTime
                options.Signatures.Add(mdSign_Date);
                // setup double
                ImageMetadataSignature mdSign_Amnt = new ImageMetadataSignature(imgsMetadataId++, 123.456M); //decimal value
                options.Signatures.Add(mdSign_Amnt);

                // sign Wmf document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "使用 Metadata 现场演示签署 Wmf 文档"
    content: |
       访问 [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) 网站，立即使用各种签名为 Wmf 文件签名。免费在线演示等着你。          

############################# More Formats ############################
more_formats:
    enable: true
    title: "C# 的其他支持的 Metadata 签名"
    content: |
        "您还可以使用其他签名类型对 Wmf 进行签名。请参阅下面的列表。"
    format: 
       
       
back_to_top:
    enable: true
---