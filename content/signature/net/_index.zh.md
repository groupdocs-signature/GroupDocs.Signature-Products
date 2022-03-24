---
############################# Static ############################
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Signature"
product_tag: "signature"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: ".NET 数字签名 API – 电子签名 PDF Word Excel 图像"
head_description: "C# .NET 数字签名 API，电子签名库，用于对 PDF、Word、Excel 电子表格、PowerPoint、图像和图形文档格式进行电子签名."

############################# Header ############################
title: "用于电子签名的本机 .NET API"
description: "将数字签名添加到文档格式并在 .NET 应用程序中实现流行的电子签名类型（文本、图像、二维码、条形码、印章和元数据）。"
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Signature for .NET"
        image: "/border/groupdocs-signature-net.svg"
        product: "GroupDocs.Signature"
        platform: ".NET"

    middle:
        button:
            # button loop
            - link: "#overview"
              text: "概述"

            # button loop
            - link: "#features"
              text: "特征"

            # button loop
            - link: "#support"
              text: "Support"

            # button loop
            - link: "https://products.groupdocs.app/signature"
              text: "Live Demo"

            # button loop
            - link: "https://purchase.groupdocs.com/pricing/signature/net"
              text: "价钱"

    right:
        link_download: "https://downloads.groupdocs.com/signature"
        link_learn: "https://docs.groupdocs.com/signature/net/"
        link_buy: "https://purchase.groupdocs.com"

