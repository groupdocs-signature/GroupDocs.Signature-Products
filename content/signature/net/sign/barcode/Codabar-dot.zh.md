---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Barcode
codetype: Codabar
fileformat: Dot
productName: .NET
lang: zh
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put  Barcode signature on Dot for C#

############################# Head ############################
head_title: "在 C# 中带有 Codabar 条码的 eSign Dot 文档"
head_description: "创建 Codabar 条码签名并使用几行代码将其放在带有 .NET 的 Dot 文档中。使用 GroupDocs 文档签名 API 对各种文件格式进行签名。"

############################# Header ############################
title: "在 C# 中为 Dot 文档生成 Codabar 条码签名"
description: "使用 Codabar 条码对您的 Dot 业务文档进行电子签名。只需几行代码即可快速轻松地生成条形码签名以设置签名选项。"
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
    title: "关于 GroupDocs.Signature for .NET 条码签名 API。"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) 是一个快速简便的 API，用于使用 UPCA、UPCE、EAN13、EAN14、Code39、Code39Extended、Code128、Codabar、Postnet、ISBN 等条码类型管理数字文档电子签名, ITF14 和许多其他的。客户可以轻松创建提供所需文本的条码，并将它们放在 PDF、Microsoft Office Words 文档、Microsoft Office Excel 工作簿、MS PowerPoint 演示文稿、Adobe Photoshop 文件和各种图像格式中。可以更新、搜索、验证、删除或预览放置在文档中的条形码。此外，还支持条码定制。
    

############################# Steps ############################
steps:
    enable: true
    title_left: "在 C# 中使用 Barcode 签署 Dot 的步骤"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) 提供使用 Barcode 签名快速轻松地签署 Dot 文档的能力。
        
        * 创建 Signature 类的实例，提供 Dot 文件应该作为路径或内存流进行签名
        * 实例化 SignOptions 类并设置所有需要的数据。
        * 调用 Signature.Sign() 方法传递输出 Dot 文件或内存流

    title_right: " 系统要求"
    content_right: |
        所有主要平台和操作系统都支持 GroupDocs.Signature for .NET。在执行以下代码之前，请确保您的系统上安装了以下先决条件。

        * 操作系统：Microsoft Windows、Linux、MacOS
        * 开发环境：Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * 从 [Nuget](https://www.nuget.org/packages/groupdocs.signature) 获取最新的 GroupDocs.Signature for .NET
         
    code: |
        ```csharp    
        
        // Set up input Dot file
        string filePath = "input.dot";
        // Set up output file
        string outputFilePath = "output.dot";

        // Instantiate Signature for input file
        using (var signature = new GroupDocs.Signature.Signature(filePath))
        {
                // create barcode option with predefined barcode text
                var options = new BarcodeSignOptions("BC12345678")
                {
                    // setup Barcode encoding type
                    EncodeType = BarcodeTypes.Codabar,

                    // set signature position
                    Left = 50,
                    Top = 50,
                    Width = 200,
                    Height = 50                                        
                };
                
                // sign Dot document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "使用 Barcode 现场演示签署 Dot 文档"
    content: |
       访问 [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) 网站，立即使用各种签名为 Dot 文件签名。免费在线演示等着你。

        
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-barcode"
          title: "About Codabar Barcode"
          content: |
            Codabar 是一种线性条码符号系统，即使在点阵打印机上打印时也能准确读取联邦快递空运单和血库表格等多部分表格。
          characterset: |
             数字 (0-9) 和特殊字符 $/-:+。
          textcapacity: |
             没有具体限制。
          image: |
             iVBORw0KGgoAAAANSUhEUgAAAD0AAABGCAYAAAB/h5zrAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsMAAA7DAcdvqGQAAAK2SURBVHhe7c9BagQBDAPB/f+nNxDQpUCOfc1MQx8khMGf7wN5n34K79NP4X36KYxPfz6fX0OyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2svfi3/I+/RTeJ9+Cg98+vv9AViQgD/8yuhqAAAAAElFTkSuQmCC

          link: ""

############################# More Formats ############################
more_formats:
    enable: true
    title: "C# 的其他支持的 Barcode 签名"
    content: |
        "您还可以使用其他签名类型对 Dot 进行签名。请参阅下面的列表。"
    format: 
        
       
back_to_top:
    enable: true
---