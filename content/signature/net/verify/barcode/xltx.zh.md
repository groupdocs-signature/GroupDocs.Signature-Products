---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Verify
signaturetype: Barcode
fileformat: Xltx
productName: .NET
lang: zh
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Barcode signature on Xltx for C#

############################# Head ############################
head_title: "通过 C# 验证 Xltx 文件的 Barcode 签名"
head_description: "仅使用几行 .NET 代码来验证 Xltx 文档及其 Barcode 签名。"

############################# Header ############################
title: "Xltx 文件的 Barcode 签名验证"
description: ".NET 的 API 提供了验证 Xltx 文档中的 Barcode 签名的机会。您的 Xltx 文档中的电子签名验证可以快速轻松地执行。"
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
    title: "发现新的 GroupDocs.Signature for .NET API 功能"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) API 通过使用电子签名提供了广泛的方法来处理多种文档格式。支持多种类型的数字签名，如文本、图像、数字证书、条形码、二维码、印章或元数据。客户可以在 PDF、MS Word 文档、MS Excel 工作簿、MS PowerPoint 演示文稿、Adobe Photoshop 文件和各种图像格式中添加、删除、编辑、验证或搜索数字签名。提供数量惊人的附加功能和设置。
    

############################# Steps ############################
steps:
    enable: true
    title_left: "如何验证 Xltx 文档中的 Barcode 签名"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) 包括有用的功能，例如验证放置在 Xltx 文档中的 Barcode 签名。利用这个机会，无需实现额外的代码。
        
        * 首先，实例化 Signature 类，提供作为构造函数参数路径到应该被验证的文档。
        * 其次，创建一个新的 VerifyOptions 对象并设置所有必需的属性。
        * 最后，调用 Signature 的对象 Verify 方法，传递 VerifyOptions 实例。
        * 然后处理验证结果。

    title_right: "系统要求"
    content_right: |
        所有主要平台和操作系统都支持 GroupDocs.Signature for .NET。在执行以下代码之前，请确保您的系统上安装了以下先决条件。

        * 操作系统：Microsoft Windows、Linux、MacOS
        * 开发环境：Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * 从 [Nuget](https://www.nuget.org/packages/groupdocs.signature) 下载最新版本的 GroupDocs.Signature for .NET
         
    code: |
        ```csharp    
        
        // Set up input Xltx file
        string filePath = "input.xltx";

        // Instantiate Signature for input file
        using (var signature = new GroupDocs.Signature.Signature(filePath))
        {
                //Provide verification options
                BarcodeVerifyOptions options = new BarcodeVerifyOptions()
                {
                    // process only specified page
                    PageNumber = 3,
                    AllPages = false,
                    // set up text match type
                    MatchType = TextMatchType.Contains,
                    // specify text pattern to search
                    Text = "Special signature",
                };

                // Verify document signatures
                VerificationResult result = signature.Verify(options);

                //process result
                if (result.IsValid)
                {
                    //..
                }
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "使用 Barcode 签名进行签名 Live Demo"
    content: |
       访问 [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) 网站，立即为 Xltx 文件添加各种电子签名。          

############################# More Formats ############################
more_formats:
    enable: true
    title: "使用 C# 验证其他 Barcode 签名"
    content: |
        "验证放置在各种文件中的电子签名。检查流行文件格式的签名质量，如下所示。"
    format: 
       
       
back_to_top:
    enable: true
---