############################# 概述 ############################
overview:
    enable: true
    content: |
      使用 GroupDocs.Signature for .NET API 以 C#、ASP.NET 和其他基于 .NET 的技术构建应用程序，允许您签署数字业务文档，例如 PDF、Microsoft Word、Excel 电子表格、PowerPoint 演示文稿、图像、OpenDocument 和其他行业标准文件格式，无需安装任何其他软件。这个电子签名库易于使用，.NET 开发人员可以轻松地在其应用程序中添加高级数字签名功能，使用户能够安全地签名、搜索和验证来自流行文档格式的电子签名。它支持实现多种签名类型，如文本、图像、条形码、二维码、表单域、图章和元数据。

      文档签名 API 使您能够使用简单和高级的搜索选项来快速在文档上找到所需的签名。应用签名样式、外观管理和自定义签名属性（如尺寸、阴影、对齐等）的选项也可以通过这个功能丰富的文档签名 API 实现。

      GroupDocs.Signature for .NET 可用于任何支持 .NET 平台的开发环境。它与所有基于 .NET 的语言兼容，并支持可以安装 Mono 或 .NET 框架（包括 .NET Core）的流行操作系统（Windows、Linux、MacOS）。
    tabs:
      enable: true
      
      ## TAB ONE ##
      tab_one:
        description: |
          以下是 .NET 的 GroupDocs.Signature 的概述：
      
        left:
          enable: true
          icon: "fab fa-html5"
          title: "签名类型"
          content: |
            * 文字签名
            * 图像签名
            * 数字签名
            * 二维码签名
            * 条码签名
            * 盖章签名
            * 元数据签名
      
      ## TAB TWO ##
      tab_two:
        description: |
          GroupDocs.Signature for .NET 支持查看所有流行的[文档文件格式](https://docs.groupdocs.com/signature/net/supported-document-formats/)。只需几行代码，即可在您的 .NET 应用程序中添加 PDF 签名、微软办公软件 Word、Excel 电子表格、图像、HTML、Outlook 电子邮件、OneNote、项目和图形查看功能。

        left:
          enable: true
          table:
            # table loop
            - title: "微软办公软件"
              content: |
                * **Word:** DOC, DOCX, DOCM, DOT, DOTX, DOTM, RTF, TXT
                * **Excel:** XLS, XLSX, XLSM, XLSB, XLTM, XLT, XLTM, XLTX, XLAM, SXC, SpreadsheetML
                * **PowerPoint:** PPT, PPTX, PPS, PPSX, PPSM, POT, POTM, POTX, PPTM

        right:
          enable: true
          table:
            # table loop
            - title: "Images & 其他格式"
              content: |
                * **图像**：JPG、BMP、PNG、TIFF、GIF、DCM、WEBP
                * **OpenDocument**：ODT、OTT、OTS、ODS、ODP、OTP、ODG
                * **Jpeg2000**：JP2、JPF、JPX、J2K、J2C、JPM
                * **元文件**：EMF、WMF、CMX
                * **便携式**：PDF
                * **可缩放矢量图形**：CDR、SVG
                * **Adobe Photoshop**：PSD
                * **其他**：DJVU

      ## TAB THREE ##
      tab_three:
        description: |
          GroupDocs.Signature for .NET 支持以下操作系统、框架和包管理器:
        
        left:
          enable: true
          table:
            # table loop
            - icon: "fab fa-windows"
              title: "操作系统"
              content: |
                * Windows Desktop
                * Windows Server
                * Windows Azure
                * Linux
                * MacOS

            # table loop
            - icon: "fas fa-code"
              title: "支持的框架"
              content: |
                * .NET Framework 2.0 或更高版本
                * Mono 框架 1.2 或更高版本
                * .NET 标准 2.0
                * .NET Core 2.0
                * .NET Core 2.1

        right:
          enable: true
          table:
            # table loop
            - icon: "fas fa-box"
              title: "包管理器"
              content: |
                * NuGet

            # table loop
            - icon: "fas fa-tools"
              title: "开发环境"
              content: |
                * Microsoft Visual Studio
                * Xamarin.Android
                * Xamarin.IOS
                * Xamarin.Mac
                * MonoDevelop

############################# 特征 ############################
features:
    enable: true
    title: "GroupDocs.Signature for .NET 特征"

    feature:
      # feature loop
      - icon: "fas fa-copy"
        content: "从支持的文档格式创建、搜索、更新、隐藏、验证和删除电子签名"

      # feature loop
      - icon: "fas fa-eye"
        content: "为 Excel 电子表格指定 XML 高级电子签名 (XAdES)"

      # feature loop
      - icon: "fas fa-bolt"
        content: "Retrieve Image Content from Documents Signed with QR-Code, BarCode & 图像签名s"
      
      # feature loop
      - icon: "fas fa-file-powerpoint"
        content: "Set Height, Width, Margins & Alignment for Text or 图像签名 & Place on Specific Page"

      # feature loop
      - icon: "fas fa-code"
        content: "搜索、验证和数字签名 PowerPoint 演示文档"

      # feature loop
      - icon: "fas fa-cloud"
        content: "使用本机文本水印对文字处理文档格式进行签名"

      # feature loop
      - icon: "fas fa-columns"
        content: "设置图像签名类型，例如圆形或方形并配置边距、字体颜色、旋转"

      # feature loop
      - icon: "fas fa-file-word"
        content: "将数字证书应用于带有签名行的文档、电子表格和 PDF 文件"

      # feature loop
      - icon: "fas fa-envelope"
        content: "对签名文字进行颜色设置、透明度和旋转"

      # feature loop
      - icon: "fas fa-print"
        content: "设置亮度和灰度选项并指定图像中图像签名的缩进"

      # feature loop
      - icon: "fas fa-file-archive"
        content: "嵌入自定义对象、序列化以及加密和解密 PDF 文档的元数据签名值"

      # feature loop
      - icon: "fas fa-lock"
        content: "在 PDF 文档中隐藏、删除或自定义数字签名的外观"

      # feature loop
      - icon: "fas fa-file-code"
        content: "使用数字表单字段和文字签名作为图像、注释、贴纸或水印签署 PDF 文档"
      
      # feature loop
      - icon: "fas fa-fill-drip"
        content: "将签名文字放入 MS Word 和 PDF 文档的表单域"

      # feature loop
      - icon: "fas fa-file-excel"
        content: "指定用于处理 Word 文件的签名或电子签名扩展验证的任意文档页"

      # feature loop
      - icon: "fas fa-heading"
        content: "以不同格式保存已签名的图像文件并将已签名的电子表格导出为图像或多页 TIFF"

      # feature loop
      - icon: "fas fa-project-diagram"
        content: "为签名文件分配、修改和删除密码并将电子签名应用于受密码保护的文件"

      # feature loop
      - icon: "fas fa-cube"
        content: "元数据中带有自定义对象的 eSign 工作表、PowerPoint 幻灯片、Word 文档和图像"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "将签名笔刷样式设置为实体、纹理、线性渐变和径向渐变"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "使用自定义加密二维码文本或数据签署文档"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "使用 DjVu 格式作为图像文档搜索和签名文件"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "通过文件 URL 提取文档信息，例如页数"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "将 CorelDraw 文件搜索、签名和验证为图像文档"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "保留存储在元数据中的已处理或已删除签名信息的历史记录"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "将自定义数据对象、VCard 或电子邮件对象添加到二维码并验证 PDF 文件中的加密二维码"

    more_feature:
      # more_feature_loop
      - title: "Easily Add 数字签名"
        content: |
          GroupDocs.Signature for .NET API 允许您向支持的文件格式添加各种类型的签名。可以使用用于 .NET 的 GroupDocs.Signature 应用签名类型，例如文本、图像、数字、印章、QR 码、条形码和元数据。以下代码示例显示了如何将文本签名应用于 PDF 文档：

          ```cs
          using (Signature signature = new Signature("D:\\sample.pdf"))
          {
            TextSignOptions options = new TextSignOptions("John Smith")
            {
              // 设置文本颜色
              ForeColor = Color.Red
            };
            // 签署文件归档
            signature.Sign("D:\\signed.pdf", options);
          }
          ```
      # more_feature_loop
      - title: "Supported Barcode 签名类型"
        content: "我们的签名操作 API 为您提供将条形码签名应用于支持的文档格式的功能。 GroupDocs.Signature for .NET 支持各种条形码类型，例如 Code128、Code39Extended、Code39Standard、EAN14、EAN8、ITF14、UPCA 和 UPCE。还提供了一个名为“AllTypes”的静态对象，以支持所有已注册的条形码类型。"

      # more_feature_loop
      - title: "搜索签名和证书"
        content: |
          GroupDocs.Signature for .NET API，允许您从 Word 文档、Excel 电子表格和 PDF 文件中搜索数字证书。您还可以获取系统中注册的所有数字证书。还可以使用 GroupDocs.Signature for .NET API 在 Word 文档、Excel 电子表格、图像和 PDF 文件中搜索元数据签名。

          通过 GroupDocs.Signature for .NET API，您可以在任何文档、演示文稿、电子表格、图像以及 PDF 文件中搜索 QR-Code 和 Barcode 签名，并获取搜索进度。您还可以从使用二维签名码签名的文档中搜索自定义数据对象。

      # more_feature_loop
      - title: "条码的高级搜索选项"
        content: "您可以通过 GroupDocs.Signature for .NET API 非常轻松地搜索和定位所需的条形码，因为我们的签名 API 提供了高级搜索选项。这些使您能够在特定页面上搜索条形码，在整个文档中搜索，指定要搜索的不同页面（第一页、最后一页、偶数、奇数）、搜索特定编码类型的条形码、基于特定文本字符串搜索条形码或搜索条形码基于带有“包含”选项的字符串."

############################# Support ############################
support:
    enable: true

############################# Solutions ############################
solutions:
    enable: true
    title: "GroupDocs.Signature 为其他流行的开发环境提供文档查看 API"

    solution:
        # solution loop
        - img_alt: "GroupDocs.Signature for Java"
          image: "/border/groupdocs-signature-java.svg"
          product: "GroupDocs.Signature"
          platform: "Java"
          link: "/signature/java/"

############################# Back to top ###############################
back_to_top:
  enable: true
---