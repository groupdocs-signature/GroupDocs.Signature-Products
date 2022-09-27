---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Delete
signaturetype: Barcode
fileformat: Dotx
productName: .NET
lang: zh
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Barcode signature on Dotx for C#

############################# Head ############################
head_title: "通过 C# 从 Dotx 文件中删除 Barcode 签名"
head_description: "使用简短的 .NET 代码可以轻松地从已签名的 Dotx 文档中删除特定的 Barcode 签名。"

############################# Header ############################
title: "删除放置在 Dotx 文件中的 Barcode 签名"
description: "从 Dotx 文档中删除各种 Barcode 签名。删除 Barcode 签名需要简单的 C# 代码。"
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
    title: "获取有关 GroupDocs.Signature for .NET API 功能的信息"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) API 提供了多种使用电子签名处理文档的方法。可以使用文本、图像、数字证书、条形码、二维码、印章或元数据等数字签名。客户可以在 PDF、MS Word 文档、MS Excel 工作簿、MS PowerPoint 演示文稿、Adobe Photoshop 文件和各种图像格式中添加、删除、更新、验证或搜索数字签名。提供了大量有用的功能和设置。
    

############################# Steps ############################
steps:
    enable: true
    title_left: "如何从您的 Dotx 文档中删除 Barcode 签名"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) 提供了有用的功能，可通过几行代码清除 Barcode 签名的 Dotx 文档。
        
        * 首先，将 Signature 对象传递到您的文档的路径作为构造函数参数进行实例化。
        * 然后，创建适当的签名对象并设置其唯一标识符。
        * 之后，调用 Delete 方法传递必须删除的签名对象。
        * 最后，处理运行结果。

    title_right: "系统要求"
    content_right: |
        所有主要平台和操作系统都支持 GroupDocs.Signature for .NET。在执行以下代码之前，请确保您的系统上安装了以下先决条件。

        * 操作系统：Microsoft Windows、Linux、MacOS
        * 开发环境：Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * 从 [Nuget](https://www.nuget.org/packages/groupdocs.signature) 下载最新版本的 GroupDocs.Signature for .NET
         
    code: |
        ```csharp    
                
        // Set up input Dotx file
        string filePath = "input.dotx";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                // Id of signature which is supposed to be deleted
                // such Id may be obtained as result of search operation
                string id = "07f83369-318b-41ad-a843-732417b912c2";

                // provide signature features to delete
                // set up particular signature id
                BarcodeSignature signatureToDelete = new BarcodeSignature(id);

                // delete signature
                bool deleteResult = signature.Delete(signatureToDelete);

                // process deletion result
                if (deleteResult)
                {
                    Console.WriteLine("Signature was deleted successfully!");
                }
        }
        ```

############################# Demos ############################
demos:
    enable: true
    title: "使用 Barcode 签名进行签名 Live Demo"
    content: |
       访问 [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) 网站，立即为 Dotx 文件添加各种电子签名。          

############################# More Formats ############################
more_formats:
    enable: true
    title: "使用 C# 删除您的 Barcode 签名"
    content: |
        "删除添加到各种文档格式的电子签名。无需额外代码即可快速删除签名。"
    format: 
       
       
back_to_top:
    enable: true
---