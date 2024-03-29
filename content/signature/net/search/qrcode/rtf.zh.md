---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Search
signaturetype: Qrcode
fileformat: Rtf
productName: .NET
lang: zh
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Search Qrcode signatures at Rtf with C#

############################# Head ############################
head_title: "在 C# 的 Rtf 文件中搜索 Qrcode 签名"
head_description: "使用 .NET 通过几行代码在 Rtf 文件中搜索 Qrcode 签名。"

############################# Header ############################
title: "在 Rtf 文件中搜索 Qrcode 签名"
description: ".NET 原生 API 允许在已签名的 Rtf 文件中搜索 Qrcode 签名。使用几行代码在您的 Rtf 文档中执行高级电子签名搜索。"
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true

    left:
        img_alt: "GroupDocs.Signature for .NET"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocsature-net.png"
        product: "GroupDocs.Signature"
        platform: ".NET"



############################# About ############################
about:
    enable: true
    title: "关于 GroupDocs.Signature for .NET API"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) 提供 .NET API 用于处理使用各种签名类型的文档，例如文本、图像、数字证书、条形码、QR 码、图章或元数据。用户可以在 PDF、MS Word 文档、MS Excel 工作簿、MS PowerPoint 演示文稿、Adobe Photoshop 文件和各种图像格式中添加、删除、更新、验证或搜索电子签名，并根据需要额外支持自定义签名属性。
    

############################# Steps ############################
steps:
    enable: true
    title_left: "如何在 Rtf 中搜索 Qrcode 签名"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) 让 .NET 开发人员通过执行几个简单的步骤，可以更轻松地从他们的应用程序中搜索 Rtf 文件中的 Qrcode 签名。
        
        * 创建 Signature 类的新实例并将源文档路径作为构造函数参数传递。
        * 根据您的要求实例化 SearchOptions 对象并指定搜索选项。
        * 调用 Signature 类实例的 Search 方法并将 SearchOptions 传递给它。
        * 根据您的需求处理搜索结果。

    title_right: "系统要求"
    content_right: |
        所有主要平台和操作系统都支持 GroupDocs.Signature for .NET。在执行以下代码之前，请确保您的系统上安装了以下先决条件。

        * 操作系统：Microsoft Windows、Linux、MacOS
        * 开发环境：Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * 从 [Nuget](https://www.nuget.org/packages/groupdocs.signature) 下载最新版本的 GroupDocs.Signature for .NET
         
    code: |
        ```csharp    
                
        // Set up input Rtf file
        string filePath = "input.rtf";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                //Create search options
                QrCodeSearchOptions options = new QrCodeSearchOptions()
                {
                    // specify special pages to search on 
                    AllPages = false,
                    // single page number
                    PageNumber = 1,
                    // set up text match type
                    MatchType = TextMatchType.Contains,
                    // specify text pattern to search
                    Text = "Text signature",
                    // return  Qrcode images for processing
                    ReturnContent = true,
                    // set up type of returned  Qrcode images
                    ReturnContentType = FileType.PNG
                };

                // search for Qrcode signatures in Rtf document
                List<QrCodeSignature> signatures = signature.Search<QrCodeSignature>(options);

                // process signatures which were found                
                foreach (QrCodeSignature item in signatures)
                {
                    //...
                }
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "搜索 Qrcode 电子签名 Live Demo"
    content: |
       立即访问 [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) 网站，在文档中搜索 Rtf 文件的各种电子签名。

        
############################# More Formats ############################
more_formats:
    enable: true
    title: "使用 C# 搜索其他 Qrcode 签名"
    content: |
        "在各种文档中搜索电子签名。从一种流行的文件格式中查找签名，如下所示。"
    format: 
           
       
back_to_top:
    enable: true
---